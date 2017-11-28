---
title: "资源管理：use 关键字 (F#)"
description: "了解有关 F # 关键字使用和 using 函数，可以控制的初始化和资源释放。"
keywords: "visual f#, f#, 函数编程"
author: cartermp
ms.author: phcart
ms.date: 05/16/2016
ms.topic: language-reference
ms.prod: .net
ms.technology: devlang-fsharp
ms.devlang: fsharp
ms.assetid: 00c3040e-859f-4dad-a7b5-7b8d44dc232c
ms.openlocfilehash: d4e8626f07f1c77e52e8fabd5ccc07dbf1fa8ddd
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="resource-management-the-use-keyword"></a><span data-ttu-id="f1536-104">资源管理：use 关键字</span><span class="sxs-lookup"><span data-stu-id="f1536-104">Resource Management: The use Keyword</span></span>

<span data-ttu-id="f1536-105">本主题介绍关键字`use`和`using`函数，可以控制的初始化和资源释放。</span><span class="sxs-lookup"><span data-stu-id="f1536-105">This topic describes the keyword `use` and the `using` function, which can control the initialization and release of resources.</span></span>

## <a name="resources"></a><span data-ttu-id="f1536-106">资源</span><span class="sxs-lookup"><span data-stu-id="f1536-106">Resources</span></span>
<span data-ttu-id="f1536-107">术语*资源*以多种方式使用。</span><span class="sxs-lookup"><span data-stu-id="f1536-107">The term *resource* is used in more than one way.</span></span> <span data-ttu-id="f1536-108">是，资源可以是应用程序使用，如字符串、 图形和类似的内容，但在此上下文中的数据*资源*指软件或操作系统资源，例如图形设备上下文，文件句柄、 网络和数据库连接、 并发对象，如等待句柄，依次类推。</span><span class="sxs-lookup"><span data-stu-id="f1536-108">Yes, resources can be data that an application uses, such as strings, graphics, and the like, but in this context, *resources* refers to software or operating system resources, such as graphics device contexts, file handles, network and database connections, concurrency objects such as wait handles, and so on.</span></span> <span data-ttu-id="f1536-109">由应用程序的这些资源的使用涉及从操作系统或其他资源提供程序，其后是更高版本的资源池，以便它可以提供给另一个应用程序资源的获取。</span><span class="sxs-lookup"><span data-stu-id="f1536-109">The use of these resources by applications involves the acquisition of the resource from the operating system or other resource provider, followed by the later release of the resource to the pool so that it can be provided to another application.</span></span> <span data-ttu-id="f1536-110">当应用程序不释放回常见的池的资源时，将发生的问题。</span><span class="sxs-lookup"><span data-stu-id="f1536-110">Problems occur when applications do not release resources back to the common pool.</span></span>

## <a name="managing-resources"></a><span data-ttu-id="f1536-111">管理资源</span><span class="sxs-lookup"><span data-stu-id="f1536-111">Managing Resources</span></span>
<span data-ttu-id="f1536-112">若要有效地负责任地管理应用程序中的资源，你必须立即和可预测的方式释放资源。</span><span class="sxs-lookup"><span data-stu-id="f1536-112">To efficiently and responsibly manage resources in an application, you must release resources promptly and in a predictable manner.</span></span> <span data-ttu-id="f1536-113">.NET Framework 可帮助你执行此操作通过提供`System.IDisposable`接口。</span><span class="sxs-lookup"><span data-stu-id="f1536-113">The .NET Framework helps you do this by providing the `System.IDisposable` interface.</span></span> <span data-ttu-id="f1536-114">实现一种`System.IDisposable`具有`System.IDisposable.Dispose`方法，正确地释放资源。</span><span class="sxs-lookup"><span data-stu-id="f1536-114">A type that implements `System.IDisposable` has the `System.IDisposable.Dispose` method, which correctly frees resources.</span></span> <span data-ttu-id="f1536-115">编写良好的应用程序会保证`System.IDisposable.Dispose`时不再需要占用有限的资源的任何对象，立即调用。</span><span class="sxs-lookup"><span data-stu-id="f1536-115">Well-written applications guarantee that `System.IDisposable.Dispose` is called promptly when any object that holds a limited resource is no longer needed.</span></span> <span data-ttu-id="f1536-116">幸运的是，大多数.NET 语言都提供支持，以简化这一操作，F # 也不例外。</span><span class="sxs-lookup"><span data-stu-id="f1536-116">Fortunately, most .NET languages provide support to make this easier, and F# is no exception.</span></span> <span data-ttu-id="f1536-117">存在的两个有用的语言构造，支持的释放模式：`use`绑定和`using`函数。</span><span class="sxs-lookup"><span data-stu-id="f1536-117">There are two useful language constructs that support the dispose pattern: the `use` binding and the `using` function.</span></span>

## <a name="use-binding"></a><span data-ttu-id="f1536-118">使用绑定</span><span class="sxs-lookup"><span data-stu-id="f1536-118">use Binding</span></span>
<span data-ttu-id="f1536-119">`use`关键字具有类似于一个窗体`let`绑定：</span><span class="sxs-lookup"><span data-stu-id="f1536-119">The `use` keyword has a form that resembles that of the `let` binding:</span></span>

<span data-ttu-id="f1536-120">使用*值* = *表达式*</span><span class="sxs-lookup"><span data-stu-id="f1536-120">use *value* = *expression*</span></span>

<span data-ttu-id="f1536-121">它提供与相同的功能`let`绑定，但添加对的调用`Dispose`上时的值超出范围的值。</span><span class="sxs-lookup"><span data-stu-id="f1536-121">It provides the same functionality as a `let` binding but adds a call to `Dispose` on the value when the value goes out of scope.</span></span> <span data-ttu-id="f1536-122">请注意，编译器将插入 null 值，检查，因此，如果值`null`，调用`Dispose`不尝试。</span><span class="sxs-lookup"><span data-stu-id="f1536-122">Note that the compiler inserts a null check on the value, so that if the value is `null`, the call to `Dispose` is not attempted.</span></span>

<span data-ttu-id="f1536-123">下面的示例演示如何通过使用自动关闭文件`use`关键字。</span><span class="sxs-lookup"><span data-stu-id="f1536-123">The following example shows how to close a file automatically by using the `use` keyword.</span></span>

[!code-fsharp[Main](../../../samples/snippets/fsharp/lang-ref-2/snippet6301.fs)]

>[!NOTE]
<span data-ttu-id="f1536-124">你可以使用`use`在计算表达式中，在这种情况下的自定义的版本`use`使用表达式。</span><span class="sxs-lookup"><span data-stu-id="f1536-124">You can use `use` in computation expressions, in which case a customized version of the `use` expression is used.</span></span> <span data-ttu-id="f1536-125">有关详细信息，请参阅[序列](sequences.md)，[异步工作流](asynchronous-workflows.md)，和[计算表达式](computation-expressions.md)。</span><span class="sxs-lookup"><span data-stu-id="f1536-125">For more information, see [Sequences](sequences.md), [Asynchronous Workflows](asynchronous-workflows.md), and [Computation Expressions](computation-expressions.md).</span></span>


## <a name="using-function"></a><span data-ttu-id="f1536-126">使用函数</span><span class="sxs-lookup"><span data-stu-id="f1536-126">using Function</span></span>
<span data-ttu-id="f1536-127">`using`函数具有以下形式：</span><span class="sxs-lookup"><span data-stu-id="f1536-127">The `using` function has the following form:</span></span>

<span data-ttu-id="f1536-128">`using`(*expression1*)*函数或 lambda*</span><span class="sxs-lookup"><span data-stu-id="f1536-128">`using` (*expression1*) *function-or-lambda*</span></span>

<span data-ttu-id="f1536-129">在`using`表达式， *expression1*创建必须释放的对象。</span><span class="sxs-lookup"><span data-stu-id="f1536-129">In a `using` expression, *expression1* creates the object that must be disposed.</span></span> <span data-ttu-id="f1536-130">结果*expression1* （必须释放的对象） 将成为自变量，*值*到*函数或 lambda*，它是需要单个任一函数剩余的值匹配的类型自变量由*expression1*，或需要该类型的自变量的 lambda 表达式。</span><span class="sxs-lookup"><span data-stu-id="f1536-130">The result of *expression1* (the object that must be disposed) becomes an argument, *value*, to *function-or-lambda*, which is either a function that expects a single remaining argument of a type that matches the value produced by *expression1*, or a lambda expression that expects an argument of that type.</span></span> <span data-ttu-id="f1536-131">在执行函数的末尾，则运行时调用`Dispose`并释放资源 (除非的值是`null`，在这种情况下不尝试对释放的调用)。</span><span class="sxs-lookup"><span data-stu-id="f1536-131">At the end of the execution of the function, the runtime calls `Dispose` and frees the resources (unless the value is `null`, in which case the call to Dispose is not attempted).</span></span>

<span data-ttu-id="f1536-132">下面的示例演示`using`使用 lambda 表达式的表达式。</span><span class="sxs-lookup"><span data-stu-id="f1536-132">The following example demonstrates the `using` expression with a lambda expression.</span></span>

[!code-fsharp[Main](../../../samples/snippets/fsharp/lang-ref-2/snippet6302.fs)]

<span data-ttu-id="f1536-133">下面的示例说明`using`使用函数的表达式。</span><span class="sxs-lookup"><span data-stu-id="f1536-133">The next example shows the `using` expression with a function.</span></span>

[!code-fsharp[Main](../../../samples/snippets/fsharp/lang-ref-2/snippet6303.fs)]

<span data-ttu-id="f1536-134">请注意，该函数可以是具有已应用某些参数的函数。</span><span class="sxs-lookup"><span data-stu-id="f1536-134">Note that the function could be a function that has some arguments applied already.</span></span> <span data-ttu-id="f1536-135">下面的代码示例说明这一点。</span><span class="sxs-lookup"><span data-stu-id="f1536-135">The following code example demonstrates this.</span></span> <span data-ttu-id="f1536-136">会创建一个文件包含由字符串`XYZ`。</span><span class="sxs-lookup"><span data-stu-id="f1536-136">It creates a file that contains the string `XYZ`.</span></span>

[!code-fsharp[Main](../../../samples/snippets/fsharp/lang-ref-2/snippet6304.fs)]

<span data-ttu-id="f1536-137">`using`函数和`use`绑定是几乎等效方法完成同样的操作。</span><span class="sxs-lookup"><span data-stu-id="f1536-137">The `using` function and the `use` binding are nearly equivalent ways to accomplish the same thing.</span></span> <span data-ttu-id="f1536-138">`using`关键字提供了更好地控制何时`Dispose`调用。</span><span class="sxs-lookup"><span data-stu-id="f1536-138">The `using` keyword provides more control over when `Dispose` is called.</span></span> <span data-ttu-id="f1536-139">当你使用`using`，`Dispose`在使用时调用的函数或 lambda 表达式，则末尾`use`关键字，`Dispose`称为包含的代码块的末尾。</span><span class="sxs-lookup"><span data-stu-id="f1536-139">When you use `using`, `Dispose` is called at the end of the function or lambda expression; when you use the `use` keyword, `Dispose` is called at the end of the containing code block.</span></span> <span data-ttu-id="f1536-140">一般情况下，您应该会希望使用`use`而不是`using`函数。</span><span class="sxs-lookup"><span data-stu-id="f1536-140">In general, you should prefer to use `use` instead of the `using` function.</span></span>


## <a name="see-also"></a><span data-ttu-id="f1536-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f1536-141">See Also</span></span>
[<span data-ttu-id="f1536-142">F# 语言参考</span><span class="sxs-lookup"><span data-stu-id="f1536-142">F# Language Reference</span></span>](index.md)
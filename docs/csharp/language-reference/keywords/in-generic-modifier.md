---
title: in（泛型修饰符）（C# 参考）
ms.date: 07/20/2015
helpviewer_keywords:
- contravariance, in keyword [C#]
- in keyword [C#]
ms.openlocfilehash: 003ce26fe9ba315eefc748a406754026231004b0
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
ms.locfileid: "33266999"
---
# <a name="in-generic-modifier-c-reference"></a>in（泛型修饰符）（C# 参考）

对于泛型类型参数，`in` 关键字可指定类型参数是逆变的。 可以在泛型接口和委托中使用 `in` 关键字。  
  
 逆变使你使用的类型可以比泛型参数指定的类型派生程度更小。 这样可以隐式转换实现变体接口的类以及隐式转换委托类型。 引用类型支持泛型类型参数中的协变和逆变，但值类型不支持它们。  
  
 仅在类型定义方法参数的类型，而不是方法返回类型时，类型可以在泛型接口或委托中声明为逆变。 `In`、`ref` 和 `out` 参数必须是固定的，这意味着它们既不为协变又不为逆变。
  
 具有逆变类型参数的接口使其方法接受的参数的类型可以比接口类型参数指定的类型派生程度更小。 例如，在 <xref:System.Collections.Generic.IComparer%601> 接口中，类型 T 是逆变的，可以将 `IComparer<Person>` 类型的对象分配给 `IComparer<Employee>` 类型的对象，而无需使用任何特殊转换方法（如果 `Employee` 继承 `Person`）。  
  
 可以向逆变委托分配相同类型的其他委托，不过要使用派生程度更小的泛型类型参数。  
  
 有关详细信息，请参阅[协变和逆变](../../programming-guide/concepts/covariance-contravariance/index.md)。  
  
## <a name="contravariant-generic-interface"></a>逆变泛型接口   

 下面的示例演示如何声明、扩展和实现逆变泛型接口。 它还演示如何对实现此接口的类使用隐式转换。  
  
 [!code-csharp[csVarianceKeywords#1](../../../csharp/language-reference/keywords/codesnippet/CSharp/in-generic-modifier_1.cs)]  
  
## <a name="contravariant-generic-delegate"></a>逆变泛型委托  

 以下示例演示如何声明、实例化和调用逆变泛型委托。 它还演示如何隐式转换委托类型。  
  
 [!code-csharp[csVarianceKeywords#2](../../../csharp/language-reference/keywords/codesnippet/CSharp/in-generic-modifier_2.cs)]  
  
## <a name="c-language-specification"></a>C# 语言规范  
 [!INCLUDE[CSharplangspec](~/includes/csharplangspec-md.md)]  
  
## <a name="see-also"></a>请参阅  
 [out](../../../csharp/language-reference/keywords/out-generic-modifier.md)  
 [协变和逆变](../../programming-guide/concepts/covariance-contravariance/index.md)  
 [修饰符](../../../csharp/language-reference/keywords/modifiers.md)  

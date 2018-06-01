### <a name="linq-to-ef-join-throws-argumentoutofrangeexception"></a><span data-ttu-id="45163-101">Linq to EF Join 会引发 ArgumentOutOfRangeException</span><span class="sxs-lookup"><span data-stu-id="45163-101">Linq to EF Join throws ArgumentOutOfRangeException</span></span>

|   |   |
|---|---|
|<span data-ttu-id="45163-102">详细信息</span><span class="sxs-lookup"><span data-stu-id="45163-102">Details</span></span>|<span data-ttu-id="45163-103">在实体框架实体上调用“Join”的 Linq 查询或枚举会在 .NET Framework 4.5 中导致 <xref:System.ArgumentOutOfRangeException?displayProperty=name> 异常</span><span class="sxs-lookup"><span data-stu-id="45163-103">Linq queries or enumerables that call &#39;Join&#39; on Entity Framework entities can cause an <xref:System.ArgumentOutOfRangeException?displayProperty=name>  in .NET Framework 4.5</span></span>|
|<span data-ttu-id="45163-104">建议</span><span class="sxs-lookup"><span data-stu-id="45163-104">Suggestion</span></span>|<span data-ttu-id="45163-105">此问题已在服务更新中得到解决。</span><span class="sxs-lookup"><span data-stu-id="45163-105">This issue was fixed in a servicing update.</span></span> <span data-ttu-id="45163-106">请更新 .NET Framework 4.5，或升级到 .NET Framework 4.5.1 或更高版本，以解决此问题。</span><span class="sxs-lookup"><span data-stu-id="45163-106">Please update the .NET Framework 4.5, or upgrade to .NET Framework 4.5.1 or later, to fix this issue.</span></span>|
|<span data-ttu-id="45163-107">范围</span><span class="sxs-lookup"><span data-stu-id="45163-107">Scope</span></span>|<span data-ttu-id="45163-108">次要</span><span class="sxs-lookup"><span data-stu-id="45163-108">Minor</span></span>|
|<span data-ttu-id="45163-109">版本</span><span class="sxs-lookup"><span data-stu-id="45163-109">Version</span></span>|<span data-ttu-id="45163-110">4.5</span><span class="sxs-lookup"><span data-stu-id="45163-110">4.5</span></span>|
|<span data-ttu-id="45163-111">类型</span><span class="sxs-lookup"><span data-stu-id="45163-111">Type</span></span>|<span data-ttu-id="45163-112">运行时</span><span class="sxs-lookup"><span data-stu-id="45163-112">Runtime</span></span>|
|<span data-ttu-id="45163-113">受影响的 API</span><span class="sxs-lookup"><span data-stu-id="45163-113">Affected APIs</span></span>|<ul><li><xref:System.Linq.Enumerable.Join%60%604(System.Collections.Generic.IEnumerable%7B%60%600%7D%2CSystem.Collections.Generic.IEnumerable%7B%60%601%7D%2CSystem.Func%7B%60%600%2C%60%602%7D%2CSystem.Func%7B%60%601%2C%60%602%7D%2CSystem.Func%7B%60%600%2C%60%601%2C%60%603%7D)?displayProperty=nameWithType></li><li><xref:System.Linq.Enumerable.Join%60%604(System.Collections.Generic.IEnumerable%7B%60%600%7D%2CSystem.Collections.Generic.IEnumerable%7B%60%601%7D%2CSystem.Func%7B%60%600%2C%60%602%7D%2CSystem.Func%7B%60%601%2C%60%602%7D%2CSystem.Func%7B%60%600%2C%60%601%2C%60%603%7D%2CSystem.Collections.Generic.IEqualityComparer%7B%60%602%7D)?displayProperty=nameWithType></li><li><xref:System.Linq.ParallelEnumerable.Join%60%604(System.Linq.ParallelQuery%7B%60%600%7D%2CSystem.Collections.Generic.IEnumerable%7B%60%601%7D%2CSystem.Func%7B%60%600%2C%60%602%7D%2CSystem.Func%7B%60%601%2C%60%602%7D%2CSystem.Func%7B%60%600%2C%60%601%2C%60%603%7D)?displayProperty=nameWithType></li><li><xref:System.Linq.ParallelEnumerable.Join%60%604(System.Linq.ParallelQuery%7B%60%600%7D%2CSystem.Collections.Generic.IEnumerable%7B%60%601%7D%2CSystem.Func%7B%60%600%2C%60%602%7D%2CSystem.Func%7B%60%601%2C%60%602%7D%2CSystem.Func%7B%60%600%2C%60%601%2C%60%603%7D%2CSystem.Collections.Generic.IEqualityComparer%7B%60%602%7D)?displayProperty=nameWithType></li><li><xref:System.Linq.ParallelEnumerable.Join%60%604(System.Linq.ParallelQuery%7B%60%600%7D%2CSystem.Linq.ParallelQuery%7B%60%601%7D%2CSystem.Func%7B%60%600%2C%60%602%7D%2CSystem.Func%7B%60%601%2C%60%602%7D%2CSystem.Func%7B%60%600%2C%60%601%2C%60%603%7D)?displayProperty=nameWithType></li><li><xref:System.Linq.ParallelEnumerable.Join%60%604(System.Linq.ParallelQuery%7B%60%600%7D%2CSystem.Linq.ParallelQuery%7B%60%601%7D%2CSystem.Func%7B%60%600%2C%60%602%7D%2CSystem.Func%7B%60%601%2C%60%602%7D%2CSystem.Func%7B%60%600%2C%60%601%2C%60%603%7D%2CSystem.Collections.Generic.IEqualityComparer%7B%60%602%7D)?displayProperty=nameWithType></li><li><xref:System.Linq.Queryable.Join%60%604(System.Linq.IQueryable%7B%60%600%7D%2CSystem.Collections.Generic.IEnumerable%7B%60%601%7D%2CSystem.Linq.Expressions.Expression%7BSystem.Func%7B%60%600%2C%60%602%7D%7D%2CSystem.Linq.Expressions.Expression%7BSystem.Func%7B%60%601%2C%60%602%7D%7D%2CSystem.Linq.Expressions.Expression%7BSystem.Func%7B%60%600%2C%60%601%2C%60%603%7D%7D)?displayProperty=nameWithType></li><li><xref:System.Linq.Queryable.Join%60%604(System.Linq.IQueryable%7B%60%600%7D%2CSystem.Collections.Generic.IEnumerable%7B%60%601%7D%2CSystem.Linq.Expressions.Expression%7BSystem.Func%7B%60%600%2C%60%602%7D%7D%2CSystem.Linq.Expressions.Expression%7BSystem.Func%7B%60%601%2C%60%602%7D%7D%2CSystem.Linq.Expressions.Expression%7BSystem.Func%7B%60%600%2C%60%601%2C%60%603%7D%7D%2CSystem.Collections.Generic.IEqualityComparer%7B%60%602%7D)?displayProperty=nameWithType></li></ul>|

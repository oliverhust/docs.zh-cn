---
title: Order By 子句 (Visual Basic)
ms.date: 07/20/2015
f1_keywords:
- vb.QueryOrderBy
- vb.QueryAscending
- vb.QueryDescending
helpviewer_keywords:
- queries [Visual Basic], Order By
- Order By clause [Visual Basic]
- Order By statement [Visual Basic]
ms.assetid: fa911282-6b81-44c7-acfa-46b5bb93df75
ms.openlocfilehash: 7c60156ee81618530b42d5f61dbcac6f59c4f675
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
ms.locfileid: "33604115"
---
# <a name="order-by-clause-visual-basic"></a>Order By 子句 (Visual Basic)
指定查询结果的排序顺序。  
  
## <a name="syntax"></a>语法  
  
```  
Order By orderExp1 [ Ascending | Descending ] [, orderExp2 [...] ]  
```  
  
## <a name="parts"></a>部件  
 `orderExp1`  
 必须的。 一个或多个当前的查询结果中标识字段进行排序的返回的值的方式。 字段名称必须用逗号 （，） 分隔。 你可以标识每个字段，如按升序或降序使用`Ascending`或`Descending`关键字。 如果没有`Ascending`或`Descending`指定关键字，默认的排序顺序为升序。 排序顺序字段优先从左到右。  
  
## <a name="remarks"></a>备注  
 你可以使用`Order By`子句的查询结果进行排序。 `Order By`子句可以仅对结果进行排序基于当前作用域的范围变量。 例如，`Select`子句引入该作用域在查询表达式中使用新的迭代变量的新作用域。 之前定义的范围变量`Select`在查询中的子句之后不可`Select`子句。 因此，如果你想要按字段不是位于你结果进行排序`Select`子句中，你必须放置`Order By`子句之前`Select`子句。 一个你将需要执行此操作的示例是当你想要对你通过不作为结果的一部分返回的字段的查询进行排序。  
  
 升序和降序顺序字段的实现决定<xref:System.IComparable>字段的数据类型的接口。 如果数据类型不实现<xref:System.IComparable>接口，排序顺序将被忽略。  
  
## <a name="example"></a>示例  
 下面的查询表达式使用`From`子句来声明范围变量`book`为`books`集合。 `Order By`子句按价格按升序 （默认值） 对查询结果进行排序。 按标题以升序排序相同价格的书籍。 `Select`子句选择`Title`和`Price`用作由查询返回的值的属性。  
  
 [!code-vb[VbSimpleQuerySamples#24](../../../visual-basic/language-reference/queries/codesnippet/VisualBasic/order-by-clause_1.vb)]  
  
## <a name="example"></a>示例  
 下面的查询表达式使用`Order By`子句对查询结果按价格按降序进行排序。 按标题以升序排序相同价格的书籍。  
  
 [!code-vb[VbSimpleQuerySamples#25](../../../visual-basic/language-reference/queries/codesnippet/VisualBasic/order-by-clause_2.vb)]  
  
## <a name="example"></a>示例  
 下面的查询表达式使用`Select`子句来选择书名、 价格、 发布日期，和创作。 然后填充`Title`， `Price`， `PublishDate`，和`Author`为新作用域的范围变量的字段。 `Order By`子句顺序由作者姓名、 书名和价格的新范围变量。 每个列进行排序 （升序） 的默认顺序。  
  
 [!code-vb[VbSimpleQuerySamples#26](../../../visual-basic/language-reference/queries/codesnippet/VisualBasic/order-by-clause_3.vb)]  
  
## <a name="see-also"></a>请参阅  
 [Visual Basic 中的 LINQ 简介](../../../visual-basic/programming-guide/language-features/linq/introduction-to-linq.md)  
 [查询](../../../visual-basic/language-reference/queries/queries.md)  
 [Select 子句](../../../visual-basic/language-reference/queries/select-clause.md)  
 [From 子句](../../../visual-basic/language-reference/queries/from-clause.md)

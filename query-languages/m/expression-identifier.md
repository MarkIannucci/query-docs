---
title: "Expression.Identifier | Microsoft Docs"
ms.date: 4/16/2018
ms.prod: power-query
ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Expression.Identifier

  
## About  
Returns a text value that can be used as an identifier from a text value.  
  
```  
Expression.Identifier(name as text) as text  
```  
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|name|The text to identify.|  
  
## Examples  
  
```  
Expression.Identifier("foo") equals "foo"  
```  
  
```  
Expression.Identifier("10 lbs") equals "#""10 lbs"""  
```  
  
```  
Expression.Identifier("try") equals "#""try"""  
```  
  
```  
Expression.Identifier("") equals "#"""""  
```  
  
```  
Expression.Identifier(null) equals Error  
```  
  
## Example of combined use  
  
```  
Expression.Evaluate(  
// "let x = 1 in x"  
"let " &  
Expression.Identifier("x") & " = " & Expression.Constant(1) &  
" in " &  
Expression.Identifier("x")  
) equals 1  
```  
---
title: "EARLIEST Function (DAX) | Microsoft Docs"
ms.prod: dax
ms.date: 4/13/2018
ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# EARLIEST Function (DAX)
Returns the current value of the specified column in an outer evaluation pass of the specified column.  
  
## Syntax  
  
```  
EARLIEST(<column>)  
```  
  
#### Parameters  
  
|Term|Definition|  
|--------|--------------|  
|**column**|A reference to a column.|  
  
## Property Value/Return Value  
A column with filters removed.  
  
## Remarks  
The EARLIEST function is similar to EARLIER, but lets you specify one additional level of recursion.  
  
## Example  
The current sample data does not support this scenario.  
  
```  
=EARLIEST(<column>)  
```  
  
## See Also  
[EARLIER Function &#40;DAX&#41;](earlier-function-dax.md)  
[Filter Functions &#40;DAX&#41;](filter-functions-dax.md)  
  
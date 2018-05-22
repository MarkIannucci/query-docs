---
title: "Type.ClosedRecord | Microsoft Docs"
ms.date: 4/16/2018
ms.prod: power-query
ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Type.ClosedRecord

  
## About  
The given type must be a record type returns a closed version of the given record type (or the same type, if it is already closed)  
  
```  
Type.ClosedRecord(#"type" as type) as type  
```  
  
## Example  
  
```  
Type.ClosedRecord( type [ A = number,…] ) equals type [A=number]  
```  
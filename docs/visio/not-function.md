---
title: "NOT Function"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251469
 
ms.localizationpriority: medium
ms.assetid: 65873b32-2406-7c33-8e68-802461f467b2
description: "Returns TRUE (1) if logicalexpression is FALSE. Otherwise, it returns FALSE (0)."
---

# NOT Function

Returns TRUE (1) if  _logicalexpression_ is FALSE. Otherwise, it returns FALSE (0). 
  
## Syntax

NOT(** *logicalexpression* ** ) 
  
### Parameters

|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _logicalexpression_ <br/> |Required  <br/> |**String** <br/> |The logical expression to evaluate. |
   
### Return value

Boolean
  
## Example

NOT(Height \> 0.75 in) 
  
Returns 1 if Height is less than or equal to 0.75 inches. Returns 0 if Height is greater than 0.75 inches. 
  


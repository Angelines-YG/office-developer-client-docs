---
title: "SMAPIFormInfoArray"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MAPI.SMAPIFormInfoArray
api_type:
- COM
ms.assetid: f5eeb75d-debb-4ac1-b239-e8e852460ce0
description: "Contains an array of pointers to form information objects for Outlook 2013 and Outlook 2016."
---

# SMAPIFormInfoArray

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains an array of pointers to form information objects. 
  
|Property |Value |
|:-----|:-----|
|Header file:  <br/> |Mapiform.h  <br/> |
|Related macro:  <br/> |[CbMAPIFormInfoArray](cbmapiforminfoarray.md) <br/> |
   
```cpp
typedef struct
{
  ULONG cForms;
  LPMAPIFORMINFO aFormInfo[MAPI_DIM];
} SMAPIFormInfoArray, FAR * LPSMAPIFORMINFOARRAY;

```

## Members

 **cForms**
  
> Count of pointers in the array pointed to by the **aFormInfo** member. 
    
 **aFormInfo**
  
> Pointer to an array of pointers to form information objects.
    
## Remarks

The **SMAPIFormInfoArray** structure is passed as a parameter in the following methods: 
  
- [IMAPIFormMgr::ResolveMultipleMessageClasses](imapiformmgr-resolvemultiplemessageclasses.md)
    
- [IMAPIFormMgr::CalcFormPropSet](imapiformmgr-calcformpropset.md)
    
- [IMAPIFormMgr::SelectMultipleForms](imapiformmgr-selectmultipleforms.md)
    
- [IMAPIFormContainer::ResolveMultipleMessageClasses](imapiformcontainer-resolvemultiplemessageclasses.md)
    
## See also



[MAPI Structures](mapi-structures.md)


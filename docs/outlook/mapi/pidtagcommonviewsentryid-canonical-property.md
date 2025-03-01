---
title: "PidTagCommonViewsEntryId Canonical Property"
 
 
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PidTagCommonViewsEntryId
api_type:
- HeaderDef
ms.assetid: cd9e6a46-2112-4663-891e-5e57b22c0950
description: "Contains the entry identifier of the predefined common view folder. The common view folder contains a predefined set of standard view specifiers."
---

# PidTagCommonViewsEntryId Canonical Property

  
  
**Applies to**: Outlook 2013 | Outlook 2016 
  
Contains the entry identifier of the predefined common view folder. 
  
|Property |Value |
|:-----|:-----|
|Associated properties:  <br/> |PR_COMMON_VIEWS_ENTRYID  <br/> |
|Identifier:  <br/> |0x35E6  <br/> |
|Data type:  <br/> |PT_BINARY  <br/> |
|Area:  <br/> |Outlook application  <br/> |
   
## Remarks

The common view folder contains a predefined set of standard view specifiers, while the view folder contains specifiers defined by a messaging user. These folders, which are not visible in the interpersonal message (IPM) hierarchy, can hold many view specifiers, each one stored as a message. A client application can choose to merge the two sets of specifiers and make them both available. 
  
For more information on views, see [View Folders](mapi-view-folders.md).
  
## Related resources

### Header files

Mapidefs.h
  
> Provides data type definitions.
    
Mapitags.h
  
> Contains definitions of properties listed as alternate names.
    
## See also



[PidTagDefaultViewEntryId Canonical Property](pidtagdefaultviewentryid-canonical-property.md)
  
[PidTagViewsEntryId Canonical Property](pidtagviewsentryid-canonical-property.md)


[MAPI Properties](mapi-properties.md)
  
[MAPI Canonical Properties](mapi-canonical-properties.md)
  
[Mapping Canonical Property Names to MAPI Names](mapping-canonical-property-names-to-mapi-names.md)
  
[Mapping MAPI Names to Canonical Property Names](mapping-mapi-names-to-canonical-property-names.md)


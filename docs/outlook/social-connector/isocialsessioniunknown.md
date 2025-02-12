---
title: "ISocialSession  IUnknown"
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0fe423d7-b044-479b-89ad-c39620eedd65
description: "Represents a connection to a social network site."
---

# ISocialSession : IUnknown

Represents a connection to a social network site.
  
## Members

The following table shows the members that are available on the **ISocialSession** interface. 
  
|**Name**|**Member type**|**Description**|
|:-----|:-----|:-----|
|[FindPerson](isocialsession-findperson.md) <br/> |Method  <br/> |Gets a string that represents one or more persons who match the  _userID_ parameter. |
|[FollowPerson](isocialsession-followperson.md) <br/> |Method  <br/> |Adds the person identified by the  _emailAddress_ parameter as a friend for the logged-on user on the social network. |
|[GetActivities](isocialsession-getactivities.md) <br/> |Method  <br/> |This method has been deprecated in Outlook Social Connector (OSC) 1.1. |
|[GetLoggedOnUser](isocialsession-getloggedonuser.md) <br/> |Method  <br/> |Gets an [ISocialProfile](isocialprofileisocialperson.md) interface that represents the logged-on user. |
|[GetLogonUrl](isocialsession-getlogonurl.md) <br/> |Method  <br/> |Gets a string that represents a URL that is used for presenting a browser-based form to the user during web authentication. |
|[GetNetworkIdentifier](isocialsession-getnetworkidentifier.md) <br/> |Method  <br/> |Gets a string that represents a unique social network identifier for a given social network connection. |
|[GetPerson](isocialsession-getperson.md) <br/> |Method  <br/> |Gets an [ISocialPerson](isocialpersoniunknown.md) interface based on the  _userID_ parameter. |
|[LoggedOnUserID](isocialsession-loggedonuserid.md) <br/> |Property  <br/> |Returns a string that represents the social network user ID of the user who is currently logged on. |
|[LoggedOnUserName](isocialsession-loggedonusername.md) <br/> |Property  <br/> |Returns a string that represents the user name that is used when logging on. |
|[Logon](isocialsession-logon.md) <br/> |Method  <br/> |Logs on to the social network site by using the specified user name and password. |
|[LogonWeb](isocialsession-logonweb.md) <br/> |Method  <br/> |Logs on to the social network site by using forms-based authentication. |
|[SiteUrl](isocialsession-siteurl.md) <br/> |Property  <br/> |Sets the social network site URL. |
|[UnFollowPerson](isocialsession-unfollowperson.md) <br/> |Method  <br/> |Removes the person identified by the  _userID_ parameter as a friend on the social network. |
   
## Remarks

An OSC provider must implement this interface to communicate with the OSC.
  
## See also

- [Outlook Social Connector Provider Interfaces](outlook-social-connector-provider-interfaces.md)


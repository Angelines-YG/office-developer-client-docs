---
title: Recordset.Type property (DAO)
TOCTitle: Type Property
ms:assetid: d841b088-50bf-16d9-33e0-2140050e1ac6
ms:mtpsurl: https://msdn.microsoft.com/library/Ff835080(v=office.15)
ms:contentKeyID: 48548030
ms.date: 09/18/2015
mtps_version: v=office.15
ms.localizationpriority: medium
---

# Recordset.Type property (DAO)


**Applies to**: Access 2013, Office 2013

Sets or returns a value that indicates the operational type or data type of an object. Read-only **Integer**.

## Syntax

*expression* .Type

*expression* A variable that represents a **Recordset** object.

## Remarks

For a **Recordset** object, the possible settings and return values are as follows.

<table>
<colgroup>
<col />
<col />
</colgroup>
<thead>
<tr class="header">
<th><p>Constant</p></th>
<th><p>Recordset type</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>dbOpenTable</strong></p></td>
<td><p>Table (Microsoft Access workspaces only)</p></td>
</tr>
<tr class="even">
<td><p><strong>dbOpenDynamic</strong></p></td>
<td><p>Dynamic (ODBCDirect workspaces only)</p>
<p><strong>NOTE</strong>: ODBCDirect workspaces are not supported in Microsoft Access 2013. Use ADO if you want to access external data sources without using the Microsoft Access database engine.</p></td>
</tr>
<tr class="odd">
<td><p><strong>dbOpenDynaset</strong></p></td>
<td><p>Dynaset</p></td>
</tr>
<tr class="even">
<td><p><strong>dbOpenSnapshot</strong></p></td>
<td><p>Snapshot</p></td>
</tr>
<tr class="odd">
<td><p><strong>dbOpenForwardOnly</strong></p></td>
<td><p>Forward-only</p></td>
</tr>
</tbody>
</table>


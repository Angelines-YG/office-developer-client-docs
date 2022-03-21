---
title: RunCode macro action
TOCTitle: RunCode macro action
ms:assetid: cb0625be-4b5d-4927-9b0e-59a6e411b5bb
ms:mtpsurl: https://msdn.microsoft.com/library/Ff834373(v=office.15)
ms:contentKeyID: 48547706
ms.date: 09/18/2015
mtps_version: v=office.15
f1_keywords:
- vbaac10.chm98700
f1_categories:
- Office.Version=v15
ms.localizationpriority: medium
---

# RunCode macro action

**Applies to**: Access 2013, Office 2013

You can use the **RunCode** action to call a Visual Basic for Applications (VBA) Function procedure.

## Setting

The **RunCode** action has the following argument.

<table>
<colgroup>
<col />
<col />
</colgroup>
<thead>
<tr class="header">
<th><p>Action argument</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Function Name</strong></p></td>
<td><p>The name of the VBA Function procedure to call. Enclose any function arguments in parentheses. Enter the function name in the <strong>Function Name</strong> box in the <strong>Action Arguments</strong> section of the Macro Builder pane. This is a required argument.</p><p><strong>NOTE</strong>: In an Access database (.mdb or .accdb), click the <strong>Build</strong> button to use the Expression Builder to select a function for this argument. Click the desired function in the list in the Expression Builder.</p></td>
</tr>
</tbody>
</table>


## Remarks

The user-defined Function procedures are stored in Microsoft Access modules.

You must include parentheses, even if the Function procedure doesn't have any arguments, as in the following example:

`TestFunction()`

Unlike user-defined function names used for event property settings, the function name in the **Function Name** argument doesn't begin with an equal sign (**=**).

Access ignores the return value of the function.

> [!NOTE]
> You can't call a Function procedure from a macro if the function name is the same as the module name.

> [!TIP]
> To run a Sub procedure or event procedure written in Visual Basic, create a Function procedure that calls the Sub procedure or event procedure. Then use the **RunCode** action to run the Function procedure.

If you use the **RunCode** action to call a function, Access looks for the function with the name specified by the **Function Name** argument in the standard modules for the database. However, when this action runs in response to clicking a menu command on a form or report or in response to an event on a form or report, Access first looks for the function in the form's or report's class module and then in the standard modules. Access doesn't search the class modules that appear in the **Modules** area of the Navigation Pane for the function specified by the **Function Name** argument.

This action isn't available in a VBA module. Instead, run the desired Function procedure directly in VBA.


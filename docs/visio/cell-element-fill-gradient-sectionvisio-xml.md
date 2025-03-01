---
title: "Cell element (Fill Gradient Section) (Visio XML)" 
manager: lindalu
ms.date: 03/09/2022
ms.audience: Developer
ms.topic: reference 
ms.localizationpriority: medium
ms.assetid: d085f83a-f77b-9bf9-07dc-4561b83e288c
description: "Cell element contains the color, transparency, and position of a gradient stop for a fill gradient."
---

# Cell element (Fill Gradient Section) (Visio XML)

Contains the color, transparency, and position of a gradient stop for a fill gradient.
  
## Element information

|**Value**|**Description**|
|:-----|:-----|
|**Element type** <br/> |[Cell_Type](cell_type-complextypevisio-xml.md) <br/> |
|**Namespace** <br/> |http://schemas.microsoft.com/office/visio/2012/main  <br/> |
|**Schema file** <br/> |VisioSchema15.xsd  <br/> |
|**Document parts** <br/> |document.xml, master#.xml, page#.xml  <br/> |
   
## Definition

```XML
< xs:element name="Cell" type="Cell_Type" minOccurs="0" maxOccurs="unbounded" >
</xs:element >
```

## Elements and attributes

If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section. 
  
### Parent elements

|**Element**|**Type**|**Description**|
|:-----|:-----|:-----|
|[Row element (FillGradient Section)](row-element-fill-gradient-sectionvisio-xml.md) <br/> |[FillGradientRow_Type](fillgradientrow_type-complextypevisio-xml.md) <br/> |Contains the color, transparency, and position of a gradient stop for a fill gradient. |
   
### Child elements

|**Element**|**Type**|**Description**|
|:-----|:-----|:-----|
|[RefBy](refby-element-cell_type-complextypevisio-xml.md) <br/> |[RefBy_Type](refby_type-complextypevisio-xml.md) <br/> |Specifies a reference to a drawing page. |
   
### Attributes

|**Attribute**|**Type**|**Required**|**Description**|**Possible values**|
|:-----|:-----|:-----|:-----|:-----|
|E  <br/> |xsd:string  <br/> |optional  <br/> |Indicates that the formula evaluates to an error. The value of **E** is the current value (an error message string); the value of the **V** attribute is the last valid value. |An error message string. |
|F  <br/> |xsd:string  <br/> |optional  <br/> | Represents the element's formula. This attribute can contain one of the following strings:  <br/>  '(some formula)' if the formula exists locally  <br/>  `No Formula` if the formula is locally deleted or blocked  <br/>  `Inh` if the formula is inherited. |A formula. |
|N  <br/> |xsd:string  <br/> |required  <br/> |Represents the name of the ShapeSheet cell. |The name of the ShapeSheet cell. See the Remarks section below. |
|U  <br/> |xsd:string  <br/> |optional  <br/> |Represents a unit of measure The default is DL. |The units of the cell. |
|V  <br/> |xsd:string  <br/> |optional  <br/> |Represents the value of the cell. |The value of the ShapeSheet cell. |
   
## Remarks

The **N** attribute of this **Cell** element must be one of a limited set of values that correspond to ShapeSheet cells. Refer to the table below to determine the values of the **N** attribute that are permitted for this **Cell** element. 
  
|**Value**|**Description**|**More information**|
|:-----|:-----|:-----|
|GradientStopColor  <br/> |The color value of the gradient stop. This value can be expressed as the index number of a color in the document palette or by using the **RGB**, **THEMEVAL**, or **HSL** functions. |[Gradient Stop Row (Fill Gradient Section)](gradient-stop-row-fill-gradient-section.md) <br/> |
|GradientStopColorTrans  <br/> |The amount of transparency of the gradient color stop, as a percentage. |[Gradient Stop Row (Fill Gradient Section)](gradient-stop-row-fill-gradient-section.md) <br/> |
|GradientStopPosition  <br/> |The position of the gradient stop along the direction of the line gradient, as a percentage from the point of origin of the gradient to the outer edge of the gradient. |[Gradient Stop Row (Fill Gradient Section)](gradient-stop-row-fill-gradient-section.md) <br/> |  

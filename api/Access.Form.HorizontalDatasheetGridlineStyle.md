---
title: Form.HorizontalDatasheetGridlineStyle property (Access)
keywords: vbaac10.chm13514
f1_keywords:
- vbaac10.chm13514
ms.prod: access
api_name:
- Access.Form.HorizontalDatasheetGridlineStyle
ms.assetid: 31467913-382f-031e-b030-68181a71d5e0
ms.date: 03/12/2019
ms.localizationpriority: medium
---


# Form.HorizontalDatasheetGridlineStyle property (Access)

Returns or sets a **Byte** indicating the line style to use for horizontal gridlines on the specified datasheet. Read/write.


## Syntax

_expression_.**HorizontalDatasheetGridlineStyle**

_expression_ A variable that represents a **[Form](Access.Form.md)** object.


## Remarks

Valid values are between zero and seven. Values greater than seven are ignored; negative values or values above 255 cause an error.

|Value|Description|
|:-----|:-----|
|0|Transparent border|
|1|Solid|
|2|Dashes|
|3|Short dashes|
|4|Dots|
|5|Sparse dots|
|6|Dash-dot|
|7|Dash-dot-dot|

## Example

This example sets the horizontal gridline style on the first open form to dash-dot. The form must be set to Datasheet view for you to see the change.


```vb
Forms(0).HorizontalDatasheetGridlineStyle = 6 

```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
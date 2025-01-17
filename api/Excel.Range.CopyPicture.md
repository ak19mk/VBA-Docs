---
title: Range.CopyPicture method (Excel)
keywords: vbaxl10.chm144106
f1_keywords:
- vbaxl10.chm144106
ms.prod: excel
api_name:
- Excel.Range.CopyPicture
ms.assetid: 0b187b51-7a52-0db3-9d55-9c1e5bc5e49b
ms.date: 01/04/2023
ms.localizationpriority: medium
---


# Range.CopyPicture method (Excel)

Copies the selected object to the Clipboard as a picture. **Variant**.

Range.CopyPicture method (Excel) | Microsoft Learn

https://learn.microsoft.com/en-us/office/vba/api/excel.range.copypicture


## Syntax

_expression_.**CopyPicture** (_Appearance_, _Format_)

_expression_ A variable that represents a **[Range](excel.range(object).md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Appearance_|Optional| **[XlPictureAppearance](Excel.XlPictureAppearance.md)**| Specifies how the picture should be copied.|
| _Format_|Optional| **[XlCopyPictureFormat](Excel.XlCopyPictureFormat.md)**| The format of the picture.|


## Return value

## Example

```python
import win32com.client
import time
xlapp = win32com.client.Dispatch("excel.Application")
xlapp.Visible = 1
xlapp.DisplayAlerts = False
ws = xlapp.ActiveSheet
Range01 = "A1:H2"
xlScreen = 1
xlBitmap = 2
ws.Range(Range01).CopyPicture(xlScreen, xlBitmap)
time.sleep(1)
ws.UsedRange.CopyPicture(xlScreen, xlBitmap)
```

Win + V 查看剪贴板

![](https://github.com/ak19mk/VBA-Docs/blob/main/Language/412341234.png)

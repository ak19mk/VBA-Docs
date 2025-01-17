---
title: NewFile.Remove method (Office)
keywords: vbaof11.chm235002
f1_keywords:
- vbaof11.chm235002
ms.prod: office
api_name:
- Office.NewFile.Remove
ms.assetid: 1954580b-3c8b-3e4b-0884-8d32932fbf58
ms.date: 01/22/2019
ms.localizationpriority: medium
---


# NewFile.Remove method (Office)

Removes an item from the **New Item** task pane. Returns a **Boolean** value to indicate whether the operation was successful.


## Syntax

_expression_.**Remove** (_FileName_, _Section_, _DisplayName_, _Action_)

_expression_ Required. A variable that represents a **[NewFile](Office.NewFile.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _FileName_|Required|**String**|The name of the file reference.|
| _Section_|Optional|**Variant**|The section of the task pane where the file reference exists. Can be any **[msoFileNew](office.msofilenewsection.md)** constant.|
| _DisplayName_|Optional|**Variant**|The display text of the file reference.|
| _Action_|Optional|**Variant**|The action to take when a user clicks the item. Can be any **msoFileNew** constant.|

## Remarks

The arguments supplied to the **Remove** method must match the arguments that were supplied to the **Add** method of the **NewFile** object, or the **Remove** method will fail. 

For example, if the **Action** argument was supplied when the **NewFile** object was added, the same **Action** argument must be supplied to remove the **NewFile** object, or the **Remove** method will fail.


## See also

- [NewFile object members](overview/library-reference/newfile-members-office.md)




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
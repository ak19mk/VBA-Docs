---
title: Attachment.OnEnter property (Access)
keywords: vbaac10.chm13939
f1_keywords:
- vbaac10.chm13939
ms.prod: access
api_name:
- Access.Attachment.OnEnter
ms.assetid: 5aae3814-5fff-2011-c86d-3765f2a3615d
ms.date: 02/07/2019
ms.localizationpriority: medium
---


# Attachment.OnEnter property (Access)

Sets or returns the value of the **On Enter** box in the Properties window of the specified object. Read/write **String**. 


## Syntax

_expression_.**OnEnter**

_expression_ A variable that represents an **[Attachment](Access.Attachment.md)** object.


## Remarks

This property is helpful for programmatically changing the action that Microsoft Access takes when an event is triggered. For example, between event calls you may want to change an expression's parameters, or switch from an event procedure to an expression or macro, depending on the circumstances under which the event was triggered. 

The **[Enter](access.attachment.enter.md)** event occurs before a control actually receives the focus from a control on the same form.

The **OnEnter** value will be one of the following, depending on the selection chosen in the Choose Builder window (accessed by choosing the **Build** button next to the **On Enter** box in the object's Properties window):

- If you choose Expression Builder, the value will be =_expression_, where _expression_ is the expression from the Expression Builder window.
    
- If you choose Macro Builder, the value is the name of the macro. 
    
- If you choose Code Builder, the value will be [Event Procedure]. 
    
If the **On Enter** box is blank, the property value is an empty string.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
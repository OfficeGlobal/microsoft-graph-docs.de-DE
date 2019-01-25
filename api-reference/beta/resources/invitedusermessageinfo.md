---
title: Konfigurieren der Einladungsnachricht
description: Mit dem invitedUserMessageInfo-Objekt können Sie die invitation-Nachricht konfigurieren.
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507782"
---
# <a name="configuring-the-invitation-message"></a>Konfigurieren der Einladungsnachricht

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit dem invitedUserMessageInfo-Objekt können Sie die [invitation](invitation.md)-Nachricht konfigurieren.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|ccRecipients|[Recipients](recipient.md)|Weitere Empfänger, an die die Einladungsnachricht gesendet werden soll. Derzeit wird nur 1 zusätzlicher Empfänger unterstützt.|
|customizedMessageBody|String|Angepasster Nachrichtentext, den Sie senden möchten, wenn Sie nicht die Standardnachricht senden.|
|messageLanguage|Zeichenfolge|Die Sprache, in der Sie die Standardnachricht senden möchten. Wenn customizedMessageBody angegeben ist, wird diese Eigenschaft ignoriert und die Nachricht wird mithilfe von customizedMessageBody gesendet. Das Sprachformat sollte ISO 639 sein. Der Standardwert ist en-US.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitedusermessageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

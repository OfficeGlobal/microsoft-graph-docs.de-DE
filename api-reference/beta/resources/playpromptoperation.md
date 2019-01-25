---
title: Ressourcentyp playPromptOperation
description: Abrufen des Ergebnisses der Aktion PlayPrompt PlayPrompt-Vorgang.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515202"
---
# <a name="playpromptoperation-resource-type"></a>Ressourcentyp playPromptOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abrufen des Ergebnisses der Aktion PlayPrompt PlayPrompt-Vorgang.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ                        | Beschreibung|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| ClientContext       | String                      | Der Clientkontext.                                                                |
| completionReason    | String                      | Mögliche Werte sind: `unknown`, `completedSuccessfully` und `mediaOperationCanceled`. |
| createdDateTime     | DateTimeOffset              | Die Startzeit des Vorgangs.                                                   |
| id                  | String                      | Schreibgeschützt.                                                                         |
| lastActionDateTime  | DateTimeOffset              | Der Zeitpunkt der letzten Aktion des Vorgangs.                                      |
| resultInfo          | [resultInfo](resultInfo.md) | Informationen zu den Ergebnissen. Schreibgeschützt. Server generiert wurde.                               |
| status              | String                      | Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.               |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/playpromptoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

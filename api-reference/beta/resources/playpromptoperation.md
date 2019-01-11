---
title: Ressourcentyp playPromptOperation
description: Abrufen des Ergebnisses der Aktion PlayPrompt PlayPrompt-Vorgang.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: bc18b8f64dedd3fa4d758778bbee37c6bcfd46c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814378"
---
# <a name="playpromptoperation-resource-type"></a>Ressourcentyp playPromptOperation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Abrufen des Ergebnisses der Aktion PlayPrompt PlayPrompt-Vorgang.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ                        | Beschreibung|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | Der Clientkontext.                                                                |
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
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

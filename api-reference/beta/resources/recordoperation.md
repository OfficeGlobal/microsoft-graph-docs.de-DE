---
title: Ressourcentyp recordOperation
description: Der RecordOperation-Typ
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2fdf8b6f1f00429e676d778c0095d4554fff4a18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948744"
---
# <a name="recordoperation-resource-type"></a>Ressourcentyp recordOperation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der RecordOperation-Typ

## <a name="properties"></a>Eigenschaften

| Eigenschaft                       | Typ                        | Beschreibung                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | Zeichenfolge                      | Der Clientkontext.                                                                                                                               |
| completionReason               | Zeichenfolge                      | Mögliche Werte: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`. |
| createdDateTime                | DateTimeOffset              | Die Uhrzeit der Erstellung die Aufzeichnung.                                                                                                          |
| id                             | Zeichenfolge                      | Die Id des Server-Vorgang. Schreibgeschützt. Server generiert wurde.                                                                                             |
| lastActionDateTime             | DateTimeOffset              | Der Zeitpunkt der letzten Aktion des Vorgangs.                                                                                                     |
| recordResourceAccessToken      | Zeichenfolge                      | Das Zugriffstoken zum Abrufen der aufzeichnungs erforderlich sind.                                                                                              |
| recordResourceLocation         | Zeichenfolge                      | Der Speicherort, in dem die Aufzeichnung gespeichert ist.                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | Informationen zu den Ergebnissen.  Schreibgeschützt. Server generiert wurde.                                                                                             |
| status                         | String                      | Mögliche Werte: `notStarted`, `running`, `completed`, `failed`. Schreibgeschützt. Server generiert wurde.                                                 |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Beispiel

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

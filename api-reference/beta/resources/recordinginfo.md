---
title: Ressourcentyp recordingInfo
description: Aufzeichnung von Informationen für einen Teilnehmer.
author: VinodRavichandran
ms.openlocfilehash: 709edcc6d473ce610cbba7f628e4ebc5057b779c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380303"
---
# <a name="recordinginfo-resource-type"></a>Ressourcentyp recordingInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aufzeichnung von Informationen für einen Teilnehmer.

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ    | Beschreibung|
|:---------------|:--------|:----------|
| initiatedBy | [participantInfo](participantinfo.md) | Der Teilnehmer, der die Aufzeichnung initiiert hat. |
| status | Zeichenfolge | Mögliche Werte sind: `recordingCapable`, `notRecording` und `startedRecording`. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

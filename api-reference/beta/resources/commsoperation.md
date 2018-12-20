---
title: Ressourcentyp commsOperation
description: Der Status der bestimmte langer Vorgänge.
author: VinodRavichandran
ms.openlocfilehash: 09d3f81e8f6307850d94cfab43f98426dae47a5f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380352"
---
# <a name="commsoperation-resource-type"></a>Ressourcentyp commsOperation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Status der bestimmte langer Vorgänge.

## <a name="methods"></a>Methoden
Keine

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ                        | Beschreibung                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | Zeichenfolge                      | Der Clientkontext.                                                             |
| createdDateTime    | DateTimeOffset              | Die Startzeit des Vorgangs.                                                |
| id                 | Zeichenfolge                      | Die Vorgangs-ID. Schreibgeschützt. Server generiert wurde.                                  |
| lastActionDateTime | DateTimeOffset              | Der Zeitpunkt der letzten Aktion des Vorgangs.                                   |
| resultInfo         | [resultInfo](resultinfo.md) | Informationen zu den Ergebnissen. Schreibgeschützt. Server generiert wurde.                            |
| status             | String                      | Mögliche Werte: `notStarted`, `running`, `completed`, `failed`. Schreibgeschützt. |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Beispiel

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "#microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

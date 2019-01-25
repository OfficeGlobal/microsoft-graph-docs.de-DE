---
title: Vorgang Ressourcentyp
description: Der Status der ein zeitintensiver Vorgang.
localization_priority: Normal
ms.openlocfilehash: 3ad9848387dab2de928f7ace2fa4b905720be615
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520186"
---
# <a name="operation-resource-type"></a>Vorgang Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der Status der ein zeitintensiver Vorgang.

## <a name="methods"></a>Methoden

Keine

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ            | Beschreibung                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| createdDateTime    | DateTimeOffset  | Die Startzeit des Vorgangs.                                                |
| id                 | String          | Die Vorgangs-ID. Schreibgeschützt. Server generiert wurde.                                  |
| lastActionDateTime | DateTimeOffset  | Der Zeitpunkt der letzten Aktion des Vorgangs.                                   |
| status             | String          | Mögliche Werte: `notStarted`, `running`, `completed`, `failed`. Schreibgeschützt. |

## <a name="relationships"></a>Beziehungen

Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Beispiel

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

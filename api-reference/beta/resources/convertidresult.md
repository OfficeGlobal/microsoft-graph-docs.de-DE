---
title: Ressourcentyp convertIdResult
description: Das Ergebnis einer ID formatkonvertierung, die von der Funktion TranslateExchangeIds durchgeführt.
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516525"
---
# <a name="convertidresult-resource-type"></a>Ressourcentyp convertIdResult

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Das Ergebnis einer ID formatkonvertierung, die von der Funktion [TranslateExchangeIds](../api/user-translateexchangeids.md) durchgeführt.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
| SourceId | String | Der Bezeichner, der konvertiert wurde. Dieser Wert ist der ursprüngliche, nicht konvertierten Bezeichner. |
| targetId | String | Der Bezeichner konvertierte. Dieser Wert ist nicht vorhanden, wenn die Konvertierung fehlgeschlagen ist. |
| errorDetails | [Allgemeiner Fehler](genericerror.md) | Ein Error-Objekt zurück, der den Grund für die Konvertierungsfehler angibt. Dieser Wert ist nicht vorhanden, wenn die Konvertierung erfolgreich war. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

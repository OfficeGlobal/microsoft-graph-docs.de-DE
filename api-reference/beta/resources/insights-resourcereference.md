---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8cc7e686aebd531a25b6c1637fcf99338df09396
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572297"
---
# <a name="resourcereference-resource-type"></a>Ressourcentyp resourceReference

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Komplexer Typ mit Eigenschaften des [Insights](insights.md).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ      | Beschreibung  |
| ------------- |-----------| -------------|
| webUrl        | String    | Eine URL, die auf das verwiesene Element führende. |
| id            | String    | Eindeutiger Bezeichner des Elements.           |
| type          | String    | Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

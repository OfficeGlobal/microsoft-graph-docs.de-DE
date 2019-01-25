---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: c50f90787627732843e152a37a469c03340aa370
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511072"
---
# <a name="searchresult-resource-type"></a>SearchResult-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **SearchResult**-Ressource gibt an, dass ein Element die Antwort auf eine Suchanfrage ist.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "onClickTelemtryUrl" ],
  "@odata.type": "microsoft.graph.searchResult"
}-->

```json
{
  "onClickTelemetryUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ   | Beschreibung
|:--------------------|:-------|:----------------------------------------------
| onClickTelemetryUrl | String | Ein Rückruf-URL, die zum Erfassen von Telemetrieinformationen verwendet werden kann. Die Anwendung sollte ein GET für diese URL ausgeben, wenn der Benutzer mit diesem Element zur Verbesserung der Qualität der Ergebnisse interagiert.

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!--
{
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult",
  "suppressions": [
    "Error: /api-reference/beta/resources/searchresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

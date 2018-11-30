---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 7e6bd6e6ff48ae34e197955d16a3df1d539a3c05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063465"
---
# <a name="searchresult-resource-type"></a>SearchResult-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

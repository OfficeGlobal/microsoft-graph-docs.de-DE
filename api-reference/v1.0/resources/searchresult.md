---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 120f1805196e40d652bd2fcd409f4ee3cd3203fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017042"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="89622-102">SearchResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="89622-102">SearchResult resource type</span></span>

<span data-ttu-id="89622-103">Die **SearchResult**-Ressource gibt an, dass ein Element die Antwort auf eine Suchanfrage ist.</span><span class="sxs-lookup"><span data-stu-id="89622-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89622-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="89622-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="89622-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="89622-105">Properties</span></span>

| <span data-ttu-id="89622-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89622-106">Property</span></span>            | <span data-ttu-id="89622-107">Typ</span><span class="sxs-lookup"><span data-stu-id="89622-107">Type</span></span>   | <span data-ttu-id="89622-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89622-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="89622-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="89622-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="89622-110">String</span><span class="sxs-lookup"><span data-stu-id="89622-110">String</span></span> | <span data-ttu-id="89622-p101">Ein Rückruf-URL, die zum Erfassen von Telemetrieinformationen verwendet werden kann. Die Anwendung sollte ein GET für diese URL ausgeben, wenn der Benutzer mit diesem Element zur Verbesserung der Qualität der Ergebnisse interagiert.</span><span class="sxs-lookup"><span data-stu-id="89622-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="89622-113">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="89622-113">Remarks</span></span> 

<span data-ttu-id="89622-114">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="89622-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 5e8bcbc18975758586b012ee32fb32ce15313517
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876601"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="6350e-102">SearchResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6350e-102">SearchResult resource type</span></span>

<span data-ttu-id="6350e-103">Die **SearchResult**-Ressource gibt an, dass ein Element die Antwort auf eine Suchanfrage ist.</span><span class="sxs-lookup"><span data-stu-id="6350e-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6350e-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6350e-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6350e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6350e-105">Properties</span></span>

| <span data-ttu-id="6350e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6350e-106">Property</span></span>            | <span data-ttu-id="6350e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="6350e-107">Type</span></span>   | <span data-ttu-id="6350e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6350e-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="6350e-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="6350e-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="6350e-110">String</span><span class="sxs-lookup"><span data-stu-id="6350e-110">String</span></span> | <span data-ttu-id="6350e-p101">Ein Rückruf-URL, die zum Erfassen von Telemetrieinformationen verwendet werden kann. Die Anwendung sollte ein GET für diese URL ausgeben, wenn der Benutzer mit diesem Element zur Verbesserung der Qualität der Ergebnisse interagiert.</span><span class="sxs-lookup"><span data-stu-id="6350e-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="6350e-113">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="6350e-113">Remarks</span></span> 

<span data-ttu-id="6350e-114">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6350e-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

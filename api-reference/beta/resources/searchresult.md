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
# <a name="searchresult-resource-type"></a><span data-ttu-id="e25d9-102">SearchResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e25d9-102">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e25d9-103">Die **SearchResult**-Ressource gibt an, dass ein Element die Antwort auf eine Suchanfrage ist.</span><span class="sxs-lookup"><span data-stu-id="e25d9-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e25d9-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e25d9-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e25d9-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e25d9-105">Properties</span></span>

| <span data-ttu-id="e25d9-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e25d9-106">Property</span></span>            | <span data-ttu-id="e25d9-107">Typ</span><span class="sxs-lookup"><span data-stu-id="e25d9-107">Type</span></span>   | <span data-ttu-id="e25d9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e25d9-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="e25d9-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="e25d9-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="e25d9-110">String</span><span class="sxs-lookup"><span data-stu-id="e25d9-110">String</span></span> | <span data-ttu-id="e25d9-p101">Ein Rückruf-URL, die zum Erfassen von Telemetrieinformationen verwendet werden kann. Die Anwendung sollte ein GET für diese URL ausgeben, wenn der Benutzer mit diesem Element zur Verbesserung der Qualität der Ergebnisse interagiert.</span><span class="sxs-lookup"><span data-stu-id="e25d9-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="e25d9-113">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="e25d9-113">Remarks</span></span> 

<span data-ttu-id="e25d9-114">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e25d9-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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

---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 025d18a48105ddb5834040aba5944a9bd408cfbc
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480383"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="7564c-102">SearchResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7564c-102">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7564c-103">Die **SearchResult**-Ressource gibt an, dass ein Element die Antwort auf eine Suchanfrage ist.</span><span class="sxs-lookup"><span data-stu-id="7564c-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7564c-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7564c-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7564c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7564c-105">Properties</span></span>

| <span data-ttu-id="7564c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7564c-106">Property</span></span>            | <span data-ttu-id="7564c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="7564c-107">Type</span></span>   | <span data-ttu-id="7564c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7564c-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="7564c-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="7564c-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="7564c-110">String</span><span class="sxs-lookup"><span data-stu-id="7564c-110">String</span></span> | <span data-ttu-id="7564c-p101">Ein Rückruf-URL, die zum Erfassen von Telemetrieinformationen verwendet werden kann. Die Anwendung sollte ein GET für diese URL ausgeben, wenn der Benutzer mit diesem Element zur Verbesserung der Qualität der Ergebnisse interagiert.</span><span class="sxs-lookup"><span data-stu-id="7564c-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="7564c-113">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="7564c-113">Remarks</span></span> 

<span data-ttu-id="7564c-114">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7564c-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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

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
# <a name="searchresult-resource-type"></a><span data-ttu-id="0756e-102">SearchResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0756e-102">SearchResult resource type</span></span>

> <span data-ttu-id="0756e-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0756e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0756e-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0756e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0756e-105">Die **SearchResult**-Ressource gibt an, dass ein Element die Antwort auf eine Suchanfrage ist.</span><span class="sxs-lookup"><span data-stu-id="0756e-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0756e-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0756e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0756e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0756e-107">Properties</span></span>

| <span data-ttu-id="0756e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0756e-108">Property</span></span>            | <span data-ttu-id="0756e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0756e-109">Type</span></span>   | <span data-ttu-id="0756e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0756e-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="0756e-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="0756e-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="0756e-112">String</span><span class="sxs-lookup"><span data-stu-id="0756e-112">String</span></span> | <span data-ttu-id="0756e-p102">Ein Rückruf-URL, die zum Erfassen von Telemetrieinformationen verwendet werden kann. Die Anwendung sollte ein GET für diese URL ausgeben, wenn der Benutzer mit diesem Element zur Verbesserung der Qualität der Ergebnisse interagiert.</span><span class="sxs-lookup"><span data-stu-id="0756e-p102">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="0756e-115">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="0756e-115">Remarks</span></span> 

<span data-ttu-id="0756e-116">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0756e-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

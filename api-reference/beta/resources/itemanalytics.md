---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemAnalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514964"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="88b32-102">Ressourcentyp itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="88b32-102">itemAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88b32-103">Die Ressource **ItemAnalytics** bietet Analytics zu Aktivitäten, die für ein Element durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="88b32-103">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="88b32-104">Diese Ressource ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="88b32-104">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="88b32-105">Sie können auch [GetActivitiesByInterval][] API verwenden, Analytics über einen benutzerdefinierten Zeitbereich oder Intervall abgerufen.</span><span class="sxs-lookup"><span data-stu-id="88b32-105">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="88b32-106">**Hinweis:** Die Ressource **ItemAnalytics** ist noch nicht in allen [nationalen Bereitstellungen](/graph/deployments)verfügbar.</span><span class="sxs-lookup"><span data-stu-id="88b32-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="88b32-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88b32-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```

## <a name="properties"></a><span data-ttu-id="88b32-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88b32-108">Properties</span></span>

| <span data-ttu-id="88b32-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88b32-109">Property</span></span>      | <span data-ttu-id="88b32-110">Typ</span><span class="sxs-lookup"><span data-stu-id="88b32-110">Type</span></span>                 | <span data-ttu-id="88b32-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88b32-111">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="88b32-112">allTime</span><span class="sxs-lookup"><span data-stu-id="88b32-112">allTime</span></span>       | <span data-ttu-id="88b32-113">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="88b32-113">[itemActivityStat][]</span></span> | <span data-ttu-id="88b32-114">Analytics über die Lebensdauer des Elements.</span><span class="sxs-lookup"><span data-stu-id="88b32-114">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="88b32-115">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="88b32-115">lastSevenDays</span></span> | <span data-ttu-id="88b32-116">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="88b32-116">[itemActivityStat][]</span></span> | <span data-ttu-id="88b32-117">Analyse für den letzten sieben Tagen.</span><span class="sxs-lookup"><span data-stu-id="88b32-117">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemanalytics.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

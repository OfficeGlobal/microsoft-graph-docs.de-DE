---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
ms.openlocfilehash: b50df7d1fdf67cffd508c3b5891d07c599521c8a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060487"
---
# <a name="itemanalytics-resource-type"></a><span data-ttu-id="6c4d1-102">Ressourcentyp itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="6c4d1-102">itemAnalytics resource type</span></span>

> <span data-ttu-id="6c4d1-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6c4d1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c4d1-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c4d1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c4d1-105">Die Ressource **ItemAnalytics** bietet Analytics zu Aktivitäten, die für ein Element durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="6c4d1-105">The **itemAnalytics** resource provides analytics about activities that took place on an item.</span></span> <span data-ttu-id="6c4d1-106">Diese Ressource ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6c4d1-106">This resource is currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="6c4d1-107">Sie können auch [GetActivitiesByInterval][] API verwenden, Analytics über einen benutzerdefinierten Zeitbereich oder Intervall abgerufen.</span><span class="sxs-lookup"><span data-stu-id="6c4d1-107">You can also use the [getActivitiesByInterval][] API to retrieve analytics over a custom time range or interval.</span></span>

><span data-ttu-id="6c4d1-108">**Hinweis:** Die Ressource **ItemAnalytics** ist noch nicht in allen [nationalen Bereitstellungen](/graph/deployments)verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6c4d1-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c4d1-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6c4d1-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6c4d1-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6c4d1-110">Properties</span></span>

| <span data-ttu-id="6c4d1-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c4d1-111">Property</span></span>      | <span data-ttu-id="6c4d1-112">Typ</span><span class="sxs-lookup"><span data-stu-id="6c4d1-112">Type</span></span>                 | <span data-ttu-id="6c4d1-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c4d1-113">Description</span></span>
|:--------------|:---------------------|:--------------------------------------
| <span data-ttu-id="6c4d1-114">allTime</span><span class="sxs-lookup"><span data-stu-id="6c4d1-114">allTime</span></span>       | <span data-ttu-id="6c4d1-115">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="6c4d1-115">[itemActivityStat][]</span></span> | <span data-ttu-id="6c4d1-116">Analytics über die Lebensdauer des Elements.</span><span class="sxs-lookup"><span data-stu-id="6c4d1-116">Analytics over the the item's lifespan.</span></span>
| <span data-ttu-id="6c4d1-117">lastSevenDays</span><span class="sxs-lookup"><span data-stu-id="6c4d1-117">lastSevenDays</span></span> | <span data-ttu-id="6c4d1-118">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="6c4d1-118">[itemActivityStat][]</span></span> | <span data-ttu-id="6c4d1-119">Analyse für den letzten sieben Tagen.</span><span class="sxs-lookup"><span data-stu-id="6c4d1-119">Analytics for the last seven days.</span></span>

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->

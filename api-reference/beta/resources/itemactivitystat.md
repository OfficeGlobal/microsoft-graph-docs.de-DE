---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517631"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="a013b-102">Ressourcentyp itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="a013b-102">itemActivityStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a013b-103">Die Ressource **ItemActivityStat** enthält Informationen zu Aktivitäten, die innerhalb eines Zeitintervalls durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="a013b-103">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a013b-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a013b-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

## <a name="properties"></a><span data-ttu-id="a013b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a013b-105">Properties</span></span>

| <span data-ttu-id="a013b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a013b-106">Property</span></span>         | <span data-ttu-id="a013b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="a013b-107">Type</span></span>                    | <span data-ttu-id="a013b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a013b-108">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="a013b-109">incompleteData</span><span class="sxs-lookup"><span data-stu-id="a013b-109">incompleteData</span></span>   | <span data-ttu-id="a013b-110">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="a013b-110">[incompleteData][]</span></span>      | <span data-ttu-id="a013b-111">Gibt an, dass die Statistiken in diesem Zeitraum auf unvollständiger Daten basieren.</span><span class="sxs-lookup"><span data-stu-id="a013b-111">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="a013b-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-112">Read-only.</span></span>
| <span data-ttu-id="a013b-113">isTrending</span><span class="sxs-lookup"><span data-stu-id="a013b-113">isTrending</span></span>       | <span data-ttu-id="a013b-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a013b-114">Boolean</span></span>                 | <span data-ttu-id="a013b-115">Gibt an, ob das Element "Trend."</span><span class="sxs-lookup"><span data-stu-id="a013b-115">Indicates whether the item is "trending."</span></span> <span data-ttu-id="a013b-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-116">Read-only.</span></span>
| <span data-ttu-id="a013b-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a013b-117">startDateTime</span></span>    | <span data-ttu-id="a013b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a013b-118">DateTimeOffset</span></span>          | <span data-ttu-id="a013b-119">Wenn das Intervall gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="a013b-119">When the interval starts.</span></span> <span data-ttu-id="a013b-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-120">Read-only.</span></span>
| <span data-ttu-id="a013b-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a013b-121">endDateTime</span></span>      | <span data-ttu-id="a013b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a013b-122">DateTimeOffset</span></span>          | <span data-ttu-id="a013b-123">Wenn das Intervall endet.</span><span class="sxs-lookup"><span data-stu-id="a013b-123">When the interval ends.</span></span> <span data-ttu-id="a013b-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-124">Read-only.</span></span>
| <span data-ttu-id="a013b-125">create</span><span class="sxs-lookup"><span data-stu-id="a013b-125">create</span></span>           | <span data-ttu-id="a013b-126">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="a013b-126">[itemActionStat][]</span></span>      | <span data-ttu-id="a013b-127">Statistiken zum **Erstellen von** Aktionen in diesem Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="a013b-127">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="a013b-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-128">Read-only.</span></span>
| <span data-ttu-id="a013b-129">Bearbeiten</span><span class="sxs-lookup"><span data-stu-id="a013b-129">edit</span></span>             | <span data-ttu-id="a013b-130">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="a013b-130">[itemActionStat][]</span></span>      | <span data-ttu-id="a013b-131">Statistiken zum **Bearbeiten von** Aktionen in diesem Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="a013b-131">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="a013b-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-132">Read-only.</span></span>
| <span data-ttu-id="a013b-133">Löschen</span><span class="sxs-lookup"><span data-stu-id="a013b-133">delete</span></span>           | <span data-ttu-id="a013b-134">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="a013b-134">[itemActionStat][]</span></span>      | <span data-ttu-id="a013b-135">Statistiken zu **Löschaktionen in diesem Zeitraum** .</span><span class="sxs-lookup"><span data-stu-id="a013b-135">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="a013b-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-136">Read-only.</span></span>
| <span data-ttu-id="a013b-137">verschieben</span><span class="sxs-lookup"><span data-stu-id="a013b-137">move</span></span>             | <span data-ttu-id="a013b-138">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="a013b-138">[itemActionStat][]</span></span>      | <span data-ttu-id="a013b-139">Statistiken zu **Verschieben** Aktionen in diesem Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="a013b-139">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="a013b-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-140">Read-only.</span></span>
| <span data-ttu-id="a013b-141">access</span><span class="sxs-lookup"><span data-stu-id="a013b-141">access</span></span>           | <span data-ttu-id="a013b-142">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="a013b-142">[itemActionStat][]</span></span>      | <span data-ttu-id="a013b-143">Statistiken zu **Access** -Aktionen in diesem Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="a013b-143">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="a013b-144">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a013b-144">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="a013b-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a013b-147">Relationships</span></span>

| <span data-ttu-id="a013b-148">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="a013b-148">Relationship name</span></span> | <span data-ttu-id="a013b-149">Typ</span><span class="sxs-lookup"><span data-stu-id="a013b-149">Type</span></span>                        | <span data-ttu-id="a013b-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a013b-150">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="a013b-151">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="a013b-151">activities</span></span>        | <span data-ttu-id="a013b-152">[itemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a013b-152">[itemActivity][] collection</span></span> | <span data-ttu-id="a013b-153">Macht die **ItemActivities** in diese Ressource **ItemActivityStat** dargestellt.</span><span class="sxs-lookup"><span data-stu-id="a013b-153">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="a013b-155">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="a013b-155">Remarks</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
ms.openlocfilehash: 067cf88773b5f5d69b2b3538a2ddeab6741631a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058467"
---
# <a name="itemactivitystat-resource-type"></a><span data-ttu-id="cb87f-102">Ressourcentyp itemActivityStat</span><span class="sxs-lookup"><span data-stu-id="cb87f-102">itemActivityStat resource type</span></span>

> <span data-ttu-id="cb87f-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cb87f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb87f-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb87f-105">Die Ressource **ItemActivityStat** enthält Informationen zu Aktivitäten, die innerhalb eines Zeitintervalls durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="cb87f-105">The **itemActivityStat** resource provides information about activities that took place within an interval of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb87f-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb87f-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cb87f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb87f-107">Properties</span></span>

| <span data-ttu-id="cb87f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb87f-108">Property</span></span>         | <span data-ttu-id="cb87f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="cb87f-109">Type</span></span>                    | <span data-ttu-id="cb87f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb87f-110">Description</span></span>
|:-----------------|:------------------------|:----------------------------------------
| <span data-ttu-id="cb87f-111">incompleteData</span><span class="sxs-lookup"><span data-stu-id="cb87f-111">incompleteData</span></span>   | <span data-ttu-id="cb87f-112">[incompleteData][]</span><span class="sxs-lookup"><span data-stu-id="cb87f-112">[incompleteData][]</span></span>      | <span data-ttu-id="cb87f-113">Gibt an, dass die Statistiken in diesem Zeitraum auf unvollständiger Daten basieren.</span><span class="sxs-lookup"><span data-stu-id="cb87f-113">Indicates that the statistics in this interval are based on incomplete data.</span></span> <span data-ttu-id="cb87f-114">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-114">Read-only.</span></span>
| <span data-ttu-id="cb87f-115">isTrending</span><span class="sxs-lookup"><span data-stu-id="cb87f-115">isTrending</span></span>       | <span data-ttu-id="cb87f-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cb87f-116">Boolean</span></span>                 | <span data-ttu-id="cb87f-117">Gibt an, ob das Element "Trend."</span><span class="sxs-lookup"><span data-stu-id="cb87f-117">Indicates whether the item is "trending."</span></span> <span data-ttu-id="cb87f-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-118">Read-only.</span></span>
| <span data-ttu-id="cb87f-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cb87f-119">startDateTime</span></span>    | <span data-ttu-id="cb87f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb87f-120">DateTimeOffset</span></span>          | <span data-ttu-id="cb87f-121">Wenn das Intervall gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="cb87f-121">When the interval starts.</span></span> <span data-ttu-id="cb87f-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-122">Read-only.</span></span>
| <span data-ttu-id="cb87f-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="cb87f-123">endDateTime</span></span>      | <span data-ttu-id="cb87f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb87f-124">DateTimeOffset</span></span>          | <span data-ttu-id="cb87f-125">Wenn das Intervall endet.</span><span class="sxs-lookup"><span data-stu-id="cb87f-125">When the interval ends.</span></span> <span data-ttu-id="cb87f-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-126">Read-only.</span></span>
| <span data-ttu-id="cb87f-127">create</span><span class="sxs-lookup"><span data-stu-id="cb87f-127">create</span></span>           | <span data-ttu-id="cb87f-128">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="cb87f-128">[itemActionStat][]</span></span>      | <span data-ttu-id="cb87f-129">Statistiken zum **Erstellen von** Aktionen in diesem Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="cb87f-129">Statistics about the **create** actions in this interval.</span></span> <span data-ttu-id="cb87f-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-130">Read-only.</span></span>
| <span data-ttu-id="cb87f-131">Bearbeiten</span><span class="sxs-lookup"><span data-stu-id="cb87f-131">edit</span></span>             | <span data-ttu-id="cb87f-132">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="cb87f-132">[itemActionStat][]</span></span>      | <span data-ttu-id="cb87f-133">Statistiken zum **Bearbeiten von** Aktionen in diesem Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="cb87f-133">Statistics about the **edit** actions in this interval.</span></span> <span data-ttu-id="cb87f-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-134">Read-only.</span></span>
| <span data-ttu-id="cb87f-135">Löschen</span><span class="sxs-lookup"><span data-stu-id="cb87f-135">delete</span></span>           | <span data-ttu-id="cb87f-136">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="cb87f-136">[itemActionStat][]</span></span>      | <span data-ttu-id="cb87f-137">Statistiken zu **Löschaktionen in diesem Zeitraum** .</span><span class="sxs-lookup"><span data-stu-id="cb87f-137">Statistics about the **delete** actions in this interval.</span></span> <span data-ttu-id="cb87f-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-138">Read-only.</span></span>
| <span data-ttu-id="cb87f-139">verschieben</span><span class="sxs-lookup"><span data-stu-id="cb87f-139">move</span></span>             | <span data-ttu-id="cb87f-140">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="cb87f-140">[itemActionStat][]</span></span>      | <span data-ttu-id="cb87f-141">Statistiken zu **Verschieben** Aktionen in diesem Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="cb87f-141">Statistics about the **move** actions in this interval.</span></span> <span data-ttu-id="cb87f-142">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-142">Read-only.</span></span>
| <span data-ttu-id="cb87f-143">Zugriff</span><span class="sxs-lookup"><span data-stu-id="cb87f-143">access</span></span>           | <span data-ttu-id="cb87f-144">[itemActionStat][]</span><span class="sxs-lookup"><span data-stu-id="cb87f-144">[itemActionStat][]</span></span>      | <span data-ttu-id="cb87f-145">Statistiken zu **Access** -Aktionen in diesem Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="cb87f-145">Statistics about the **access** actions in this interval.</span></span> <span data-ttu-id="cb87f-146">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-146">Read-only.</span></span>

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a><span data-ttu-id="cb87f-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cb87f-149">Relationships</span></span>

| <span data-ttu-id="cb87f-150">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="cb87f-150">Relationship name</span></span> | <span data-ttu-id="cb87f-151">Typ</span><span class="sxs-lookup"><span data-stu-id="cb87f-151">Type</span></span>                        | <span data-ttu-id="cb87f-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb87f-152">Description</span></span>
|:------------------|:----------------------------|:---------------------------
| <span data-ttu-id="cb87f-153">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="cb87f-153">activities</span></span>        | <span data-ttu-id="cb87f-154">[itemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cb87f-154">[itemActivity][] collection</span></span> | <span data-ttu-id="cb87f-155">Macht die **ItemActivities** in diese Ressource **ItemActivityStat** dargestellt.</span><span class="sxs-lookup"><span data-stu-id="cb87f-155">Exposes the **itemActivities** represented in this **itemActivityStat** resource.</span></span>

[itemActivity]: itemactivity.md

## <a name="remarks"></a><span data-ttu-id="cb87f-157">Hinweise</span><span class="sxs-lookup"><span data-stu-id="cb87f-157">Remarks</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->

---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 2ff3e1a2356c43457fe251928728632bd2228b10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809892"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="ee044-102">ItemActivityTimeSet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ee044-102">ItemActivityTimeSet resource type</span></span>

> <span data-ttu-id="ee044-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ee044-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee044-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee044-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ee044-105">Die **ItemActivityTimeSet**-Ressource enthält Informationen darüber, wann eine [Aktivität][activity] in einem Element stattfindet.</span><span class="sxs-lookup"><span data-stu-id="ee044-105">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="ee044-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ee044-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="ee044-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ee044-107">Properties</span></span>

| <span data-ttu-id="ee044-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="ee044-108">Property name</span></span>    | <span data-ttu-id="ee044-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ee044-109">Type</span></span>           | <span data-ttu-id="ee044-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee044-110">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="ee044-111">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee044-111">observedDateTime</span></span> | <span data-ttu-id="ee044-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee044-112">DateTimeOffset</span></span> | <span data-ttu-id="ee044-113">Wann die Ausführung der Aktivität beobachtet wurde.</span><span class="sxs-lookup"><span data-stu-id="ee044-113">When the activity was observed to take place.</span></span>
| <span data-ttu-id="ee044-114">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee044-114">recordedDateTime</span></span> | <span data-ttu-id="ee044-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee044-115">DateTimeOffset</span></span> | <span data-ttu-id="ee044-116">Wann die Beobachtung vom Dienst aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="ee044-116">When the observation was recorded on the service.</span></span>

<span data-ttu-id="ee044-117">Der Unterschied zwischen den Zeiten **observed** und **recorded** ist besonders wichtig bei Offline-Zusammenarbeitsszenarien.</span><span class="sxs-lookup"><span data-stu-id="ee044-117">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="ee044-118">Wenn ein Benutzer offline eine Datei kommentiert, wird der Zeitpunkt des Kommentars als **observedDateTime** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ee044-118">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="ee044-119">Wenn sich der Benutzer zu einem späteren Zeitpunkt erneut mit der Cloud verbindet und die Änderungen hochgeladen werden, wird dieser Zeitpunkt als **recordedDateTime** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ee044-119">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="ee044-120">Hinweise</span><span class="sxs-lookup"><span data-stu-id="ee044-120">Remarks</span></span>

<span data-ttu-id="ee044-121">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ee044-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->

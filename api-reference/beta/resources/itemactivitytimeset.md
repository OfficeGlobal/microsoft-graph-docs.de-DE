---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 474d20e08d96294a30029e764d0b01f5b0c6bfcd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518513"
---
# <a name="itemactivitytimeset-resource-type"></a><span data-ttu-id="5f14c-102">ItemActivityTimeSet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5f14c-102">ItemActivityTimeSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f14c-103">Die **ItemActivityTimeSet**-Ressource enthält Informationen darüber, wann eine [Aktivität][activity] in einem Element stattfindet.</span><span class="sxs-lookup"><span data-stu-id="5f14c-103">The **ItemActivityTimeSet** resource provides information about when an [activity][activity] on an item took place.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5f14c-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f14c-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5f14c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f14c-105">Properties</span></span>

| <span data-ttu-id="5f14c-106">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="5f14c-106">Property name</span></span>    | <span data-ttu-id="5f14c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="5f14c-107">Type</span></span>           | <span data-ttu-id="5f14c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f14c-108">Description</span></span>
|:-----------------|:---------------|:-----------------------------------------
| <span data-ttu-id="5f14c-109">observedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f14c-109">observedDateTime</span></span> | <span data-ttu-id="5f14c-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f14c-110">DateTimeOffset</span></span> | <span data-ttu-id="5f14c-111">Wann die Ausführung der Aktivität beobachtet wurde.</span><span class="sxs-lookup"><span data-stu-id="5f14c-111">When the activity was observed to take place.</span></span>
| <span data-ttu-id="5f14c-112">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f14c-112">recordedDateTime</span></span> | <span data-ttu-id="5f14c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f14c-113">DateTimeOffset</span></span> | <span data-ttu-id="5f14c-114">Wann die Beobachtung vom Dienst aufgezeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="5f14c-114">When the observation was recorded on the service.</span></span>

<span data-ttu-id="5f14c-115">Der Unterschied zwischen den Zeiten **observed** und **recorded** ist besonders wichtig bei Offline-Zusammenarbeitsszenarien.</span><span class="sxs-lookup"><span data-stu-id="5f14c-115">The difference between **observed** and **recorded** times is especially important for offline collaboration scenarios.</span></span>
<span data-ttu-id="5f14c-116">Wenn ein Benutzer offline eine Datei kommentiert, wird der Zeitpunkt des Kommentars als **observedDateTime** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5f14c-116">If a user comments on a file while offline, the time that they make the comment is set as the **observedDateTime**.</span></span>
<span data-ttu-id="5f14c-117">Wenn sich der Benutzer zu einem späteren Zeitpunkt erneut mit der Cloud verbindet und die Änderungen hochgeladen werden, wird dieser Zeitpunkt als **recordedDateTime** festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5f14c-117">At a later time when the user re-connects to the cloud and the changes get uploaded, that later time is set as the **recordedDateTime**.</span></span>

## <a name="remarks"></a><span data-ttu-id="5f14c-118">Hinweise</span><span class="sxs-lookup"><span data-stu-id="5f14c-118">Remarks</span></span>

<span data-ttu-id="5f14c-119">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5f14c-119">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitytimeset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

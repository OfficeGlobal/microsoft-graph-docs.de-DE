---
title: Ressourcentyp licenseAssignmentState
description: Die **LicenseAssignmentStates** -Eigenschaft der Benutzerentität ist eine Auflistung von **LicenseAssignmentState** -Objekten. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649419"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="13b8a-104">Ressourcentyp licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="13b8a-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="13b8a-105">Die **LicenseAssignmentStates** -Eigenschaft der Entität [Benutzer](user.md) ist eine Auflistung von **LicenseAssignmentState** -Objekten.</span><span class="sxs-lookup"><span data-stu-id="13b8a-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="13b8a-106">Es enthält Details zur Lizenz Zuordnungen für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="13b8a-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="13b8a-107">Die Details enthalten Informationen wie etwa:</span><span class="sxs-lookup"><span data-stu-id="13b8a-107">The details include information such as:</span></span>  

 - <span data-ttu-id="13b8a-108">Welche Pläne für einen Benutzer deaktiviert sind</span><span class="sxs-lookup"><span data-stu-id="13b8a-108">What plans are disabled for a user</span></span>
 - <span data-ttu-id="13b8a-109">Gibt an, ob die Lizenz zugewiesen, die dem Benutzer direkt oder aus einer Gruppe geerbt wurde</span><span class="sxs-lookup"><span data-stu-id="13b8a-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="13b8a-110">Den aktuellen Status der Zuordnung</span><span class="sxs-lookup"><span data-stu-id="13b8a-110">The current state of the assignment</span></span>
 - <span data-ttu-id="13b8a-111">Wenn der Zuordnung Zustand Fehler ist Fehlerdetails</span><span class="sxs-lookup"><span data-stu-id="13b8a-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="13b8a-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13b8a-112">Properties</span></span>
| <span data-ttu-id="13b8a-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13b8a-113">Property</span></span>     | <span data-ttu-id="13b8a-114">Typ</span><span class="sxs-lookup"><span data-stu-id="13b8a-114">Type</span></span>   |<span data-ttu-id="13b8a-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13b8a-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13b8a-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="13b8a-116">assignedByGroup</span></span>|<span data-ttu-id="13b8a-117">string</span><span class="sxs-lookup"><span data-stu-id="13b8a-117">string</span></span>|<span data-ttu-id="13b8a-118">Die Id der Gruppe, die diese Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="13b8a-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="13b8a-119">Wenn die Zuordnung einer Lizenz Direct zugewiesen ist, werden in diesem Feld auf Null festgelegt.</span><span class="sxs-lookup"><span data-stu-id="13b8a-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="13b8a-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13b8a-120">Read-Only.</span></span>|
|<span data-ttu-id="13b8a-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="13b8a-121">disabledPlans</span></span>|<span data-ttu-id="13b8a-122">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="13b8a-122">Collection(String)</span></span>|<span data-ttu-id="13b8a-123">Die Servicepläne, die in dieser Aufgabe deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="13b8a-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="13b8a-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13b8a-124">Read-Only.</span></span>|
|<span data-ttu-id="13b8a-125">error</span><span class="sxs-lookup"><span data-stu-id="13b8a-125">error</span></span>|<span data-ttu-id="13b8a-126">String</span><span class="sxs-lookup"><span data-stu-id="13b8a-126">String</span></span>|<span data-ttu-id="13b8a-127">Lizenz-Zuordnung-Fehler.</span><span class="sxs-lookup"><span data-stu-id="13b8a-127">License assignment failure error.</span></span> <span data-ttu-id="13b8a-128">Wenn die Lizenz erfolgreich zugewiesen ist, werden in diesem Feld auf Null festgelegt.</span><span class="sxs-lookup"><span data-stu-id="13b8a-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="13b8a-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13b8a-129">Read-Only.</span></span> <span data-ttu-id="13b8a-130">Mögliche Werte: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, und `Others`.</span><span class="sxs-lookup"><span data-stu-id="13b8a-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="13b8a-131">Weitere Informationen zum Identifizieren und Beheben von lizenzzuweisung Fehler finden Sie [hier](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="13b8a-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="13b8a-132">skuId</span><span class="sxs-lookup"><span data-stu-id="13b8a-132">skuId</span></span>|<span data-ttu-id="13b8a-133">String</span><span class="sxs-lookup"><span data-stu-id="13b8a-133">String</span></span>|<span data-ttu-id="13b8a-134">Die eindeutige ID der SKU.</span><span class="sxs-lookup"><span data-stu-id="13b8a-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="13b8a-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13b8a-135">Read-Only.</span></span>|
|<span data-ttu-id="13b8a-136">state</span><span class="sxs-lookup"><span data-stu-id="13b8a-136">state</span></span>|<span data-ttu-id="13b8a-137">String</span><span class="sxs-lookup"><span data-stu-id="13b8a-137">String</span></span>|<span data-ttu-id="13b8a-138">Geben Sie den aktuellen Status dieser Aufgabe an.</span><span class="sxs-lookup"><span data-stu-id="13b8a-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="13b8a-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13b8a-139">Read-Only.</span></span> <span data-ttu-id="13b8a-140">Mögliche Werte: aktiv "," ActiveWithError "," deaktiviert "und" Fehler.</span><span class="sxs-lookup"><span data-stu-id="13b8a-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13b8a-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13b8a-141">JSON representation</span></span>

<span data-ttu-id="13b8a-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13b8a-142">The following is a JSON representation of the resource.</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->

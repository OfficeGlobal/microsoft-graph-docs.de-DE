---
title: Ressourcentyp licenseAssignmentState
description: 'Die **LicenseAssignmentStates** -Eigenschaft der Benutzerentität ist eine Auflistung von **LicenseAssignmentState**. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer. Die Details enthält Informationen wie folgt:  '
localization_priority: Normal
ms.openlocfilehash: 51ff878f356902362487eda36d17c1894c33e5f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855629"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="18eb1-105">Ressourcentyp licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="18eb1-105">licenseAssignmentState resource type</span></span>

> <span data-ttu-id="18eb1-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="18eb1-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18eb1-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18eb1-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18eb1-108">Die **LicenseAssignmentStates** -Eigenschaft der Entität [Benutzer](user.md) ist eine Auflistung von **LicenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="18eb1-108">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="18eb1-109">Es enthält Details zur Lizenz Zuordnungen für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="18eb1-109">It provides details about license assignments to a user.</span></span> <span data-ttu-id="18eb1-110">Die Details enthält Informationen wie folgt:</span><span class="sxs-lookup"><span data-stu-id="18eb1-110">The details includes information like:</span></span>  

 - <span data-ttu-id="18eb1-111">Welche Pläne für einen Benutzer deaktiviert sind</span><span class="sxs-lookup"><span data-stu-id="18eb1-111">What plans are disabled for a user</span></span>
 - <span data-ttu-id="18eb1-112">Gibt an, ob die Lizenz zugewiesen, die dem Benutzer direkt oder aus einer Gruppe geerbt wurde</span><span class="sxs-lookup"><span data-stu-id="18eb1-112">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="18eb1-113">Aktuellen Status der Zuordnung</span><span class="sxs-lookup"><span data-stu-id="18eb1-113">Current state of the assignment</span></span>
 - <span data-ttu-id="18eb1-114">Wenn der Zuordnung Zustand Fehler ist, was die Fehlerdetails für den Fehler ist?</span><span class="sxs-lookup"><span data-stu-id="18eb1-114">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="18eb1-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="18eb1-115">Properties</span></span>
| <span data-ttu-id="18eb1-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="18eb1-116">Property</span></span>     | <span data-ttu-id="18eb1-117">Typ</span><span class="sxs-lookup"><span data-stu-id="18eb1-117">Type</span></span>   |<span data-ttu-id="18eb1-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18eb1-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18eb1-119">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="18eb1-119">assignedByGroup</span></span>|<span data-ttu-id="18eb1-120">string</span><span class="sxs-lookup"><span data-stu-id="18eb1-120">string</span></span>|<span data-ttu-id="18eb1-121">Die Id der Gruppe, die diese Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="18eb1-121">The id of the group that assigns this license.</span></span> <span data-ttu-id="18eb1-122">Wenn die Zuordnung einer Lizenz Direct zugewiesen ist, werden in diesem Feld auf Null festgelegt.</span><span class="sxs-lookup"><span data-stu-id="18eb1-122">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="18eb1-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18eb1-123">Read-Only.</span></span>|
|<span data-ttu-id="18eb1-124">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="18eb1-124">disabledPlans</span></span>|<span data-ttu-id="18eb1-125">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="18eb1-125">Collection(String)</span></span>|<span data-ttu-id="18eb1-126">Die Servicepläne, die in dieser Aufgabe deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="18eb1-126">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="18eb1-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18eb1-127">Read-Only.</span></span>|
|<span data-ttu-id="18eb1-128">error</span><span class="sxs-lookup"><span data-stu-id="18eb1-128">error</span></span>|<span data-ttu-id="18eb1-129">String</span><span class="sxs-lookup"><span data-stu-id="18eb1-129">String</span></span>|<span data-ttu-id="18eb1-130">Lizenz-Zuordnung-Fehler.</span><span class="sxs-lookup"><span data-stu-id="18eb1-130">License assignment failure error.</span></span> <span data-ttu-id="18eb1-131">Wenn die Lizenz erfolgreich zugewiesen ist, werden in diesem Feld auf Null festgelegt.</span><span class="sxs-lookup"><span data-stu-id="18eb1-131">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="18eb1-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18eb1-132">Read-Only.</span></span> <span data-ttu-id="18eb1-133">Mögliche Werte: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, und `Others`.</span><span class="sxs-lookup"><span data-stu-id="18eb1-133">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="18eb1-134">Weitere Informationen zum Identifizieren und Beheben von lizenzzuweisung Fehler finden Sie [hier](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="18eb1-134">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="18eb1-135">skuId</span><span class="sxs-lookup"><span data-stu-id="18eb1-135">skuId</span></span>|<span data-ttu-id="18eb1-136">String</span><span class="sxs-lookup"><span data-stu-id="18eb1-136">String</span></span>|<span data-ttu-id="18eb1-137">Die eindeutige ID der SKU.</span><span class="sxs-lookup"><span data-stu-id="18eb1-137">The unique identifier for the SKU.</span></span> <span data-ttu-id="18eb1-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18eb1-138">Read-Only.</span></span>|
|<span data-ttu-id="18eb1-139">state</span><span class="sxs-lookup"><span data-stu-id="18eb1-139">state</span></span>|<span data-ttu-id="18eb1-140">String</span><span class="sxs-lookup"><span data-stu-id="18eb1-140">String</span></span>|<span data-ttu-id="18eb1-141">Geben Sie den aktuellen Status dieser Aufgabe an.</span><span class="sxs-lookup"><span data-stu-id="18eb1-141">Indicate the current state of this assignment.</span></span> <span data-ttu-id="18eb1-142">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18eb1-142">Read-Only.</span></span> <span data-ttu-id="18eb1-143">Mögliche Werte: aktiv "," ActiveWithError "," deaktiviert "und" Fehler.</span><span class="sxs-lookup"><span data-stu-id="18eb1-143">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18eb1-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="18eb1-144">JSON representation</span></span>

<span data-ttu-id="18eb1-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="18eb1-145">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```

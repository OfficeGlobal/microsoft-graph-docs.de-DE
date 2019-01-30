---
title: Ressourcentyp licenseAssignmentState
description: 'Die **LicenseAssignmentStates** -Eigenschaft der Benutzerentität ist eine Auflistung von **LicenseAssignmentState**. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer. Die Details enthält Informationen wie folgt:  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641680"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="e17da-105">Ressourcentyp licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="e17da-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e17da-106">Die **LicenseAssignmentStates** -Eigenschaft der Entität [Benutzer](user.md) ist eine Auflistung von **LicenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="e17da-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="e17da-107">Es enthält Details zur Lizenz Zuordnungen für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="e17da-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="e17da-108">Die Details enthält Informationen wie folgt:</span><span class="sxs-lookup"><span data-stu-id="e17da-108">The details includes information like:</span></span>  

 - <span data-ttu-id="e17da-109">Welche Pläne für einen Benutzer deaktiviert sind</span><span class="sxs-lookup"><span data-stu-id="e17da-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="e17da-110">Gibt an, ob die Lizenz zugewiesen, die dem Benutzer direkt oder aus einer Gruppe geerbt wurde</span><span class="sxs-lookup"><span data-stu-id="e17da-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="e17da-111">Aktuellen Status der Zuordnung</span><span class="sxs-lookup"><span data-stu-id="e17da-111">Current state of the assignment</span></span>
 - <span data-ttu-id="e17da-112">Wenn der Zuordnung Zustand Fehler ist, was die Fehlerdetails für den Fehler ist?</span><span class="sxs-lookup"><span data-stu-id="e17da-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="e17da-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e17da-113">Properties</span></span>
| <span data-ttu-id="e17da-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e17da-114">Property</span></span>     | <span data-ttu-id="e17da-115">Typ</span><span class="sxs-lookup"><span data-stu-id="e17da-115">Type</span></span>   |<span data-ttu-id="e17da-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e17da-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e17da-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="e17da-117">assignedByGroup</span></span>|<span data-ttu-id="e17da-118">string</span><span class="sxs-lookup"><span data-stu-id="e17da-118">string</span></span>|<span data-ttu-id="e17da-119">Die Id der Gruppe, die diese Lizenz zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e17da-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="e17da-120">Wenn die Zuordnung einer Lizenz Direct zugewiesen ist, werden in diesem Feld auf Null festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e17da-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="e17da-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e17da-121">Read-Only.</span></span>|
|<span data-ttu-id="e17da-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="e17da-122">disabledPlans</span></span>|<span data-ttu-id="e17da-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="e17da-123">Collection(String)</span></span>|<span data-ttu-id="e17da-124">Die Servicepläne, die in dieser Aufgabe deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="e17da-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="e17da-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e17da-125">Read-Only.</span></span>|
|<span data-ttu-id="e17da-126">error</span><span class="sxs-lookup"><span data-stu-id="e17da-126">error</span></span>|<span data-ttu-id="e17da-127">String</span><span class="sxs-lookup"><span data-stu-id="e17da-127">String</span></span>|<span data-ttu-id="e17da-128">Lizenz-Zuordnung-Fehler.</span><span class="sxs-lookup"><span data-stu-id="e17da-128">License assignment failure error.</span></span> <span data-ttu-id="e17da-129">Wenn die Lizenz erfolgreich zugewiesen ist, werden in diesem Feld auf Null festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e17da-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="e17da-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e17da-130">Read-Only.</span></span> <span data-ttu-id="e17da-131">Mögliche Werte: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, und `Others`.</span><span class="sxs-lookup"><span data-stu-id="e17da-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="e17da-132">Weitere Informationen zum Identifizieren und Beheben von lizenzzuweisung Fehler finden Sie [hier](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="e17da-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="e17da-133">skuId</span><span class="sxs-lookup"><span data-stu-id="e17da-133">skuId</span></span>|<span data-ttu-id="e17da-134">String</span><span class="sxs-lookup"><span data-stu-id="e17da-134">String</span></span>|<span data-ttu-id="e17da-135">Die eindeutige ID der SKU.</span><span class="sxs-lookup"><span data-stu-id="e17da-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="e17da-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e17da-136">Read-Only.</span></span>|
|<span data-ttu-id="e17da-137">state</span><span class="sxs-lookup"><span data-stu-id="e17da-137">state</span></span>|<span data-ttu-id="e17da-138">String</span><span class="sxs-lookup"><span data-stu-id="e17da-138">String</span></span>|<span data-ttu-id="e17da-139">Geben Sie den aktuellen Status dieser Aufgabe an.</span><span class="sxs-lookup"><span data-stu-id="e17da-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="e17da-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e17da-140">Read-Only.</span></span> <span data-ttu-id="e17da-141">Mögliche Werte: aktiv "," ActiveWithError "," deaktiviert "und" Fehler.</span><span class="sxs-lookup"><span data-stu-id="e17da-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e17da-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e17da-142">JSON representation</span></span>

<span data-ttu-id="e17da-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e17da-143">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

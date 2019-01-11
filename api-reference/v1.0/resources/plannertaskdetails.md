---
title: plannerTaskDetails-Ressourcentyp
description: Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes task-Objekt hat ein Detailobjekt.
localization_priority: Normal
ms.openlocfilehash: a183ba0f9b19ea2de700913d29e9586442ba2c03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806574"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="d33de-104">plannerTaskDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d33de-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="d33de-p102">Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="d33de-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="d33de-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="d33de-107">Methods</span></span>

| <span data-ttu-id="d33de-108">Methode</span><span class="sxs-lookup"><span data-stu-id="d33de-108">Method</span></span>           | <span data-ttu-id="d33de-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d33de-109">Return Type</span></span>    |<span data-ttu-id="d33de-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d33de-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d33de-111">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="d33de-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="d33de-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d33de-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="d33de-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d33de-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="d33de-114">Update</span><span class="sxs-lookup"><span data-stu-id="d33de-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="d33de-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d33de-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="d33de-116">Dient zum Aktualisieren des **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d33de-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d33de-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d33de-117">Properties</span></span>
| <span data-ttu-id="d33de-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d33de-118">Property</span></span>     | <span data-ttu-id="d33de-119">Typ</span><span class="sxs-lookup"><span data-stu-id="d33de-119">Type</span></span>   |<span data-ttu-id="d33de-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d33de-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d33de-121">checklist</span><span class="sxs-lookup"><span data-stu-id="d33de-121">checklist</span></span>|[<span data-ttu-id="d33de-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="d33de-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="d33de-123">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="d33de-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="d33de-124">description</span><span class="sxs-lookup"><span data-stu-id="d33de-124">description</span></span>|<span data-ttu-id="d33de-125">String</span><span class="sxs-lookup"><span data-stu-id="d33de-125">String</span></span>|<span data-ttu-id="d33de-126">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="d33de-126">Description of the task</span></span>|
|<span data-ttu-id="d33de-127">id</span><span class="sxs-lookup"><span data-stu-id="d33de-127">id</span></span>|<span data-ttu-id="d33de-128">String</span><span class="sxs-lookup"><span data-stu-id="d33de-128">String</span></span>| <span data-ttu-id="d33de-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d33de-129">Read-only.</span></span> <span data-ttu-id="d33de-130">ID des die Aufgabendetails.</span><span class="sxs-lookup"><span data-stu-id="d33de-130">ID of the task details.</span></span> <span data-ttu-id="d33de-131">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="d33de-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d33de-132">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="d33de-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d33de-133">previewType</span><span class="sxs-lookup"><span data-stu-id="d33de-133">previewType</span></span>|<span data-ttu-id="d33de-134">string</span><span class="sxs-lookup"><span data-stu-id="d33de-134">string</span></span>|<span data-ttu-id="d33de-135">Hierdurch wird den Typ der Vorschau, die für den Vorgang wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d33de-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="d33de-136">Die möglichen Werte sind: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="d33de-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="d33de-137">Bei Festlegung auf `automatic` die angezeigte Vorschau wird von der app anzeigen den Vorgang ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="d33de-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="d33de-138">references</span><span class="sxs-lookup"><span data-stu-id="d33de-138">references</span></span>|[<span data-ttu-id="d33de-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="d33de-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="d33de-140">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="d33de-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d33de-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d33de-141">Relationships</span></span>
<span data-ttu-id="d33de-142">Keine</span><span class="sxs-lookup"><span data-stu-id="d33de-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d33de-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d33de-143">JSON representation</span></span>
<span data-ttu-id="d33de-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d33de-144">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

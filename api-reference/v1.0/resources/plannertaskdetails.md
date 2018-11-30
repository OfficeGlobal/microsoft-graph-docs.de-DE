---
title: plannerTaskDetails-Ressourcentyp
description: Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes task-Objekt hat ein Detailobjekt.
ms.openlocfilehash: 74ba1c5b7c607f30253463e6cfc256fd3119bf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019818"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="ed7fd-104">plannerTaskDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ed7fd-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="ed7fd-p102">Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="ed7fd-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="ed7fd-107">Methods</span></span>

| <span data-ttu-id="ed7fd-108">Methode</span><span class="sxs-lookup"><span data-stu-id="ed7fd-108">Method</span></span>           | <span data-ttu-id="ed7fd-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ed7fd-109">Return Type</span></span>    |<span data-ttu-id="ed7fd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed7fd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed7fd-111">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="ed7fd-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="ed7fd-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="ed7fd-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="ed7fd-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="ed7fd-114">Update</span><span class="sxs-lookup"><span data-stu-id="ed7fd-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="ed7fd-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="ed7fd-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="ed7fd-116">Dient zum Aktualisieren des **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed7fd-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed7fd-117">Properties</span></span>
| <span data-ttu-id="ed7fd-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed7fd-118">Property</span></span>     | <span data-ttu-id="ed7fd-119">Typ</span><span class="sxs-lookup"><span data-stu-id="ed7fd-119">Type</span></span>   |<span data-ttu-id="ed7fd-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed7fd-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed7fd-121">checklist</span><span class="sxs-lookup"><span data-stu-id="ed7fd-121">checklist</span></span>|[<span data-ttu-id="ed7fd-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="ed7fd-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="ed7fd-123">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="ed7fd-124">description</span><span class="sxs-lookup"><span data-stu-id="ed7fd-124">description</span></span>|<span data-ttu-id="ed7fd-125">String</span><span class="sxs-lookup"><span data-stu-id="ed7fd-125">String</span></span>|<span data-ttu-id="ed7fd-126">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-126">Description of the task</span></span>|
|<span data-ttu-id="ed7fd-127">id</span><span class="sxs-lookup"><span data-stu-id="ed7fd-127">id</span></span>|<span data-ttu-id="ed7fd-128">String</span><span class="sxs-lookup"><span data-stu-id="ed7fd-128">String</span></span>| <span data-ttu-id="ed7fd-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-129">Read-only.</span></span> <span data-ttu-id="ed7fd-130">ID des die Aufgabendetails.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-130">ID of the task details.</span></span> <span data-ttu-id="ed7fd-131">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ed7fd-132">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ed7fd-133">previewType</span><span class="sxs-lookup"><span data-stu-id="ed7fd-133">previewType</span></span>|<span data-ttu-id="ed7fd-134">string</span><span class="sxs-lookup"><span data-stu-id="ed7fd-134">string</span></span>|<span data-ttu-id="ed7fd-135">Hierdurch wird den Typ der Vorschau, die für den Vorgang wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="ed7fd-136">Die möglichen Werte sind: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="ed7fd-137">Bei Festlegung auf `automatic` die angezeigte Vorschau wird von der app anzeigen den Vorgang ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="ed7fd-138">references</span><span class="sxs-lookup"><span data-stu-id="ed7fd-138">references</span></span>|[<span data-ttu-id="ed7fd-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="ed7fd-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="ed7fd-140">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed7fd-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ed7fd-141">Relationships</span></span>
<span data-ttu-id="ed7fd-142">Keine</span><span class="sxs-lookup"><span data-stu-id="ed7fd-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed7fd-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ed7fd-143">JSON representation</span></span>
<span data-ttu-id="ed7fd-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ed7fd-144">Here is a JSON representation of the resource.</span></span>

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

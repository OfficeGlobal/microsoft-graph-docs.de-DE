---
title: plannerTaskDetails-Ressourcentyp
description: Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes task-Objekt hat ein Detailobjekt.
ms.openlocfilehash: 3d5ab0b3a2f0c2e6c1abf284d5a87c2726c7aa15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066002"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="0c3bf-104">plannerTaskDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0c3bf-104">plannerTaskDetails resource type</span></span>

> <span data-ttu-id="0c3bf-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c3bf-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c3bf-p103">Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-p103">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="0c3bf-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="0c3bf-109">Methods</span></span>

| <span data-ttu-id="0c3bf-110">Methode</span><span class="sxs-lookup"><span data-stu-id="0c3bf-110">Method</span></span>           | <span data-ttu-id="0c3bf-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0c3bf-111">Return Type</span></span>    |<span data-ttu-id="0c3bf-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c3bf-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c3bf-113">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="0c3bf-113">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="0c3bf-114">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0c3bf-114">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="0c3bf-115">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="0c3bf-116">Update</span><span class="sxs-lookup"><span data-stu-id="0c3bf-116">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="0c3bf-117">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0c3bf-117">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="0c3bf-118">Dient zum Aktualisieren des **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-118">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c3bf-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0c3bf-119">Properties</span></span>
| <span data-ttu-id="0c3bf-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c3bf-120">Property</span></span>     | <span data-ttu-id="0c3bf-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0c3bf-121">Type</span></span>   |<span data-ttu-id="0c3bf-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c3bf-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c3bf-123">checklist</span><span class="sxs-lookup"><span data-stu-id="0c3bf-123">checklist</span></span>|[<span data-ttu-id="0c3bf-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="0c3bf-124">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="0c3bf-125">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="0c3bf-126">description</span><span class="sxs-lookup"><span data-stu-id="0c3bf-126">description</span></span>|<span data-ttu-id="0c3bf-127">String</span><span class="sxs-lookup"><span data-stu-id="0c3bf-127">String</span></span>|<span data-ttu-id="0c3bf-128">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-128">Description of the task</span></span>|
|<span data-ttu-id="0c3bf-129">id</span><span class="sxs-lookup"><span data-stu-id="0c3bf-129">id</span></span>|<span data-ttu-id="0c3bf-130">String</span><span class="sxs-lookup"><span data-stu-id="0c3bf-130">String</span></span>| <span data-ttu-id="0c3bf-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-131">Read-only.</span></span> <span data-ttu-id="0c3bf-132">ID des die Aufgabendetails.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-132">ID of the task details.</span></span> <span data-ttu-id="0c3bf-133">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-133">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0c3bf-134">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-134">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="0c3bf-135">previewType</span><span class="sxs-lookup"><span data-stu-id="0c3bf-135">previewType</span></span>|<span data-ttu-id="0c3bf-136">string</span><span class="sxs-lookup"><span data-stu-id="0c3bf-136">string</span></span>|<span data-ttu-id="0c3bf-p105">Hierdurch wird der Typ der Vorschau festgelegt, die für die Aufgabe angezeigt wird. Mögliche Werte: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, mit der die Aufgabe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="0c3bf-140">references</span><span class="sxs-lookup"><span data-stu-id="0c3bf-140">references</span></span>|[<span data-ttu-id="0c3bf-141">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="0c3bf-141">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="0c3bf-142">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-142">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c3bf-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0c3bf-143">Relationships</span></span>
<span data-ttu-id="0c3bf-144">Keine</span><span class="sxs-lookup"><span data-stu-id="0c3bf-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0c3bf-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0c3bf-145">JSON representation</span></span>
<span data-ttu-id="0c3bf-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0c3bf-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
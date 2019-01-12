---
title: plannerTaskDetails-Ressourcentyp
description: Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes task-Objekt hat ein Detailobjekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84b7191822be56e881b31d99503fdcdc4097890c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941142"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="37f41-104">plannerTaskDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="37f41-104">plannerTaskDetails resource type</span></span>

> <span data-ttu-id="37f41-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="37f41-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37f41-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37f41-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37f41-p103">Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="37f41-p103">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="37f41-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="37f41-109">Methods</span></span>

| <span data-ttu-id="37f41-110">Methode</span><span class="sxs-lookup"><span data-stu-id="37f41-110">Method</span></span>           | <span data-ttu-id="37f41-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="37f41-111">Return Type</span></span>    |<span data-ttu-id="37f41-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37f41-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37f41-113">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="37f41-113">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="37f41-114">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="37f41-114">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="37f41-115">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="37f41-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="37f41-116">Update</span><span class="sxs-lookup"><span data-stu-id="37f41-116">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="37f41-117">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="37f41-117">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="37f41-118">Dient zum Aktualisieren des **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="37f41-118">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="37f41-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="37f41-119">Properties</span></span>
| <span data-ttu-id="37f41-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37f41-120">Property</span></span>     | <span data-ttu-id="37f41-121">Typ</span><span class="sxs-lookup"><span data-stu-id="37f41-121">Type</span></span>   |<span data-ttu-id="37f41-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37f41-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37f41-123">checklist</span><span class="sxs-lookup"><span data-stu-id="37f41-123">checklist</span></span>|[<span data-ttu-id="37f41-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="37f41-124">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="37f41-125">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="37f41-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="37f41-126">description</span><span class="sxs-lookup"><span data-stu-id="37f41-126">description</span></span>|<span data-ttu-id="37f41-127">String</span><span class="sxs-lookup"><span data-stu-id="37f41-127">String</span></span>|<span data-ttu-id="37f41-128">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="37f41-128">Description of the task</span></span>|
|<span data-ttu-id="37f41-129">id</span><span class="sxs-lookup"><span data-stu-id="37f41-129">id</span></span>|<span data-ttu-id="37f41-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f41-130">String</span></span>| <span data-ttu-id="37f41-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="37f41-131">Read-only.</span></span> <span data-ttu-id="37f41-132">ID des die Aufgabendetails.</span><span class="sxs-lookup"><span data-stu-id="37f41-132">ID of the task details.</span></span> <span data-ttu-id="37f41-133">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="37f41-133">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="37f41-134">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="37f41-134">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="37f41-135">previewType</span><span class="sxs-lookup"><span data-stu-id="37f41-135">previewType</span></span>|<span data-ttu-id="37f41-136">string</span><span class="sxs-lookup"><span data-stu-id="37f41-136">string</span></span>|<span data-ttu-id="37f41-p105">Hierdurch wird der Typ der Vorschau festgelegt, die für die Aufgabe angezeigt wird. Mögliche Werte: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, mit der die Aufgabe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="37f41-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="37f41-140">references</span><span class="sxs-lookup"><span data-stu-id="37f41-140">references</span></span>|[<span data-ttu-id="37f41-141">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="37f41-141">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="37f41-142">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="37f41-142">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37f41-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="37f41-143">Relationships</span></span>
<span data-ttu-id="37f41-144">Keine</span><span class="sxs-lookup"><span data-stu-id="37f41-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="37f41-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="37f41-145">JSON representation</span></span>
<span data-ttu-id="37f41-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="37f41-146">Here is a JSON representation of the resource.</span></span>

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

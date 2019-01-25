---
title: plannerTaskDetails-Ressourcentyp
description: Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes task-Objekt hat ein Detailobjekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512311"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="6dbc0-104">plannerTaskDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6dbc0-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dbc0-p102">Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="6dbc0-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="6dbc0-107">Methods</span></span>

| <span data-ttu-id="6dbc0-108">Methode</span><span class="sxs-lookup"><span data-stu-id="6dbc0-108">Method</span></span>           | <span data-ttu-id="6dbc0-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6dbc0-109">Return Type</span></span>    |<span data-ttu-id="6dbc0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6dbc0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6dbc0-111">plannerTaskDetails abrufen</span><span class="sxs-lookup"><span data-stu-id="6dbc0-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="6dbc0-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6dbc0-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="6dbc0-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="6dbc0-114">Update</span><span class="sxs-lookup"><span data-stu-id="6dbc0-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="6dbc0-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6dbc0-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="6dbc0-116">Dient zum Aktualisieren des **plannerTaskDetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6dbc0-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6dbc0-117">Properties</span></span>
| <span data-ttu-id="6dbc0-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6dbc0-118">Property</span></span>     | <span data-ttu-id="6dbc0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="6dbc0-119">Type</span></span>   |<span data-ttu-id="6dbc0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6dbc0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dbc0-121">checklist</span><span class="sxs-lookup"><span data-stu-id="6dbc0-121">checklist</span></span>|[<span data-ttu-id="6dbc0-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="6dbc0-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="6dbc0-123">Die Sammlung von Checklistenelementen für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="6dbc0-124">description</span><span class="sxs-lookup"><span data-stu-id="6dbc0-124">description</span></span>|<span data-ttu-id="6dbc0-125">String</span><span class="sxs-lookup"><span data-stu-id="6dbc0-125">String</span></span>|<span data-ttu-id="6dbc0-126">Beschreibung der Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-126">Description of the task</span></span>|
|<span data-ttu-id="6dbc0-127">id</span><span class="sxs-lookup"><span data-stu-id="6dbc0-127">id</span></span>|<span data-ttu-id="6dbc0-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6dbc0-128">String</span></span>| <span data-ttu-id="6dbc0-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-129">Read-only.</span></span> <span data-ttu-id="6dbc0-130">ID des die Aufgabendetails.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-130">ID of the task details.</span></span> <span data-ttu-id="6dbc0-131">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="6dbc0-132">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6dbc0-133">previewType</span><span class="sxs-lookup"><span data-stu-id="6dbc0-133">previewType</span></span>|<span data-ttu-id="6dbc0-134">string</span><span class="sxs-lookup"><span data-stu-id="6dbc0-134">string</span></span>|<span data-ttu-id="6dbc0-p104">Hierdurch wird der Typ der Vorschau festgelegt, die für die Aufgabe angezeigt wird. Mögliche Werte: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, mit der die Aufgabe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="6dbc0-138">references</span><span class="sxs-lookup"><span data-stu-id="6dbc0-138">references</span></span>|[<span data-ttu-id="6dbc0-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="6dbc0-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="6dbc0-140">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dbc0-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6dbc0-141">Relationships</span></span>
<span data-ttu-id="6dbc0-142">Keine</span><span class="sxs-lookup"><span data-stu-id="6dbc0-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6dbc0-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6dbc0-143">JSON representation</span></span>
<span data-ttu-id="6dbc0-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6dbc0-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertaskdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

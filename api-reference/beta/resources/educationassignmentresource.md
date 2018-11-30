---
title: Ressourcentyp educationAssignmentResource
description: Ein Wrapperobjekt, die Ressourcen, die einer Zuordnung zugeordnet speichert. Der Wrapper fügt die Eigenschaft **DistributeForStudentWork** hinzu und gibt an, dass diese Ressource wird
ms.openlocfilehash: 6907af5e4408248487b118c390bb2ec209700124
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062224"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="35391-104">Ressourcentyp educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="35391-104">educationAssignmentResource resource type</span></span>

> <span data-ttu-id="35391-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="35391-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35391-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35391-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35391-107">Ein Wrapperobjekt, die Ressourcen, die einer Zuordnung zugeordnet speichert.</span><span class="sxs-lookup"><span data-stu-id="35391-107">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="35391-108">Der Wrapper fügt die Eigenschaft **DistributeForStudentWork** hinzu und gibt an, dass diese Ressource in der Studentenübermittlung kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="35391-108">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="35391-109">Wenn das Objekt nicht kopiert wird, sehen Studenten einen Link zu der Ressource für die Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="35391-109">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="35391-110">Die Student möglich so aktualisieren Sie diese Ressource nicht.</span><span class="sxs-lookup"><span data-stu-id="35391-110">The student will not be able to update this resource.</span></span> <span data-ttu-id="35391-111">Hierbei handelt es sich um Handzetteln aus der Schulungsleiter in den Teilnehmern nothing in aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="35391-111">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="35391-112">Wenn die Ressource verteilt ist, erhält jeder Student eine Kopie dieser Ressource in der Ressourcenliste ihrer Einreichung.</span><span class="sxs-lookup"><span data-stu-id="35391-112">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="35391-113">Studenten werden ihre Kopie ändern und zur Benotung übermitteln können.</span><span class="sxs-lookup"><span data-stu-id="35391-113">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="35391-114">Methoden</span><span class="sxs-lookup"><span data-stu-id="35391-114">Methods</span></span>

| <span data-ttu-id="35391-115">Methode</span><span class="sxs-lookup"><span data-stu-id="35391-115">Method</span></span>           | <span data-ttu-id="35391-116">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="35391-116">Return Type</span></span>    |<span data-ttu-id="35391-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35391-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35391-118">Abrufen von educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="35391-118">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="35391-119">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="35391-119">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="35391-120">Lesen Sie Eigenschaften und die Beziehungen eines **EducationAssignmentResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="35391-120">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="35391-121">Update</span><span class="sxs-lookup"><span data-stu-id="35391-121">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="35391-122">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="35391-122">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="35391-123">Aktualisieren eines **EducationAssignmentResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="35391-123">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="35391-124">Delete</span><span class="sxs-lookup"><span data-stu-id="35391-124">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="35391-125">Keine</span><span class="sxs-lookup"><span data-stu-id="35391-125">None</span></span> |<span data-ttu-id="35391-126">Löschen eines **EducationAssignmentResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="35391-126">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="35391-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35391-127">Properties</span></span>
| <span data-ttu-id="35391-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35391-128">Property</span></span>     | <span data-ttu-id="35391-129">Typ</span><span class="sxs-lookup"><span data-stu-id="35391-129">Type</span></span>   |<span data-ttu-id="35391-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35391-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35391-131">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="35391-131">distributeForStudentWork</span></span>|<span data-ttu-id="35391-132">Boolesch</span><span class="sxs-lookup"><span data-stu-id="35391-132">Boolean</span></span>|<span data-ttu-id="35391-133">Gibt an, ob diese Ressource in jeder Studentenübermittlung für Änderung und Übermittlung kopiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="35391-133">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="35391-134">id</span><span class="sxs-lookup"><span data-stu-id="35391-134">id</span></span>|<span data-ttu-id="35391-135">String</span><span class="sxs-lookup"><span data-stu-id="35391-135">String</span></span>| <span data-ttu-id="35391-136">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35391-136">ID of this resource.</span></span> <span data-ttu-id="35391-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35391-137">Read-only.</span></span>|
|<span data-ttu-id="35391-138">resource</span><span class="sxs-lookup"><span data-stu-id="35391-138">resource</span></span>|[<span data-ttu-id="35391-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="35391-139">educationResource</span></span>](educationresource.md)|<span data-ttu-id="35391-140">Resource-Objekt, das diese Zuordnung zugeordnet wurde.</span><span class="sxs-lookup"><span data-stu-id="35391-140">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35391-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="35391-141">Relationships</span></span>
<span data-ttu-id="35391-142">Keine.</span><span class="sxs-lookup"><span data-stu-id="35391-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="35391-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35391-143">JSON representation</span></span>

<span data-ttu-id="35391-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35391-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

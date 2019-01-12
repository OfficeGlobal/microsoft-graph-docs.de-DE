---
title: Ressourcentyp educationAssignmentResource
description: Ein Wrapperobjekt, die Ressourcen, die einer Zuordnung zugeordnet speichert. Der Wrapper fügt die Eigenschaft **DistributeForStudentWork** hinzu und gibt an, dass diese Ressource wird
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb0879737d0375bf2463268fe29f2c98f2b6ed51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991349"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="5c5c9-104">Ressourcentyp educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="5c5c9-104">educationAssignmentResource resource type</span></span>

> <span data-ttu-id="5c5c9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c5c9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c5c9-107">Ein Wrapperobjekt, die Ressourcen, die einer Zuordnung zugeordnet speichert.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-107">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="5c5c9-108">Der Wrapper fügt die Eigenschaft **DistributeForStudentWork** hinzu und gibt an, dass diese Ressource in der Studentenübermittlung kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-108">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="5c5c9-109">Wenn das Objekt nicht kopiert wird, sehen Studenten einen Link zu der Ressource für die Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-109">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="5c5c9-110">Die Student möglich so aktualisieren Sie diese Ressource nicht.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-110">The student will not be able to update this resource.</span></span> <span data-ttu-id="5c5c9-111">Hierbei handelt es sich um Handzetteln aus der Schulungsleiter in den Teilnehmern nothing in aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-111">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="5c5c9-112">Wenn die Ressource verteilt ist, erhält jeder Student eine Kopie dieser Ressource in der Ressourcenliste ihrer Einreichung.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-112">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="5c5c9-113">Studenten werden ihre Kopie ändern und zur Benotung übermitteln können.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-113">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="5c5c9-114">Methoden</span><span class="sxs-lookup"><span data-stu-id="5c5c9-114">Methods</span></span>

| <span data-ttu-id="5c5c9-115">Methode</span><span class="sxs-lookup"><span data-stu-id="5c5c9-115">Method</span></span>           | <span data-ttu-id="5c5c9-116">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5c5c9-116">Return Type</span></span>    |<span data-ttu-id="5c5c9-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c5c9-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c5c9-118">Abrufen von educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="5c5c9-118">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="5c5c9-119">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="5c5c9-119">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="5c5c9-120">Lesen Sie Eigenschaften und die Beziehungen eines **EducationAssignmentResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-120">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="5c5c9-121">Update</span><span class="sxs-lookup"><span data-stu-id="5c5c9-121">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="5c5c9-122">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="5c5c9-122">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="5c5c9-123">Aktualisieren eines **EducationAssignmentResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-123">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="5c5c9-124">Delete</span><span class="sxs-lookup"><span data-stu-id="5c5c9-124">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="5c5c9-125">Keine</span><span class="sxs-lookup"><span data-stu-id="5c5c9-125">None</span></span> |<span data-ttu-id="5c5c9-126">Löschen eines **EducationAssignmentResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-126">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5c5c9-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5c5c9-127">Properties</span></span>
| <span data-ttu-id="5c5c9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c5c9-128">Property</span></span>     | <span data-ttu-id="5c5c9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5c5c9-129">Type</span></span>   |<span data-ttu-id="5c5c9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c5c9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c5c9-131">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="5c5c9-131">distributeForStudentWork</span></span>|<span data-ttu-id="5c5c9-132">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5c5c9-132">Boolean</span></span>|<span data-ttu-id="5c5c9-133">Gibt an, ob diese Ressource in jeder Studentenübermittlung für Änderung und Übermittlung kopiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-133">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="5c5c9-134">id</span><span class="sxs-lookup"><span data-stu-id="5c5c9-134">id</span></span>|<span data-ttu-id="5c5c9-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c5c9-135">String</span></span>| <span data-ttu-id="5c5c9-136">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-136">ID of this resource.</span></span> <span data-ttu-id="5c5c9-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-137">Read-only.</span></span>|
|<span data-ttu-id="5c5c9-138">resource</span><span class="sxs-lookup"><span data-stu-id="5c5c9-138">resource</span></span>|[<span data-ttu-id="5c5c9-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="5c5c9-139">educationResource</span></span>](educationresource.md)|<span data-ttu-id="5c5c9-140">Resource-Objekt, das diese Zuordnung zugeordnet wurde.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-140">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c5c9-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5c5c9-141">Relationships</span></span>
<span data-ttu-id="5c5c9-142">Keine.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5c5c9-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5c5c9-143">JSON representation</span></span>

<span data-ttu-id="5c5c9-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5c5c9-144">The following is a JSON representation of the resource.</span></span>

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

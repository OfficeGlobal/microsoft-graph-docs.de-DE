---
title: Ressourcentyp educationSubmissionResource
description: 'Ein Wrapper für eine Ressource für die Verwendung einer Übermittlung. Der Wrapper wird die Zuordnung Ressource einen Zeiger hinzugefügt, sofern dies in der Zuweisung kopiert wurde.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef231de49d3871ec877c279b4e77585343e1a85e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522077"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="491a7-104">Ressourcentyp educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="491a7-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="491a7-105">Ein Wrapper für eine Ressource für die Verwendung einer Übermittlung.</span><span class="sxs-lookup"><span data-stu-id="491a7-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="491a7-106">Der Wrapper wird die Zuordnung Ressource einen Zeiger hinzugefügt, sofern dies in der Zuweisung kopiert wurde.</span><span class="sxs-lookup"><span data-stu-id="491a7-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="491a7-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="491a7-107">Methods</span></span>

| <span data-ttu-id="491a7-108">Methode</span><span class="sxs-lookup"><span data-stu-id="491a7-108">Method</span></span>           | <span data-ttu-id="491a7-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="491a7-109">Return Type</span></span>    |<span data-ttu-id="491a7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="491a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="491a7-111">Abrufen von educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="491a7-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="491a7-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="491a7-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="491a7-113">Lesen Sie Eigenschaften und die Beziehungen eines **EducationSubmissionResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="491a7-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="491a7-114">Delete</span><span class="sxs-lookup"><span data-stu-id="491a7-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="491a7-115">Keine</span><span class="sxs-lookup"><span data-stu-id="491a7-115">None</span></span> |<span data-ttu-id="491a7-116">Löschen eines **EducationSubmissionResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="491a7-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="491a7-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="491a7-117">Properties</span></span>
| <span data-ttu-id="491a7-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="491a7-118">Property</span></span>     | <span data-ttu-id="491a7-119">Typ</span><span class="sxs-lookup"><span data-stu-id="491a7-119">Type</span></span>   |<span data-ttu-id="491a7-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="491a7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="491a7-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="491a7-121">assignmentResourceUrl</span></span>|<span data-ttu-id="491a7-122">String</span><span class="sxs-lookup"><span data-stu-id="491a7-122">String</span></span>|<span data-ttu-id="491a7-123">Zeiger auf die Zuordnung aus der diese Ressource kopiert wurden.</span><span class="sxs-lookup"><span data-stu-id="491a7-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="491a7-124">Wenn dies null ist, hochgeladen Student die Ressource.</span><span class="sxs-lookup"><span data-stu-id="491a7-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="491a7-125">id</span><span class="sxs-lookup"><span data-stu-id="491a7-125">id</span></span>|<span data-ttu-id="491a7-126">String</span><span class="sxs-lookup"><span data-stu-id="491a7-126">String</span></span>| <span data-ttu-id="491a7-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="491a7-127">Read-only.</span></span>|
|<span data-ttu-id="491a7-128">resource</span><span class="sxs-lookup"><span data-stu-id="491a7-128">resource</span></span>|[<span data-ttu-id="491a7-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="491a7-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="491a7-130">Resource-Objekt</span><span class="sxs-lookup"><span data-stu-id="491a7-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="491a7-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="491a7-131">Relationships</span></span>
<span data-ttu-id="491a7-132">Keine</span><span class="sxs-lookup"><span data-stu-id="491a7-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="491a7-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="491a7-133">JSON representation</span></span>

<span data-ttu-id="491a7-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="491a7-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

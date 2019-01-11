---
title: Ressourcentyp educationSubmissionResource
description: 'Ein Wrapper für eine Ressource für die Verwendung einer Übermittlung. Der Wrapper wird die Zuordnung Ressource einen Zeiger hinzugefügt, sofern dies in der Zuweisung kopiert wurde.  '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 8703072fccb77a2577db6ce0717647e79a47fdc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875985"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="d4271-104">Ressourcentyp educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d4271-104">educationSubmissionResource resource type</span></span>

> <span data-ttu-id="d4271-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d4271-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4271-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4271-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4271-107">Ein Wrapper für eine Ressource für die Verwendung einer Übermittlung.</span><span class="sxs-lookup"><span data-stu-id="d4271-107">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="d4271-108">Der Wrapper wird die Zuordnung Ressource einen Zeiger hinzugefügt, sofern dies in der Zuweisung kopiert wurde.</span><span class="sxs-lookup"><span data-stu-id="d4271-108">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="d4271-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="d4271-109">Methods</span></span>

| <span data-ttu-id="d4271-110">Methode</span><span class="sxs-lookup"><span data-stu-id="d4271-110">Method</span></span>           | <span data-ttu-id="d4271-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d4271-111">Return Type</span></span>    |<span data-ttu-id="d4271-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4271-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4271-113">Abrufen von educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d4271-113">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="d4271-114">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d4271-114">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="d4271-115">Lesen Sie Eigenschaften und die Beziehungen eines **EducationSubmissionResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4271-115">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="d4271-116">Delete</span><span class="sxs-lookup"><span data-stu-id="d4271-116">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="d4271-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d4271-117">None</span></span> |<span data-ttu-id="d4271-118">Löschen eines **EducationSubmissionResource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4271-118">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4271-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4271-119">Properties</span></span>
| <span data-ttu-id="d4271-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4271-120">Property</span></span>     | <span data-ttu-id="d4271-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d4271-121">Type</span></span>   |<span data-ttu-id="d4271-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4271-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4271-123">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="d4271-123">assignmentResourceUrl</span></span>|<span data-ttu-id="d4271-124">String</span><span class="sxs-lookup"><span data-stu-id="d4271-124">String</span></span>|<span data-ttu-id="d4271-125">Zeiger auf die Zuordnung aus der diese Ressource kopiert wurden.</span><span class="sxs-lookup"><span data-stu-id="d4271-125">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="d4271-126">Wenn dies null ist, hochgeladen Student die Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4271-126">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="d4271-127">id</span><span class="sxs-lookup"><span data-stu-id="d4271-127">id</span></span>|<span data-ttu-id="d4271-128">String</span><span class="sxs-lookup"><span data-stu-id="d4271-128">String</span></span>| <span data-ttu-id="d4271-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4271-129">Read-only.</span></span>|
|<span data-ttu-id="d4271-130">resource</span><span class="sxs-lookup"><span data-stu-id="d4271-130">resource</span></span>|[<span data-ttu-id="d4271-131">educationResource</span><span class="sxs-lookup"><span data-stu-id="d4271-131">educationResource</span></span>](educationresource.md)|<span data-ttu-id="d4271-132">Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d4271-132">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4271-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4271-133">Relationships</span></span>
<span data-ttu-id="d4271-134">Keine</span><span class="sxs-lookup"><span data-stu-id="d4271-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d4271-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4271-135">JSON representation</span></span>

<span data-ttu-id="d4271-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4271-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

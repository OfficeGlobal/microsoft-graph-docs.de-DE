---
title: educationCategory-Ressourcentyp
description: Eine Kategorie, die auf Zuordnungen angewendet werden kann.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 928f37b4d29a4443c947bd92bf4a71f9f8a05f59
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801000"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="01c47-103">educationCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="01c47-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01c47-104">Eine Kategorie, die auf Zuordnungen angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="01c47-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="01c47-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="01c47-105">Methods</span></span>

| <span data-ttu-id="01c47-106">Methode</span><span class="sxs-lookup"><span data-stu-id="01c47-106">Method</span></span>           | <span data-ttu-id="01c47-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="01c47-107">Return Type</span></span>    |<span data-ttu-id="01c47-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01c47-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01c47-109">EducationCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="01c47-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="01c47-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="01c47-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="01c47-111">Abrufen einer vorhandenen **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="01c47-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="01c47-112">Kategorie löschen</span><span class="sxs-lookup"><span data-stu-id="01c47-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="01c47-113">Keines</span><span class="sxs-lookup"><span data-stu-id="01c47-113">None</span></span> | <span data-ttu-id="01c47-114">Entfernen einer **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="01c47-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="01c47-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="01c47-115">Properties</span></span>
| <span data-ttu-id="01c47-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01c47-116">Property</span></span>     | <span data-ttu-id="01c47-117">Typ</span><span class="sxs-lookup"><span data-stu-id="01c47-117">Type</span></span>   |<span data-ttu-id="01c47-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01c47-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01c47-119">id</span><span class="sxs-lookup"><span data-stu-id="01c47-119">id</span></span>|<span data-ttu-id="01c47-120">String</span><span class="sxs-lookup"><span data-stu-id="01c47-120">String</span></span>|<span data-ttu-id="01c47-121">Eindeutiger Bezeichner für die Kategorie.</span><span class="sxs-lookup"><span data-stu-id="01c47-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="01c47-122">displayName</span><span class="sxs-lookup"><span data-stu-id="01c47-122">displayName</span></span>|<span data-ttu-id="01c47-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01c47-123">String</span></span>|<span data-ttu-id="01c47-124">Eindeutiger Bezeichner für die Kategorie.</span><span class="sxs-lookup"><span data-stu-id="01c47-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01c47-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="01c47-125">JSON representation</span></span>

<span data-ttu-id="01c47-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="01c47-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcategory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

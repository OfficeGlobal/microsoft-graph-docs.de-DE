---
title: Ressourcentyp educationLinkResource
description: Eine Unterklasse der EducationResource. Diese Ressource ist ein Link, und ist nicht haben zusätzlichen Daten zugeordnet.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 09e7c7c5070d6f8f288dbf18d6fb9ce81b456092
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516959"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="aebf5-104">Ressourcentyp educationLinkResource</span><span class="sxs-lookup"><span data-stu-id="aebf5-104">educationLinkResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aebf5-105">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="aebf5-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="aebf5-106">Diese Ressource ist ein Link, und ist nicht haben zusätzlichen Daten zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="aebf5-106">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="aebf5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aebf5-107">Properties</span></span>
| <span data-ttu-id="aebf5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aebf5-108">Property</span></span>     | <span data-ttu-id="aebf5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="aebf5-109">Type</span></span>   |<span data-ttu-id="aebf5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aebf5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aebf5-111">Link</span><span class="sxs-lookup"><span data-stu-id="aebf5-111">link</span></span>|<span data-ttu-id="aebf5-112">String</span><span class="sxs-lookup"><span data-stu-id="aebf5-112">String</span></span>|<span data-ttu-id="aebf5-113">URL für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="aebf5-113">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aebf5-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aebf5-114">JSON representation</span></span>

<span data-ttu-id="aebf5-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aebf5-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationlinkresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

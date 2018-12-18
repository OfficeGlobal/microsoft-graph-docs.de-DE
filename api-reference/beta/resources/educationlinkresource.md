---
title: Ressourcentyp educationLinkResource
description: Eine Unterklasse der EducationResource. Diese Ressource ist ein Link, und ist nicht haben zusätzlichen Daten zugeordnet.
author: mmast-msft
ms.openlocfilehash: 02a55eeea25ab2c27d6c5848fbc178ff535d5e33
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349804"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="1210d-104">Ressourcentyp educationLinkResource</span><span class="sxs-lookup"><span data-stu-id="1210d-104">educationLinkResource resource type</span></span>

> <span data-ttu-id="1210d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1210d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1210d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1210d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1210d-107">Eine Unterklasse der [EducationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="1210d-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="1210d-108">Diese Ressource ist ein Link, und ist nicht haben zusätzlichen Daten zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1210d-108">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="1210d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1210d-109">Properties</span></span>
| <span data-ttu-id="1210d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1210d-110">Property</span></span>     | <span data-ttu-id="1210d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1210d-111">Type</span></span>   |<span data-ttu-id="1210d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1210d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1210d-113">Link</span><span class="sxs-lookup"><span data-stu-id="1210d-113">link</span></span>|<span data-ttu-id="1210d-114">String</span><span class="sxs-lookup"><span data-stu-id="1210d-114">String</span></span>|<span data-ttu-id="1210d-115">URL für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="1210d-115">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1210d-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1210d-116">JSON representation</span></span>

<span data-ttu-id="1210d-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1210d-117">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: personType-Ressourcentyp
description: Stellt den Typ der Person dar.
localization_priority: Normal
ms.openlocfilehash: d30441a9eab3f51b63e31e5c3c627444312449ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831493"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="af055-103">personType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="af055-103">personType resource type</span></span>

<span data-ttu-id="af055-104">Stellt den Typ der Person dar.</span><span class="sxs-lookup"><span data-stu-id="af055-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="af055-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="af055-105">JSON representation</span></span>

<span data-ttu-id="af055-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="af055-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="af055-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="af055-107">Properties</span></span>
| <span data-ttu-id="af055-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af055-108">Property</span></span>     | <span data-ttu-id="af055-109">Typ</span><span class="sxs-lookup"><span data-stu-id="af055-109">Type</span></span>   |<span data-ttu-id="af055-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af055-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af055-111">class</span><span class="sxs-lookup"><span data-stu-id="af055-111">class</span></span>|<span data-ttu-id="af055-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af055-112">String</span></span>|<span data-ttu-id="af055-113">Der Typ der Datenquelle, z. B. Person.</span><span class="sxs-lookup"><span data-stu-id="af055-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="af055-114">subclass</span><span class="sxs-lookup"><span data-stu-id="af055-114">subclass</span></span>|<span data-ttu-id="af055-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af055-115">String</span></span>|<span data-ttu-id="af055-116">Der sekundäre Typ der Datenquelle, z. B. OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="af055-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

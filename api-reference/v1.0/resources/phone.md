---
title: phone-Ressourcentyp
description: Gibt eine Telefonnummer an.
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805061"
---
# <a name="phone-resource-type"></a><span data-ttu-id="cc620-103">phone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cc620-103">phone resource type</span></span>

<span data-ttu-id="cc620-104">Gibt eine Telefonnummer an.</span><span class="sxs-lookup"><span data-stu-id="cc620-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="cc620-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cc620-105">Properties</span></span>
| <span data-ttu-id="cc620-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cc620-106">Property</span></span>     | <span data-ttu-id="cc620-107">Typ</span><span class="sxs-lookup"><span data-stu-id="cc620-107">Type</span></span>   |<span data-ttu-id="cc620-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc620-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc620-109">number</span><span class="sxs-lookup"><span data-stu-id="cc620-109">number</span></span>|<span data-ttu-id="cc620-110">string</span><span class="sxs-lookup"><span data-stu-id="cc620-110">string</span></span>|<span data-ttu-id="cc620-111">Die Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="cc620-111">The phone number.</span></span>|
|<span data-ttu-id="cc620-112">type</span><span class="sxs-lookup"><span data-stu-id="cc620-112">type</span></span>|<span data-ttu-id="cc620-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="cc620-113">phoneType</span></span>|<span data-ttu-id="cc620-114">Der Typ der Telefonnummer.</span><span class="sxs-lookup"><span data-stu-id="cc620-114">The type of phone number.</span></span> <span data-ttu-id="cc620-115">Die möglichen Werte sind: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="cc620-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc620-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cc620-116">JSON representation</span></span>

<span data-ttu-id="cc620-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cc620-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

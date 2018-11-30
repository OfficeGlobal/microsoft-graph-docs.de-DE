---
title: phone-Ressourcentyp
description: Gibt eine Telefonnummer an.
ms.openlocfilehash: 1293b1f84d9e73f5d92c9b6f6b078b5f39126e33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018997"
---
# <a name="phone-resource-type"></a><span data-ttu-id="2dce1-103">phone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2dce1-103">phone resource type</span></span>

<span data-ttu-id="2dce1-104">Gibt eine Telefonnummer an.</span><span class="sxs-lookup"><span data-stu-id="2dce1-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="2dce1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2dce1-105">Properties</span></span>
| <span data-ttu-id="2dce1-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2dce1-106">Property</span></span>     | <span data-ttu-id="2dce1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2dce1-107">Type</span></span>   |<span data-ttu-id="2dce1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dce1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dce1-109">number</span><span class="sxs-lookup"><span data-stu-id="2dce1-109">number</span></span>|<span data-ttu-id="2dce1-110">string</span><span class="sxs-lookup"><span data-stu-id="2dce1-110">string</span></span>|<span data-ttu-id="2dce1-111">Die Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="2dce1-111">The phone number.</span></span>|
|<span data-ttu-id="2dce1-112">type</span><span class="sxs-lookup"><span data-stu-id="2dce1-112">type</span></span>|<span data-ttu-id="2dce1-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="2dce1-113">phoneType</span></span>|<span data-ttu-id="2dce1-114">Der Typ der Telefonnummer.</span><span class="sxs-lookup"><span data-stu-id="2dce1-114">The type of phone number.</span></span> <span data-ttu-id="2dce1-115">Die möglichen Werte sind: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="2dce1-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dce1-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2dce1-116">JSON representation</span></span>

<span data-ttu-id="2dce1-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2dce1-117">Here is a JSON representation of the resource.</span></span>

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

---
title: phone-Ressourcentyp
description: Gibt eine Telefonnummer an.
ms.openlocfilehash: d47f2c36f9913eb75868077bdd5bb2d599055c59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058044"
---
# <a name="phone-resource-type"></a><span data-ttu-id="b4888-103">phone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b4888-103">phone resource type</span></span>

> <span data-ttu-id="b4888-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4888-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4888-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4888-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4888-106">Gibt eine Telefonnummer an.</span><span class="sxs-lookup"><span data-stu-id="b4888-106">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="b4888-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4888-107">Properties</span></span>
| <span data-ttu-id="b4888-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4888-108">Property</span></span>     | <span data-ttu-id="b4888-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b4888-109">Type</span></span>   |<span data-ttu-id="b4888-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4888-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4888-111">number</span><span class="sxs-lookup"><span data-stu-id="b4888-111">number</span></span>|<span data-ttu-id="b4888-112">string</span><span class="sxs-lookup"><span data-stu-id="b4888-112">string</span></span>|<span data-ttu-id="b4888-113">Die Telefonnummer</span><span class="sxs-lookup"><span data-stu-id="b4888-113">The phone number.</span></span>|
|<span data-ttu-id="b4888-114">type</span><span class="sxs-lookup"><span data-stu-id="b4888-114">type</span></span>|<span data-ttu-id="b4888-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4888-115">String</span></span>|<span data-ttu-id="b4888-p102">Der Typ der Telefonnummer. Mögliche Werte sind: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="b4888-p102">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4888-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4888-118">JSON representation</span></span>

<span data-ttu-id="b4888-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4888-119">Here is a JSON representation of the resource.</span></span>

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
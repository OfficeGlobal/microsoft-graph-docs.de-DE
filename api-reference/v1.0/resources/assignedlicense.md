---
title: assignedLicense-Ressourcentyp
description: Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der user-Entität ist eine Sammlung von **assignedLicense**.
ms.openlocfilehash: 48863a9acdcfa173a3f0c1a2a008516360ffdf9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017156"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="af0d4-104">assignedLicense-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="af0d4-104">assignedLicense resource type</span></span>

<span data-ttu-id="af0d4-p102">Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der [user](user.md)-Entität ist eine Sammlung von **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="af0d4-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="af0d4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="af0d4-107">Properties</span></span>
| <span data-ttu-id="af0d4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af0d4-108">Property</span></span>     | <span data-ttu-id="af0d4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="af0d4-109">Type</span></span>   |<span data-ttu-id="af0d4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af0d4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af0d4-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="af0d4-111">disabledPlans</span></span>|<span data-ttu-id="af0d4-112">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="af0d4-112">Guid collection</span></span>|<span data-ttu-id="af0d4-113">Eine Auflistung der eindeutigen Bezeichner für Pläne, die deaktiviert wurden.</span><span class="sxs-lookup"><span data-stu-id="af0d4-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="af0d4-114">skuId</span><span class="sxs-lookup"><span data-stu-id="af0d4-114">skuId</span></span>|<span data-ttu-id="af0d4-115">Guid</span><span class="sxs-lookup"><span data-stu-id="af0d4-115">Guid</span></span>|<span data-ttu-id="af0d4-116">Die eindeutige ID der SKU.</span><span class="sxs-lookup"><span data-stu-id="af0d4-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af0d4-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="af0d4-117">JSON representation</span></span>

<span data-ttu-id="af0d4-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="af0d4-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

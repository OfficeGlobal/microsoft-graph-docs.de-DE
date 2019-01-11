---
title: assignedLicense-Ressourcentyp
description: Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der user-Entität ist eine Sammlung von **assignedLicense**.
localization_priority: Normal
ms.openlocfilehash: 1e190060d0aafa4d494240f691b354b28e7697c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885344"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="ba90f-104">assignedLicense-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ba90f-104">assignedLicense resource type</span></span>

<span data-ttu-id="ba90f-p102">Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der [user](user.md)-Entität ist eine Sammlung von **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="ba90f-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="ba90f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ba90f-107">Properties</span></span>
| <span data-ttu-id="ba90f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba90f-108">Property</span></span>     | <span data-ttu-id="ba90f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ba90f-109">Type</span></span>   |<span data-ttu-id="ba90f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba90f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba90f-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="ba90f-111">disabledPlans</span></span>|<span data-ttu-id="ba90f-112">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ba90f-112">Guid collection</span></span>|<span data-ttu-id="ba90f-113">Eine Auflistung der eindeutigen Bezeichner für Pläne, die deaktiviert wurden.</span><span class="sxs-lookup"><span data-stu-id="ba90f-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="ba90f-114">skuId</span><span class="sxs-lookup"><span data-stu-id="ba90f-114">skuId</span></span>|<span data-ttu-id="ba90f-115">Guid</span><span class="sxs-lookup"><span data-stu-id="ba90f-115">Guid</span></span>|<span data-ttu-id="ba90f-116">Die eindeutige ID der SKU.</span><span class="sxs-lookup"><span data-stu-id="ba90f-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba90f-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ba90f-117">JSON representation</span></span>

<span data-ttu-id="ba90f-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ba90f-118">Here is a JSON representation of the resource</span></span>

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

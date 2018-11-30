---
title: assignedLicense-Ressourcentyp
description: Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der user-Entität ist eine Sammlung von **assignedLicense**.
ms.openlocfilehash: a41ece17882e6b85da009b4e29292e4b9a7965af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065454"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="e7e1d-104">assignedLicense-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e7e1d-104">assignedLicense resource type</span></span>

> <span data-ttu-id="e7e1d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e7e1d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7e1d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e7e1d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7e1d-p103">Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der [user](user.md)-Entität ist eine Sammlung von **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="e7e1d-p103">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="e7e1d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e7e1d-109">Properties</span></span>
| <span data-ttu-id="e7e1d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7e1d-110">Property</span></span>     | <span data-ttu-id="e7e1d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e7e1d-111">Type</span></span>   |<span data-ttu-id="e7e1d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7e1d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7e1d-113">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="e7e1d-113">disabledPlans</span></span>|<span data-ttu-id="e7e1d-114">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e7e1d-114">Guid collection</span></span>|<span data-ttu-id="e7e1d-115">Eine Auflistung der eindeutigen Bezeichner für Pläne, die deaktiviert wurden.</span><span class="sxs-lookup"><span data-stu-id="e7e1d-115">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="e7e1d-116">skuId</span><span class="sxs-lookup"><span data-stu-id="e7e1d-116">skuId</span></span>|<span data-ttu-id="e7e1d-117">Guid</span><span class="sxs-lookup"><span data-stu-id="e7e1d-117">Guid</span></span>|<span data-ttu-id="e7e1d-118">Die eindeutige ID der SKU.</span><span class="sxs-lookup"><span data-stu-id="e7e1d-118">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7e1d-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e7e1d-119">JSON representation</span></span>

<span data-ttu-id="e7e1d-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e7e1d-120">Here is a JSON representation of the resource</span></span>

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

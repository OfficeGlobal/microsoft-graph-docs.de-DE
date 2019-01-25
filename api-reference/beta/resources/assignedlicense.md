---
title: assignedLicense-Ressourcentyp
description: Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der **user**-Entität ist eine Sammlung von assignedLicense.
localization_priority: Normal
ms.openlocfilehash: 2d9620ec33a296c09ced9bc9d8af8d6d032bb7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524919"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="ad5ba-104">assignedLicense-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ad5ba-104">assignedLicense resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad5ba-p102">Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der [user](user.md)-Entität ist eine Sammlung von **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="ad5ba-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="ad5ba-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad5ba-107">Properties</span></span>
| <span data-ttu-id="ad5ba-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad5ba-108">Property</span></span>     | <span data-ttu-id="ad5ba-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ad5ba-109">Type</span></span>   |<span data-ttu-id="ad5ba-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad5ba-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad5ba-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="ad5ba-111">disabledPlans</span></span>|<span data-ttu-id="ad5ba-112">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ad5ba-112">Guid collection</span></span>|<span data-ttu-id="ad5ba-113">Eine Auflistung der eindeutigen Bezeichner für Pläne, die deaktiviert wurden.</span><span class="sxs-lookup"><span data-stu-id="ad5ba-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="ad5ba-114">skuId</span><span class="sxs-lookup"><span data-stu-id="ad5ba-114">skuId</span></span>|<span data-ttu-id="ad5ba-115">Guid</span><span class="sxs-lookup"><span data-stu-id="ad5ba-115">Guid</span></span>|<span data-ttu-id="ad5ba-116">Die eindeutige ID der SKU.</span><span class="sxs-lookup"><span data-stu-id="ad5ba-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad5ba-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad5ba-117">JSON representation</span></span>

<span data-ttu-id="ad5ba-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad5ba-118">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/assignedlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

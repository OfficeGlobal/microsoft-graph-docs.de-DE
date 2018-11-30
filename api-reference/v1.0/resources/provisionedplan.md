---
title: provisionedPlan-Ressourcentyp
description: Die **ProvisionedPlans**-Eigenschaft der user-Entität und der oganization-Entität ist eine Sammlung von **provisionedPlan**.
ms.openlocfilehash: 7808e3a17e471123f702381fb52535e53682e276
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018643"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="9e4a4-103">provisionedPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e4a4-103">provisionedPlan resource type</span></span>

<span data-ttu-id="9e4a4-104">Die **ProvisionedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="9e4a4-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="9e4a4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e4a4-105">Properties</span></span>
| <span data-ttu-id="9e4a4-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e4a4-106">Property</span></span>     | <span data-ttu-id="9e4a4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="9e4a4-107">Type</span></span>   |<span data-ttu-id="9e4a4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e4a4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e4a4-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="9e4a4-109">capabilityStatus</span></span>|<span data-ttu-id="9e4a4-110">String</span><span class="sxs-lookup"><span data-stu-id="9e4a4-110">String</span></span>|<span data-ttu-id="9e4a4-111">Z. B. „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="9e4a4-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="9e4a4-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="9e4a4-112">provisioningStatus</span></span>|<span data-ttu-id="9e4a4-113">String</span><span class="sxs-lookup"><span data-stu-id="9e4a4-113">String</span></span>|<span data-ttu-id="9e4a4-114">Z. B. „Erfolgreich“.</span><span class="sxs-lookup"><span data-stu-id="9e4a4-114">For example, “Success”.</span></span>|
|<span data-ttu-id="9e4a4-115">service</span><span class="sxs-lookup"><span data-stu-id="9e4a4-115">service</span></span>|<span data-ttu-id="9e4a4-116">String</span><span class="sxs-lookup"><span data-stu-id="9e4a4-116">String</span></span>|<span data-ttu-id="9e4a4-117">Der Name des Diensts. z. B. „AccessControlS2S“</span><span class="sxs-lookup"><span data-stu-id="9e4a4-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e4a4-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e4a4-118">JSON representation</span></span>

<span data-ttu-id="9e4a4-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e4a4-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
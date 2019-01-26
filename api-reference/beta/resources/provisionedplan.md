---
title: provisionedPlan-Ressourcentyp
description: Die **ProvisionedPlans**-Eigenschaft der user-Entität und der oganization-Entität ist eine Sammlung von **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: be19bb49409751ae5d7a0f11387e74770fde333b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572549"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="87901-103">provisionedPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="87901-103">provisionedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87901-104">Die **ProvisionedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="87901-104">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="87901-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87901-105">Properties</span></span>
| <span data-ttu-id="87901-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87901-106">Property</span></span>     | <span data-ttu-id="87901-107">Typ</span><span class="sxs-lookup"><span data-stu-id="87901-107">Type</span></span>   |<span data-ttu-id="87901-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87901-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87901-109">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="87901-109">capabilityStatus</span></span>|<span data-ttu-id="87901-110">String</span><span class="sxs-lookup"><span data-stu-id="87901-110">String</span></span>|<span data-ttu-id="87901-111">Z. B. „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="87901-111">For example, “Enabled”.</span></span>|
|<span data-ttu-id="87901-112">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="87901-112">provisioningStatus</span></span>|<span data-ttu-id="87901-113">String</span><span class="sxs-lookup"><span data-stu-id="87901-113">String</span></span>|<span data-ttu-id="87901-114">Z. B. „Erfolgreich“.</span><span class="sxs-lookup"><span data-stu-id="87901-114">For example, “Success”.</span></span>|
|<span data-ttu-id="87901-115">service</span><span class="sxs-lookup"><span data-stu-id="87901-115">service</span></span>|<span data-ttu-id="87901-116">String</span><span class="sxs-lookup"><span data-stu-id="87901-116">String</span></span>|<span data-ttu-id="87901-117">Der Name des Diensts. z. B. „AccessControlS2S“</span><span class="sxs-lookup"><span data-stu-id="87901-117">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87901-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87901-118">JSON representation</span></span>

<span data-ttu-id="87901-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="87901-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/provisionedplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: provisionedPlan-Ressourcentyp
description: Die **ProvisionedPlans**-Eigenschaft der user-Entität und der oganization-Entität ist eine Sammlung von **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: 7bed57761777e637fdc2e567d10aa7f741a86663
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837254"
---
# <a name="provisionedplan-resource-type"></a><span data-ttu-id="6c48f-103">provisionedPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6c48f-103">provisionedPlan resource type</span></span>

> <span data-ttu-id="6c48f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6c48f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c48f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c48f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c48f-106">Die **ProvisionedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="6c48f-106">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="6c48f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6c48f-107">Properties</span></span>
| <span data-ttu-id="6c48f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c48f-108">Property</span></span>     | <span data-ttu-id="6c48f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6c48f-109">Type</span></span>   |<span data-ttu-id="6c48f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c48f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c48f-111">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="6c48f-111">capabilityStatus</span></span>|<span data-ttu-id="6c48f-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c48f-112">String</span></span>|<span data-ttu-id="6c48f-113">Z. B. „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="6c48f-113">For example, “Enabled”.</span></span>|
|<span data-ttu-id="6c48f-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="6c48f-114">provisioningStatus</span></span>|<span data-ttu-id="6c48f-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c48f-115">String</span></span>|<span data-ttu-id="6c48f-116">Z. B. „Erfolgreich“.</span><span class="sxs-lookup"><span data-stu-id="6c48f-116">For example, “Success”.</span></span>|
|<span data-ttu-id="6c48f-117">service</span><span class="sxs-lookup"><span data-stu-id="6c48f-117">service</span></span>|<span data-ttu-id="6c48f-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c48f-118">String</span></span>|<span data-ttu-id="6c48f-119">Der Name des Diensts. z. B. „AccessControlS2S“</span><span class="sxs-lookup"><span data-stu-id="6c48f-119">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c48f-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6c48f-120">JSON representation</span></span>

<span data-ttu-id="6c48f-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6c48f-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
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

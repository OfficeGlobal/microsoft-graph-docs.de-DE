---
title: servicePlanInfo-Ressourcentyp
description: Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der subscribedSku-Entität ist eine Sammlung von **servicePlanInfo**.
localization_priority: Normal
ms.openlocfilehash: f0cb96a11b280fcda4e97a6dad30a9e5200c2e88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842679"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="68d55-104">servicePlanInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="68d55-104">servicePlanInfo resource type</span></span>

> <span data-ttu-id="68d55-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="68d55-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68d55-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68d55-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68d55-p103">Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist eine Sammlung von **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="68d55-p103">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="68d55-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68d55-109">Properties</span></span>
| <span data-ttu-id="68d55-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68d55-110">Property</span></span>     | <span data-ttu-id="68d55-111">Typ</span><span class="sxs-lookup"><span data-stu-id="68d55-111">Type</span></span>   |<span data-ttu-id="68d55-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68d55-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68d55-113">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="68d55-113">servicePlanId</span></span>|<span data-ttu-id="68d55-114">Guid</span><span class="sxs-lookup"><span data-stu-id="68d55-114">Guid</span></span>|<span data-ttu-id="68d55-115">Der eindeutige Bezeichner des Serviceplans.</span><span class="sxs-lookup"><span data-stu-id="68d55-115">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="68d55-116">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="68d55-116">servicePlanName</span></span>|<span data-ttu-id="68d55-117">String</span><span class="sxs-lookup"><span data-stu-id="68d55-117">String</span></span>|<span data-ttu-id="68d55-118">Der Name des Serviceplans.</span><span class="sxs-lookup"><span data-stu-id="68d55-118">The name of the service plan.</span></span>|
|<span data-ttu-id="68d55-119">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="68d55-119">provisioningStatus</span></span>|<span data-ttu-id="68d55-120">String</span><span class="sxs-lookup"><span data-stu-id="68d55-120">String</span></span>|<span data-ttu-id="68d55-p104">Der Bereitstellungsstatus des Serviceplans. Mögliche Werte:</span><span class="sxs-lookup"><span data-stu-id="68d55-p104">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="68d55-123">„Success“ - Der Dienst wurde vollständig bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="68d55-123">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="68d55-124">„Disabled“ - Der Dienst wurde deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="68d55-124">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="68d55-125">„PendingInput“ - Der Dienst wurde noch nicht bereitgestellt, es wird auf die Dienstbestätigung gewartet.</span><span class="sxs-lookup"><span data-stu-id="68d55-125">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="68d55-126">"PendingActivation" - Dienst erfordert explizite Aktivierung vom Administrator (beispielsweise Intune_O365 Dienstplan) jedoch bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="68d55-126">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan).</span></span><br/><span data-ttu-id="68d55-127">„PendingProvisioning“ - Microsoft hat einen neuen Dienst zur Produkt-SKU hinzugefügt, der noch nicht im Mandanten aktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="68d55-127">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="68d55-128">appliesTo</span><span class="sxs-lookup"><span data-stu-id="68d55-128">appliesTo</span></span>|<span data-ttu-id="68d55-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68d55-129">String</span></span>|<span data-ttu-id="68d55-p105">Das Objekt, dem der Serviceplan zugewiesen werden kann. Mögliche Werte:</span><span class="sxs-lookup"><span data-stu-id="68d55-p105">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="68d55-132">„User“ - Der Serviceplan kann einzelnen Benutzern zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="68d55-132">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="68d55-133">„Company“ - Der Serviceplan kann dem gesamten Mandanten zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="68d55-133">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68d55-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68d55-134">JSON representation</span></span>

<span data-ttu-id="68d55-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68d55-135">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

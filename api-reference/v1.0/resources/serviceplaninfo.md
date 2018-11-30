---
title: servicePlanInfo-Ressourcentyp
description: Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der subscribedSku-Entität ist eine Sammlung von **servicePlanInfo**.
ms.openlocfilehash: 70d49eb22542e9bc22ee28df5bc77b3bf6146b6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017896"
---
# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="4d700-104">servicePlanInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4d700-104">servicePlanInfo resource type</span></span>

<span data-ttu-id="4d700-p102">Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist eine Sammlung von **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="4d700-p102">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="4d700-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4d700-107">Properties</span></span>
| <span data-ttu-id="4d700-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d700-108">Property</span></span>     | <span data-ttu-id="4d700-109">Typ</span><span class="sxs-lookup"><span data-stu-id="4d700-109">Type</span></span>   |<span data-ttu-id="4d700-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d700-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d700-111">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="4d700-111">servicePlanId</span></span>|<span data-ttu-id="4d700-112">Guid</span><span class="sxs-lookup"><span data-stu-id="4d700-112">Guid</span></span>|<span data-ttu-id="4d700-113">Der eindeutige Bezeichner des Serviceplans.</span><span class="sxs-lookup"><span data-stu-id="4d700-113">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="4d700-114">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="4d700-114">servicePlanName</span></span>|<span data-ttu-id="4d700-115">String</span><span class="sxs-lookup"><span data-stu-id="4d700-115">String</span></span>|<span data-ttu-id="4d700-116">Der Name des Serviceplans.</span><span class="sxs-lookup"><span data-stu-id="4d700-116">The name of the service plan.</span></span>|
|<span data-ttu-id="4d700-117">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="4d700-117">provisioningStatus</span></span>|<span data-ttu-id="4d700-118">String</span><span class="sxs-lookup"><span data-stu-id="4d700-118">String</span></span>|<span data-ttu-id="4d700-p103">Der Bereitstellungsstatus des Serviceplans. Mögliche Werte:</span><span class="sxs-lookup"><span data-stu-id="4d700-p103">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="4d700-121">„Success“ - Der Dienst wurde vollständig bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="4d700-121">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="4d700-122">„Disabled“ - Der Dienst wurde deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="4d700-122">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="4d700-123">„PendingInput“ - Der Dienst wurde noch nicht bereitgestellt, es wird auf die Dienstbestätigung gewartet.</span><span class="sxs-lookup"><span data-stu-id="4d700-123">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="4d700-124">„PendingActivation“ - Der Dienst wurde bereitgestellt, erfordert aber die explizite Aktivierung durch einen Administrator (z. B. Intune_O365-Serviceplan)</span><span class="sxs-lookup"><span data-stu-id="4d700-124">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="4d700-125">„PendingProvisioning“ - Microsoft hat einen neuen Dienst zur Produkt-SKU hinzugefügt, der noch nicht im Mandanten aktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="4d700-125">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="4d700-126">appliesTo</span><span class="sxs-lookup"><span data-stu-id="4d700-126">appliesTo</span></span>|<span data-ttu-id="4d700-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d700-127">String</span></span>|<span data-ttu-id="4d700-p104">Das Objekt, dem der Serviceplan zugewiesen werden kann. Mögliche Werte:</span><span class="sxs-lookup"><span data-stu-id="4d700-p104">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="4d700-130">„User“ - Der Serviceplan kann einzelnen Benutzern zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="4d700-130">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="4d700-131">„Company“ - Der Serviceplan kann dem gesamten Mandanten zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="4d700-131">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d700-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4d700-132">JSON representation</span></span>

<span data-ttu-id="4d700-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d700-133">Here is a JSON representation of the resource</span></span>

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

---
title: Ressourcentyp cloudAppSecurityState
description: Statusinformationen über die Cloudanwendung (DestinationServiceName, DestinationServiceIp) enthält.
ms.openlocfilehash: 915044c3084e3d9a9435d602ecc7ec809d2168f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019783"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="81ec4-103">Ressourcentyp cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="81ec4-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="81ec4-104">Statusinformationen über die Cloudanwendung (DestinationServiceName, DestinationServiceIp) enthält.</span><span class="sxs-lookup"><span data-stu-id="81ec4-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="81ec4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81ec4-105">Properties</span></span>

| <span data-ttu-id="81ec4-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81ec4-106">Property</span></span>     | <span data-ttu-id="81ec4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="81ec4-107">Type</span></span>        | <span data-ttu-id="81ec4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81ec4-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81ec4-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="81ec4-109">destinationServiceIp</span></span>|<span data-ttu-id="81ec4-110">String</span><span class="sxs-lookup"><span data-stu-id="81ec4-110">String</span></span>|<span data-ttu-id="81ec4-111">Ziel-IP-Adresse der Verbindung mit der Cloud Anwendungsdienst.</span><span class="sxs-lookup"><span data-stu-id="81ec4-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="81ec4-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="81ec4-112">destinationServiceName</span></span>|<span data-ttu-id="81ec4-113">String</span><span class="sxs-lookup"><span data-stu-id="81ec4-113">String</span></span>|<span data-ttu-id="81ec4-114">Cloud-Anwendungsdienst/Name (zum Beispiel "Vertrieb", "Ablage" usw.).</span><span class="sxs-lookup"><span data-stu-id="81ec4-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="81ec4-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="81ec4-115">riskScore</span></span>|<span data-ttu-id="81ec4-116">String</span><span class="sxs-lookup"><span data-stu-id="81ec4-116">String</span></span>|<span data-ttu-id="81ec4-117">Provider-generiert/berechnet Risiko Score von der Anwendung/Clouddienst.</span><span class="sxs-lookup"><span data-stu-id="81ec4-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="81ec4-118">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="81ec4-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81ec4-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81ec4-119">JSON representation</span></span>

<span data-ttu-id="81ec4-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81ec4-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
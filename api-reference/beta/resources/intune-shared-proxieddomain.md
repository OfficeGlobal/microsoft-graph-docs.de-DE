---
title: proxiedDomain-Ressourcentyp
description: Proxydomäne
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5edabc31761a3abd79a94bb700392923d2d54513
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151205"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="54161-103">proxiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="54161-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="54161-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54161-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54161-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="54161-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54161-106">Proxydomäne</span><span class="sxs-lookup"><span data-stu-id="54161-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="54161-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54161-107">Properties</span></span>
|<span data-ttu-id="54161-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54161-108">Property</span></span>|<span data-ttu-id="54161-109">Typ</span><span class="sxs-lookup"><span data-stu-id="54161-109">Type</span></span>|<span data-ttu-id="54161-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54161-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54161-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="54161-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="54161-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54161-112">String</span></span>|<span data-ttu-id="54161-113">Die IP-Adresse oder der FQDN</span><span class="sxs-lookup"><span data-stu-id="54161-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="54161-114">Proxy</span><span class="sxs-lookup"><span data-stu-id="54161-114">proxy</span></span>|<span data-ttu-id="54161-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54161-115">String</span></span>|<span data-ttu-id="54161-116">Proxy-IP oder FQDN</span><span class="sxs-lookup"><span data-stu-id="54161-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="54161-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="54161-117">Relationships</span></span>
<span data-ttu-id="54161-118">Keine</span><span class="sxs-lookup"><span data-stu-id="54161-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54161-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54161-119">JSON Representation</span></span>
<span data-ttu-id="54161-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54161-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```





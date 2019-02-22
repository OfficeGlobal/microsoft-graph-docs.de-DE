---
title: vpnTrafficRule-Ressourcentyp
description: Definition der VPN-Datenverkehr-Regel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd004341928260187518966e2356f59faff57898
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139942"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="580f0-103">vpnTrafficRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="580f0-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="580f0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="580f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="580f0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="580f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="580f0-106">Definition der VPN-Datenverkehr-Regel.</span><span class="sxs-lookup"><span data-stu-id="580f0-106">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="580f0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="580f0-107">Properties</span></span>
|<span data-ttu-id="580f0-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="580f0-108">Property</span></span>|<span data-ttu-id="580f0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="580f0-109">Type</span></span>|<span data-ttu-id="580f0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="580f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="580f0-111">name</span><span class="sxs-lookup"><span data-stu-id="580f0-111">name</span></span>|<span data-ttu-id="580f0-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="580f0-112">String</span></span>|<span data-ttu-id="580f0-113">Namen.</span><span class="sxs-lookup"><span data-stu-id="580f0-113">Name.</span></span>|
|<span data-ttu-id="580f0-114">Protokolle</span><span class="sxs-lookup"><span data-stu-id="580f0-114">protocols</span></span>|<span data-ttu-id="580f0-115">Int32</span><span class="sxs-lookup"><span data-stu-id="580f0-115">Int32</span></span>|<span data-ttu-id="580f0-116">Protokolle (0-255).</span><span class="sxs-lookup"><span data-stu-id="580f0-116">Protocols (0-255).</span></span> <span data-ttu-id="580f0-117">Gültige Werte 0 bis 255</span><span class="sxs-lookup"><span data-stu-id="580f0-117">Valid values 0 to 255</span></span>|
|<span data-ttu-id="580f0-118">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="580f0-118">localPortRanges</span></span>|<span data-ttu-id="580f0-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="580f0-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="580f0-120">Der lokale Portregel kann nur festgelegt werden, wenn das Protokoll TCP oder UDP (6 oder 17) ist.</span><span class="sxs-lookup"><span data-stu-id="580f0-120">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="580f0-121">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="580f0-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="580f0-122">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="580f0-122">remotePortRanges</span></span>|<span data-ttu-id="580f0-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="580f0-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="580f0-124">Der Remote-Portierungs-Range kann nur festgelegt werden, wenn das Protokoll TCP oder UDP (6 oder 17) ist.</span><span class="sxs-lookup"><span data-stu-id="580f0-124">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="580f0-125">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="580f0-125">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="580f0-126">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="580f0-126">localAddressRanges</span></span>|<span data-ttu-id="580f0-127">[iPv4Range](../resources/intune-shared-ipv4range.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="580f0-127">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="580f0-128">Lokaler adressumfang.</span><span class="sxs-lookup"><span data-stu-id="580f0-128">Local address range.</span></span> <span data-ttu-id="580f0-129">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="580f0-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="580f0-130">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="580f0-130">remoteAddressRanges</span></span>|<span data-ttu-id="580f0-131">[iPv4Range](../resources/intune-shared-ipv4range.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="580f0-131">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="580f0-132">Remote Adressbereiche.</span><span class="sxs-lookup"><span data-stu-id="580f0-132">Remote address range.</span></span> <span data-ttu-id="580f0-133">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="580f0-133">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="580f0-134">appId</span><span class="sxs-lookup"><span data-stu-id="580f0-134">appId</span></span>|<span data-ttu-id="580f0-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="580f0-135">String</span></span>|<span data-ttu-id="580f0-136">APP-ID, wenn diese Datenverkehrs Regel von einer APP ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="580f0-136">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="580f0-137">appType</span><span class="sxs-lookup"><span data-stu-id="580f0-137">appType</span></span>|[<span data-ttu-id="580f0-138">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="580f0-138">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="580f0-139">App-Typ, wenn diese Datenverkehrs Regel von einer APP ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="580f0-139">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="580f0-140">Mögliche Werte sind: `none`, `desktop` und `universal`.</span><span class="sxs-lookup"><span data-stu-id="580f0-140">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="580f0-141">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="580f0-141">routingPolicyType</span></span>|[<span data-ttu-id="580f0-142">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="580f0-142">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="580f0-143">Wenn die APP ausgelöst wird, wird angegeben, ob ein geteilten Tunnel auf dieser Route aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="580f0-143">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="580f0-144">Mögliche Werte sind: `none`, `splitTunnel` und `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="580f0-144">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="580f0-145">Ansprüche</span><span class="sxs-lookup"><span data-stu-id="580f0-145">claims</span></span>|<span data-ttu-id="580f0-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="580f0-146">String</span></span>|<span data-ttu-id="580f0-147">Dieser Datenverkehrs Regel zugeordnete Forderung.</span><span class="sxs-lookup"><span data-stu-id="580f0-147">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="580f0-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="580f0-148">Relationships</span></span>
<span data-ttu-id="580f0-149">Keine</span><span class="sxs-lookup"><span data-stu-id="580f0-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="580f0-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="580f0-150">JSON Representation</span></span>
<span data-ttu-id="580f0-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="580f0-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```





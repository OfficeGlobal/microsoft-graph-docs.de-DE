---
title: Ressourcentyp vpnTrafficRule
description: VPN-Datenverkehr Regeldefinition.
ms.openlocfilehash: 564528cf0c0ae39785a2cc43dc800d8dbdf7d285
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059972"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="4fa9c-103">Ressourcentyp vpnTrafficRule</span><span class="sxs-lookup"><span data-stu-id="4fa9c-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="4fa9c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fa9c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fa9c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fa9c-107">VPN-Datenverkehr Regeldefinition.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-107">VPN Traffic Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="4fa9c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4fa9c-108">Properties</span></span>
|<span data-ttu-id="4fa9c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4fa9c-109">Property</span></span>|<span data-ttu-id="4fa9c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4fa9c-110">Type</span></span>|<span data-ttu-id="4fa9c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4fa9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fa9c-112">name</span><span class="sxs-lookup"><span data-stu-id="4fa9c-112">name</span></span>|<span data-ttu-id="4fa9c-113">String</span><span class="sxs-lookup"><span data-stu-id="4fa9c-113">String</span></span>|<span data-ttu-id="4fa9c-114">Name.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-114">Name.</span></span>|
|<span data-ttu-id="4fa9c-115">Protokolle</span><span class="sxs-lookup"><span data-stu-id="4fa9c-115">protocols</span></span>|<span data-ttu-id="4fa9c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4fa9c-116">Int32</span></span>|<span data-ttu-id="4fa9c-117">Protokolle (0 – 255).</span><span class="sxs-lookup"><span data-stu-id="4fa9c-117">Protocols (0-255).</span></span> <span data-ttu-id="4fa9c-118">Gültige Werte zwischen 0 und 255</span><span class="sxs-lookup"><span data-stu-id="4fa9c-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="4fa9c-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="4fa9c-119">localPortRanges</span></span>|<span data-ttu-id="4fa9c-120">[NumberRange](../resources/intune-deviceconfig-numberrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4fa9c-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="4fa9c-121">Lokaler Portbereich kann nur bei Protokoll entweder TCP oder UDP (6 oder 17) festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="4fa9c-122">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4fa9c-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="4fa9c-123">remotePortRanges</span></span>|<span data-ttu-id="4fa9c-124">[NumberRange](../resources/intune-deviceconfig-numberrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4fa9c-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="4fa9c-125">Remote Portbereich kann nur bei Protokoll entweder TCP oder UDP (6 oder 17) festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="4fa9c-126">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4fa9c-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="4fa9c-127">localAddressRanges</span></span>|<span data-ttu-id="4fa9c-128">[iPv4Range](../resources/intune-shared-ipv4range.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4fa9c-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="4fa9c-129">Lokale Adressbereich.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-129">Local address range.</span></span> <span data-ttu-id="4fa9c-130">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4fa9c-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="4fa9c-131">remoteAddressRanges</span></span>|<span data-ttu-id="4fa9c-132">[iPv4Range](../resources/intune-shared-ipv4range.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4fa9c-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="4fa9c-133">Remote-Adressbereichs.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-133">Remote address range.</span></span> <span data-ttu-id="4fa9c-134">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4fa9c-135">appId</span><span class="sxs-lookup"><span data-stu-id="4fa9c-135">appId</span></span>|<span data-ttu-id="4fa9c-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4fa9c-136">String</span></span>|<span data-ttu-id="4fa9c-137">App-Bezeichner, wenn diese Regel Datenverkehr durch eine app ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="4fa9c-138">der appType</span><span class="sxs-lookup"><span data-stu-id="4fa9c-138">appType</span></span>|[<span data-ttu-id="4fa9c-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="4fa9c-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="4fa9c-140">App-Typ, wenn diese Regel Datenverkehr durch eine app ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="4fa9c-141">Mögliche Werte sind: `none`, `desktop` und `universal`.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="4fa9c-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="4fa9c-142">routingPolicyType</span></span>|[<span data-ttu-id="4fa9c-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="4fa9c-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="4fa9c-144">Wenn gibt an, ob aktivieren Split-tunneling auf diese Route ausgelöst, app.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="4fa9c-145">Mögliche Werte sind: `none`, `splitTunnel` und `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="4fa9c-146">Ansprüche</span><span class="sxs-lookup"><span data-stu-id="4fa9c-146">claims</span></span>|<span data-ttu-id="4fa9c-147">String</span><span class="sxs-lookup"><span data-stu-id="4fa9c-147">String</span></span>|<span data-ttu-id="4fa9c-148">Ansprüche im Zusammenhang mit dieser Regel Datenverkehr.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fa9c-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4fa9c-149">Relationships</span></span>
<span data-ttu-id="4fa9c-150">Keine</span><span class="sxs-lookup"><span data-stu-id="4fa9c-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4fa9c-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4fa9c-151">JSON Representation</span></span>
<span data-ttu-id="4fa9c-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4fa9c-152">Here is a JSON representation of the resource.</span></span>
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






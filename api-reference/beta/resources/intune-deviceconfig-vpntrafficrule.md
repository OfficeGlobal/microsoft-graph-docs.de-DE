---
title: Ressourcentyp vpnTrafficRule
description: VPN-Datenverkehr Regeldefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b28d26356eea113f267c4eb0499f9600671f114
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415285"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="6a134-103">Ressourcentyp vpnTrafficRule</span><span class="sxs-lookup"><span data-stu-id="6a134-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="6a134-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6a134-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6a134-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a134-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a134-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a134-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a134-107">VPN-Datenverkehr Regeldefinition.</span><span class="sxs-lookup"><span data-stu-id="6a134-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="6a134-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a134-108">Properties</span></span>
|<span data-ttu-id="6a134-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a134-109">Property</span></span>|<span data-ttu-id="6a134-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6a134-110">Type</span></span>|<span data-ttu-id="6a134-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a134-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a134-112">name</span><span class="sxs-lookup"><span data-stu-id="6a134-112">name</span></span>|<span data-ttu-id="6a134-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a134-113">String</span></span>|<span data-ttu-id="6a134-114">Name.</span><span class="sxs-lookup"><span data-stu-id="6a134-114">Name.</span></span>|
|<span data-ttu-id="6a134-115">Protokolle</span><span class="sxs-lookup"><span data-stu-id="6a134-115">protocols</span></span>|<span data-ttu-id="6a134-116">Int32</span><span class="sxs-lookup"><span data-stu-id="6a134-116">Int32</span></span>|<span data-ttu-id="6a134-117">Protokolle (0 – 255).</span><span class="sxs-lookup"><span data-stu-id="6a134-117">Protocols (0-255).</span></span> <span data-ttu-id="6a134-118">Gültige Werte zwischen 0 und 255</span><span class="sxs-lookup"><span data-stu-id="6a134-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="6a134-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="6a134-119">localPortRanges</span></span>|<span data-ttu-id="6a134-120">[NumberRange](../resources/intune-deviceconfig-numberrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6a134-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="6a134-121">Lokaler Portbereich kann nur bei Protokoll entweder TCP oder UDP (6 oder 17) festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="6a134-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="6a134-122">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6a134-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6a134-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="6a134-123">remotePortRanges</span></span>|<span data-ttu-id="6a134-124">[NumberRange](../resources/intune-deviceconfig-numberrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6a134-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="6a134-125">Remote Portbereich kann nur bei Protokoll entweder TCP oder UDP (6 oder 17) festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="6a134-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="6a134-126">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6a134-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6a134-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="6a134-127">localAddressRanges</span></span>|<span data-ttu-id="6a134-128">[iPv4Range](../resources/intune-shared-ipv4range.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6a134-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="6a134-129">Lokale Adressbereich.</span><span class="sxs-lookup"><span data-stu-id="6a134-129">Local address range.</span></span> <span data-ttu-id="6a134-130">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6a134-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6a134-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="6a134-131">remoteAddressRanges</span></span>|<span data-ttu-id="6a134-132">[iPv4Range](../resources/intune-shared-ipv4range.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6a134-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="6a134-133">Remote-Adressbereichs.</span><span class="sxs-lookup"><span data-stu-id="6a134-133">Remote address range.</span></span> <span data-ttu-id="6a134-134">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6a134-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6a134-135">appId</span><span class="sxs-lookup"><span data-stu-id="6a134-135">appId</span></span>|<span data-ttu-id="6a134-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a134-136">String</span></span>|<span data-ttu-id="6a134-137">App-Bezeichner, wenn diese Regel Datenverkehr durch eine app ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="6a134-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="6a134-138">der appType</span><span class="sxs-lookup"><span data-stu-id="6a134-138">appType</span></span>|[<span data-ttu-id="6a134-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="6a134-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="6a134-140">App-Typ, wenn diese Regel Datenverkehr durch eine app ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="6a134-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="6a134-141">Mögliche Werte sind: `none`, `desktop` und `universal`.</span><span class="sxs-lookup"><span data-stu-id="6a134-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="6a134-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="6a134-142">routingPolicyType</span></span>|[<span data-ttu-id="6a134-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="6a134-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="6a134-144">Wenn gibt an, ob aktivieren Split-tunneling auf diese Route ausgelöst, app.</span><span class="sxs-lookup"><span data-stu-id="6a134-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="6a134-145">Mögliche Werte sind: `none`, `splitTunnel` und `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="6a134-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="6a134-146">Ansprüche</span><span class="sxs-lookup"><span data-stu-id="6a134-146">claims</span></span>|<span data-ttu-id="6a134-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a134-147">String</span></span>|<span data-ttu-id="6a134-148">Ansprüche im Zusammenhang mit dieser Regel Datenverkehr.</span><span class="sxs-lookup"><span data-stu-id="6a134-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a134-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6a134-149">Relationships</span></span>
<span data-ttu-id="6a134-150">Keine</span><span class="sxs-lookup"><span data-stu-id="6a134-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a134-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a134-151">JSON Representation</span></span>
<span data-ttu-id="6a134-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a134-152">Here is a JSON representation of the resource.</span></span>
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





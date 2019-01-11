---
title: Ressourcentyp vpnTrafficRule
description: VPN-Datenverkehr Regeldefinition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b7a4a1841850c0276e50068b9e9c7d1ce69e765
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840222"
---
# <a name="vpntrafficrule-resource-type"></a>Ressourcentyp vpnTrafficRule

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

VPN-Datenverkehr Regeldefinition.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|String|Name.|
|Protokolle|Int32|Protokolle (0 – 255). Gültige Werte zwischen 0 und 255|
|localPortRanges|[NumberRange](../resources/intune-deviceconfig-numberrange.md) -Auflistung|Lokaler Portbereich kann nur bei Protokoll entweder TCP oder UDP (6 oder 17) festgelegt werden. Diese Collection darf maximal 500 Elemente enthalten.|
|remotePortRanges|[NumberRange](../resources/intune-deviceconfig-numberrange.md) -Auflistung|Remote Portbereich kann nur bei Protokoll entweder TCP oder UDP (6 oder 17) festgelegt werden. Diese Collection darf maximal 500 Elemente enthalten.|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) -Auflistung|Lokale Adressbereich. Diese Collection darf maximal 500 Elemente enthalten.|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) -Auflistung|Remote-Adressbereichs. Diese Collection darf maximal 500 Elemente enthalten.|
|appId|Zeichenfolge|App-Bezeichner, wenn diese Regel Datenverkehr durch eine app ausgelöst wird.|
|der appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|App-Typ, wenn diese Regel Datenverkehr durch eine app ausgelöst wird. Mögliche Werte sind: `none`, `desktop` und `universal`.|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|Wenn gibt an, ob aktivieren Split-tunneling auf diese Route ausgelöst, app. Mögliche Werte sind: `none`, `splitTunnel` und `forceTunnel`.|
|Ansprüche|String|Ansprüche im Zusammenhang mit dieser Regel Datenverkehr.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
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






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
# <a name="vpntrafficrule-resource-type"></a>Ressourcentyp vpnTrafficRule

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

VPN-Datenverkehr Regeldefinition.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Name.|
|Protokolle|Int32|Protokolle (0 – 255). Gültige Werte zwischen 0 und 255|
|localPortRanges|[NumberRange](../resources/intune-deviceconfig-numberrange.md) -Auflistung|Lokaler Portbereich kann nur bei Protokoll entweder TCP oder UDP (6 oder 17) festgelegt werden. Diese Collection darf maximal 500 Elemente enthalten.|
|remotePortRanges|[NumberRange](../resources/intune-deviceconfig-numberrange.md) -Auflistung|Remote Portbereich kann nur bei Protokoll entweder TCP oder UDP (6 oder 17) festgelegt werden. Diese Collection darf maximal 500 Elemente enthalten.|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) -Auflistung|Lokale Adressbereich. Diese Collection darf maximal 500 Elemente enthalten.|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) -Auflistung|Remote-Adressbereichs. Diese Collection darf maximal 500 Elemente enthalten.|
|appId|Zeichenfolge|App-Bezeichner, wenn diese Regel Datenverkehr durch eine app ausgelöst wird.|
|der appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|App-Typ, wenn diese Regel Datenverkehr durch eine app ausgelöst wird. Mögliche Werte sind: `none`, `desktop` und `universal`.|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|Wenn gibt an, ob aktivieren Split-tunneling auf diese Route ausgelöst, app. Mögliche Werte sind: `none`, `splitTunnel` und `forceTunnel`.|
|Ansprüche|Zeichenfolge|Ansprüche im Zusammenhang mit dieser Regel Datenverkehr.|

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





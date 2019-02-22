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
# <a name="vpntrafficrule-resource-type"></a>vpnTrafficRule-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Definition der VPN-Datenverkehr-Regel.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Namen.|
|Protokolle|Int32|Protokolle (0-255). Gültige Werte 0 bis 255|
|localPortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md) -Sammlung|Der lokale Portregel kann nur festgelegt werden, wenn das Protokoll TCP oder UDP (6 oder 17) ist. Diese Collection darf maximal 500 Elemente enthalten.|
|remotePortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md) -Sammlung|Der Remote-Portierungs-Range kann nur festgelegt werden, wenn das Protokoll TCP oder UDP (6 oder 17) ist. Diese Collection darf maximal 500 Elemente enthalten.|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) -Sammlung|Lokaler adressumfang. Diese Collection darf maximal 500 Elemente enthalten.|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) -Sammlung|Remote Adressbereiche. Diese Collection darf maximal 500 Elemente enthalten.|
|appId|Zeichenfolge|APP-ID, wenn diese Datenverkehrs Regel von einer APP ausgelöst wird.|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|App-Typ, wenn diese Datenverkehrs Regel von einer APP ausgelöst wird. Mögliche Werte sind: `none`, `desktop` und `universal`.|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|Wenn die APP ausgelöst wird, wird angegeben, ob ein geteilten Tunnel auf dieser Route aktiviert werden soll. Mögliche Werte sind: `none`, `splitTunnel` und `forceTunnel`.|
|Ansprüche|Zeichenfolge|Dieser Datenverkehrs Regel zugeordnete Forderung.|

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





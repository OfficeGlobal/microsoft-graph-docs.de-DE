---
title: vpnDnsRule-Ressourcentyp
description: Definition der VPN-DNS-Regel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 545c0dd8a84f19888452261e350a9b347061595c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158506"
---
# <a name="vpndnsrule-resource-type"></a>vpnDnsRule-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Definition der VPN-DNS-Regel.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Namen.|
|Server|String collection|Server.|
|proxyServerUri|Zeichenfolge|Proxy Server-URI.|
|autoTrigger|Boolescher Wert|Herstellen einer Verbindung mit dem VPN, wenn das Gerät eine Verbindung mit dieser Domäne herstellt: Standard false.|
|persistent|Boolescher Wert|Diese Regel auch dann aktiv halten, wenn das VPN nicht verbunden ist: Standard false|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```





---
title: Ressourcentyp windows81VpnProxyServer
description: VPN-Proxy-Server.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a400ed128a80e6fae11f090f7cdd445fe8c174b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398891"
---
# <a name="windows81vpnproxyserver-resource-type"></a>Ressourcentyp windows81VpnProxyServer

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

VPN-Proxy-Server.


Erbt vom [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|automaticConfigurationScriptUrl|Zeichenfolge|Automatische Konfiguration Skript-Url des Proxys. Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|Zeichenfolge|Adresse. Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|port|Int32|Port. Gültige Werte zwischen 0 und 65535 Inherited aus [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|automaticallyDetectProxySettings|Boolean|Erkennen Sie Proxyeinstellungen automatisch.|
|bypassProxyServerForLocalAddress|Boolean|Proxyserver für lokale Adressen umgehen.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```





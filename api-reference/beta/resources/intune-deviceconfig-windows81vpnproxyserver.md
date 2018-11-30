---
title: Ressourcentyp windows81VpnProxyServer
description: VPN-Proxy-Server.
ms.openlocfilehash: 27100dd3faecc9ba20a4bcc28985c56c9cb409c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058981"
---
# <a name="windows81vpnproxyserver-resource-type"></a>Ressourcentyp windows81VpnProxyServer

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

VPN-Proxy-Server.

Erbt vom [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|Automatische Konfiguration Skript-Url des Proxys. Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|Adresse. Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|port|Int32|Port. Gültige Werte zwischen 0 und 65535 Inherited aus [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|automaticallyDetectProxySettings|Boolesch|Erkennen Sie Proxyeinstellungen automatisch.|
|bypassProxyServerForLocalAddress|Boolesch|Proxyserver für lokale Adressen umgehen.|

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






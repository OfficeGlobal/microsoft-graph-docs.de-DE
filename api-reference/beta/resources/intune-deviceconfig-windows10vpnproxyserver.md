---
title: Ressourcentyp windows10VpnProxyServer
description: VPN-Proxy-Server.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4b34d105900478a1bcbc811e782e1ceaf94f251
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912274"
---
# <a name="windows10vpnproxyserver-resource-type"></a>Ressourcentyp windows10VpnProxyServer

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

VPN-Proxy-Server.

Erbt vom [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|automaticConfigurationScriptUrl|Zeichenfolge|Automatische Konfiguration Skript-Url des Proxys. Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|Zeichenfolge|Adresse. Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|port|Int32|Port. Gültige Werte zwischen 0 und 65535 Inherited aus [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Boolescher Wert|Proxyserver für lokale Adressen umgehen.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```






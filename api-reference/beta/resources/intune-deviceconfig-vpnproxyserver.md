---
title: Ressourcentyp vpnProxyServer
description: VPN-Proxy-Server.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 727d26af7f2c1801cd06fc98949109efec267f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955352"
---
# <a name="vpnproxyserver-resource-type"></a>Ressourcentyp vpnProxyServer

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

VPN-Proxy-Server.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|automaticConfigurationScriptUrl|Zeichenfolge|Automatische Konfiguration Skript-Url des Proxys.|
|address|Zeichenfolge|Adresse.|
|port|Int32|Port. Gültige Werte zwischen 0 und 65535|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```






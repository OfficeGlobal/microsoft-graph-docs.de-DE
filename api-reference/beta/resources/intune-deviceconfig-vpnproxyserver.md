---
title: Ressourcentyp vpnProxyServer
description: VPN-Proxy-Server.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 676e56771f021a79179e268280f5e3190754eef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425673"
---
# <a name="vpnproxyserver-resource-type"></a>Ressourcentyp vpnProxyServer

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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





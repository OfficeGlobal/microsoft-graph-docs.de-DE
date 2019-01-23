---
title: Ressourcentyp vpnDnsRule
description: VPN-DNS-Regeldefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae6141cc0579840a23a28be2dce951c160f90248
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425582"
---
# <a name="vpndnsrule-resource-type"></a>Ressourcentyp vpnDnsRule

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

VPN-DNS-Regeldefinition.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Name.|
|Server|Zeichenfolgenauflistung|Server.|
|proxyServerUri|Zeichenfolge|Proxy-Server-Uri.|
|autoTrigger|Boolean|Automatisch mit dem VPN verbinden, wenn das Gerät an diese Domäne eine Verbindung herstellt: Standardeinstellung "false".|
|persistent|Boolean|Diese Regel aktiv lassen, auch wenn das VPN nicht verbunden ist: Standardeinstellung "false"|

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





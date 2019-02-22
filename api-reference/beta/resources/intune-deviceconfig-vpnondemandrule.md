---
title: vpnOnDemandRule-Ressourcentyp
description: Definition der VPN-on-Demand-Regel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1bccd015e45291b344e7c77df4ac5c0a0af07d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161586"
---
# <a name="vpnondemandrule-resource-type"></a>vpnOnDemandRule-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Definition der VPN-on-Demand-Regel.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|SSIDs|String collection|Netzwerkdienst Satz-IDs (SSIDs).|
|dnsSearchDomains|String collection|DNS-Such Domänen.|
|probeUrl|Zeichenfolge|Eine zu über URL. Wenn diese URL erfolgreich abgerufen wird (zurückgeben eines 200 HTTP-Statuscodes) ohne Umleitung, stimmt diese Regel überein.|
|Aktion|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Aktion. Mögliche Werte: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|Domäne|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Domänen Aktion (gilt nur, wenn die Aktion die Verbindung auswertet). Mögliche Werte sind: `connectIfNeeded` und `neverConnect`.|
|Domänen|String collection|Domänen (gilt nur, wenn die Aktion die Verbindung auswertet).|
|probeRequiredUrl|Zeichenfolge|Überprüfen Sie die erforderliche URL (gilt nur, wenn die Aktion die Verbindung auswertet und wenn erforderlich die Domäne "Connect" ist).|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```





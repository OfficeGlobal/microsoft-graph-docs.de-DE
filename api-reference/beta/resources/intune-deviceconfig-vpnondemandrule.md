---
title: Ressourcentyp vpnOnDemandRule
description: VPN-On-Demand Regeldefinition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bd6e494975c8626a25380b3f037d702fb81e082b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875635"
---
# <a name="vpnondemandrule-resource-type"></a>Ressourcentyp vpnOnDemandRule

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

VPN-On-Demand Regeldefinition.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|SSIDs|Collection von Objekten des Typs „String“|Netzwerkdienst festgelegt (SSIDs Identifiers).|
|dnsSearchDomains|Collection von Objekten des Typs „String“|DNS-Suche Domänen.|
|probeUrl|Zeichenfolge|Eine URL zu belegen. Wenn diese URL erfolgreich ist ohne Umleitung abgerufen (einen 200 HTTP-Statuscode zurückgibt), die dieser Regel entspricht.|
|Aktion|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Aktion. Mögliche Werte: sind `connect`, `evaluateConnection`, `ignore` und `disconnect`.|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Domäne-Aktion (gilt nur bei der Aktion Verbindung bewerten ist). Mögliche Werte sind: `connectIfNeeded` und `neverConnect`.|
|Domänen|Collection von Objekten des Typs „String“|Domänen (gilt nur bei der Aktion Verbindung bewerten ist).|
|probeRequiredUrl|Zeichenfolge|Prüfpunkt erforderliche Url (gilt nur bei der Aktion wird Verbindung bewerten und DomainAction ist eine Verbindung herstellen, falls erforderlich).|

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






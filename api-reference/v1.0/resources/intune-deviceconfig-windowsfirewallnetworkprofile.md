---
title: Ressourcentyp „windowsFirewallNetworkProfile“
description: Richtlinien im Windows-Firewall-Profil
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 75e76e0cd4789f8e2f760d0bdc423fe15378ed67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867032"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Ressourcentyp „windowsFirewallNetworkProfile“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Richtlinien im Windows-Firewall-Profil
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Konfiguriert das Host-Gerät zum Zulassen oder Sperren der Firewall und Erzwingung der erweiterten Sicherheit für das Netzwerkprofil. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|stealthModeBlocked|Boolean|Verhindern Sie, dass des Servers Betrieb unbemerkt ausgeführt. Wenn StealthModeRequired und StealthModeBlocked sind beide true StealthModeBlocked Vorrang.|
|incomingTrafficBlocked|Boolean|Konfiguriert die Firewall, um alle eingehenden Datenverkehr unabhängig von anderen Richtlinieneinstellungen zu blockieren. Wenn IncomingTrafficRequired und IncomingTrafficBlocked sind beide true IncomingTrafficBlocked Vorrang.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Konfiguriert die Firewall zum Blockieren Unicast-Antworten auf multicast broadcast-Verkehr an. Wenn UnicastResponsesToMulticastBroadcastsRequired und UnicastResponsesToMulticastBroadcastsBlocked sind beide true UnicastResponsesToMulticastBroadcastsBlocked Vorrang.|
|inboundNotificationsBlocked|Boolean|Verhindert, dass die Firewall Benachrichtigungen anzeigen, wenn eine Anwendung einen Port Abhören blockiert wird. Wenn InboundNotificationsRequired und InboundNotificationsBlocked sind beide true InboundNotificationsBlocked Vorrang.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall, um den autorisierten Anwendungsregeln aus der Gruppenrichtlinie, mit denen aus lokalen Speicher anstelle von ignoriert die lokalen Speicher Regeln zusammenführen. Wenn AuthorizedApplicationRulesFromGroupPolicyNotMerged und AuthorizedApplicationRulesFromGroupPolicyMerged sind beide true AuthorizedApplicationRulesFromGroupPolicyMerged Vorrang.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall, um das Zusammenführen von globalen Portregeln aus der Gruppenrichtlinie mit denen aus lokalen Speicher, anstatt die lokalen Speicher Regeln werden ignoriert. Wenn GlobalPortRulesFromGroupPolicyNotMerged und GlobalPortRulesFromGroupPolicyMerged sind beide true GlobalPortRulesFromGroupPolicyMerged Vorrang.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall, um die Verbindungssicherheitsregeln von Gruppenrichtlinien mit denen aus lokalen Speicher anstelle von ignoriert die lokalen Speicher Regeln zusammenführen. Wenn ConnectionSecurityRulesFromGroupPolicyNotMerged und ConnectionSecurityRulesFromGroupPolicyMerged sind beide true ConnectionSecurityRulesFromGroupPolicyMerged Vorrang.|
|outboundConnectionsBlocked|Boolean|Konfiguriert die Firewall, um alle ausgehenden Verbindungen standardmäßig blockieren. Wenn OutboundConnectionsRequired und OutboundConnectionsBlocked sind beide true OutboundConnectionsBlocked Vorrang.|
|inboundConnectionsBlocked|Boolean|Konfiguriert die Firewall, um alle eingehenden Verbindungen standardmäßig blockieren. Wenn InboundConnectionsRequired und InboundConnectionsBlocked sind beide true InboundConnectionsBlocked Vorrang.|
|securedPacketExemptionAllowed|Boolean|Konfigurieren der Firewall zum Zulassen der Hostcomputer auf der Anzahl unerwünschter Netzwerkverkehr reagieren, dass IPSec Datenverkehr gesichert wird, auch wenn StealthModeBlocked festgelegt ist auf "true". Wenn SecuredPacketExemptionBlocked und SecuredPacketExemptionAllowed sind beide true SecuredPacketExemptionAllowed Vorrang.|
|policyRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall zum Zusammenführen Firewallregel Richtlinien aus der Gruppenrichtlinie, mit denen aus lokalen Speicher, anstatt die lokalen Speicher Regeln werden ignoriert. Wenn PolicyRulesFromGroupPolicyNotMerged und PolicyRulesFromGroupPolicyMerged sind beide true PolicyRulesFromGroupPolicyMerged Vorrang.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeBlocked": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "policyRulesFromGroupPolicyMerged": true
}
```




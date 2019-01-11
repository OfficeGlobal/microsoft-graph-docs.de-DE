---
title: Ressourcentyp „windowsFirewallNetworkProfile“
description: Richtlinien im Windows-Firewall-Profil
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8f6431d1a19c2e74dd2cf009ee433f10dc9ecb51
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877063"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Ressourcentyp „windowsFirewallNetworkProfile“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Richtlinien im Windows-Firewall-Profil
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Konfiguriert das Host-Gerät zum Zulassen oder Sperren der Firewall und Erzwingung der erweiterten Sicherheit für das Netzwerkprofil. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|stealthModeRequired|Boolean|Kann der Server für den Betrieb unbemerkt ausgeführt. Wenn StealthModeRequired und StealthModeBlocked sind beide true StealthModeBlocked Vorrang.|
|stealthModeBlocked|Boolean|Verhindern Sie, dass des Servers Betrieb unbemerkt ausgeführt. Wenn StealthModeRequired und StealthModeBlocked sind beide true StealthModeBlocked Vorrang.|
|incomingTrafficRequired|Boolean|Konfiguriert den Firewall zum Zulassen von eingehendem Datenverkehr nach anderen Einstellungen für die Informationsverwaltungsrichtlinie. Wenn IncomingTrafficRequired und IncomingTrafficBlocked sind beide true IncomingTrafficBlocked Vorrang.|
|incomingTrafficBlocked|Boolean|Konfiguriert die Firewall, um alle eingehenden Datenverkehr unabhängig von anderen Richtlinieneinstellungen zu blockieren. Wenn IncomingTrafficRequired und IncomingTrafficBlocked sind beide true IncomingTrafficBlocked Vorrang.|
|unicastResponsesToMulticastBroadcastsRequired|Boolean|Konfiguriert die Firewall, um Unicast-Antworten auf multicast broadcast-Datenverkehr zu ermöglichen. Wenn UnicastResponsesToMulticastBroadcastsRequired und UnicastResponsesToMulticastBroadcastsBlocked sind beide true UnicastResponsesToMulticastBroadcastsBlocked Vorrang.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Konfiguriert die Firewall zum Blockieren Unicast-Antworten auf multicast broadcast-Verkehr an. Wenn UnicastResponsesToMulticastBroadcastsRequired und UnicastResponsesToMulticastBroadcastsBlocked sind beide true UnicastResponsesToMulticastBroadcastsBlocked Vorrang.|
|inboundNotificationsRequired|Boolean|Kann die Firewall Benachrichtigungen angezeigt wird, wenn eine Anwendung einen Port Abhören blockiert wird. Wenn InboundNotificationsRequired und InboundNotificationsBlocked sind beide true InboundNotificationsBlocked Vorrang.|
|inboundNotificationsBlocked|Boolean|Verhindert, dass die Firewall Benachrichtigungen anzeigen, wenn eine Anwendung einen Port Abhören blockiert wird. Wenn InboundNotificationsRequired und InboundNotificationsBlocked sind beide true InboundNotificationsBlocked Vorrang.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall, um den autorisierten Anwendungsregeln aus der Gruppenrichtlinie, mit denen aus lokalen Speicher anstelle von ignoriert die lokalen Speicher Regeln zusammenführen. Wenn AuthorizedApplicationRulesFromGroupPolicyNotMerged und AuthorizedApplicationRulesFromGroupPolicyMerged sind beide true AuthorizedApplicationRulesFromGroupPolicyMerged Vorrang.|
|authorizedApplicationRulesFromGroupPolicyNotMerged|Boolean|Konfigurieren der Firewall zum Zusammenführen von autorisierten Anwendung zu verhindern, dass Regeln aus der Gruppenrichtlinie mit denen aus lokalen Speicher anstelle der lokalen Kopie ignorieren Regeln zu speichern. Wenn AuthorizedApplicationRulesFromGroupPolicyNotMerged und AuthorizedApplicationRulesFromGroupPolicyMerged sind beide true AuthorizedApplicationRulesFromGroupPolicyMerged Vorrang.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall, um das Zusammenführen von globalen Portregeln aus der Gruppenrichtlinie mit denen aus lokalen Speicher, anstatt die lokalen Speicher Regeln werden ignoriert. Wenn GlobalPortRulesFromGroupPolicyNotMerged und GlobalPortRulesFromGroupPolicyMerged sind beide true GlobalPortRulesFromGroupPolicyMerged Vorrang.|
|globalPortRulesFromGroupPolicyNotMerged|Boolean|Konfiguriert die Firewall, um zu verhindern, dass beim Zusammenführen der globalen Portregeln aus der Gruppenrichtlinie mit denen aus lokalen Speicher, anstatt die lokalen Speicher Regeln werden ignoriert. Wenn GlobalPortRulesFromGroupPolicyNotMerged und GlobalPortRulesFromGroupPolicyMerged sind beide true GlobalPortRulesFromGroupPolicyMerged Vorrang.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall, um die Verbindungssicherheitsregeln von Gruppenrichtlinien mit denen aus lokalen Speicher anstelle von ignoriert die lokalen Speicher Regeln zusammenführen. Wenn ConnectionSecurityRulesFromGroupPolicyNotMerged und ConnectionSecurityRulesFromGroupPolicyMerged sind beide true ConnectionSecurityRulesFromGroupPolicyMerged Vorrang.|
|connectionSecurityRulesFromGroupPolicyNotMerged|Boolean|Konfigurieren der Firewall zum Zusammenführen von verhindern Verbindungssicherheitsregeln von Gruppenrichtlinien mit denen aus lokalen Speicher anstelle der lokalen Kopie ignorieren Regeln zu speichern. Wenn ConnectionSecurityRulesFromGroupPolicyNotMerged und ConnectionSecurityRulesFromGroupPolicyMerged sind beide true ConnectionSecurityRulesFromGroupPolicyMerged Vorrang.|
|outboundConnectionsRequired|Boolean|Konfiguriert die Firewall, um standardmäßig alle ausgehende Verbindungen zu ermöglichen. Wenn OutboundConnectionsRequired und OutboundConnectionsBlocked sind beide true OutboundConnectionsBlocked Vorrang.|
|outboundConnectionsBlocked|Boolean|Konfiguriert die Firewall, um alle ausgehenden Verbindungen standardmäßig blockieren. Wenn OutboundConnectionsRequired und OutboundConnectionsBlocked sind beide true OutboundConnectionsBlocked Vorrang.|
|inboundConnectionsRequired|Boolean|Konfiguriert die Firewall, um alle eingehenden Verbindungen standardmäßig zu ermöglichen. Wenn InboundConnectionsRequired und InboundConnectionsBlocked sind beide true InboundConnectionsBlocked Vorrang.|
|inboundConnectionsBlocked|Boolean|Konfiguriert die Firewall, um alle eingehenden Verbindungen standardmäßig blockieren. Wenn InboundConnectionsRequired und InboundConnectionsBlocked sind beide true InboundConnectionsBlocked Vorrang.|
|securedPacketExemptionAllowed|Boolean|Konfigurieren der Firewall zum Zulassen der Hostcomputer auf der Anzahl unerwünschter Netzwerkverkehr reagieren, dass IPSec Datenverkehr gesichert wird, auch wenn StealthModeBlocked festgelegt ist auf "true". Wenn SecuredPacketExemptionBlocked und SecuredPacketExemptionAllowed sind beide true SecuredPacketExemptionAllowed Vorrang.|
|securedPacketExemptionBlocked|Boolean|Konfigurieren der Firewall zum Blockieren des Hostcomputer um unerwünschte Netzwerkdatenverkehr zu beantworten, dass IPSec Datenverkehr gesichert wird, auch wenn StealthModeBlocked festgelegt ist auf "true". Wenn SecuredPacketExemptionBlocked und SecuredPacketExemptionAllowed sind beide true SecuredPacketExemptionAllowed Vorrang.|
|policyRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall zum Zusammenführen Firewallregel Richtlinien aus der Gruppenrichtlinie, mit denen aus lokalen Speicher, anstatt die lokalen Speicher Regeln werden ignoriert. Wenn PolicyRulesFromGroupPolicyNotMerged und PolicyRulesFromGroupPolicyMerged sind beide true PolicyRulesFromGroupPolicyMerged Vorrang.|
|policyRulesFromGroupPolicyNotMerged|Boolean|Konfigurieren der Firewall zum Zusammenführen von Firewallregel zu verhindern, dass Richtlinien aus der Gruppenrichtlinie, mit denen aus lokalen Speicher anstelle der lokalen Kopie ignorieren Regeln zu speichern. Wenn PolicyRulesFromGroupPolicyNotMerged und PolicyRulesFromGroupPolicyMerged sind beide true PolicyRulesFromGroupPolicyMerged Vorrang.|

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
  "stealthModeRequired": true,
  "stealthModeBlocked": true,
  "incomingTrafficRequired": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsRequired": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsRequired": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyNotMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyNotMerged": true,
  "outboundConnectionsRequired": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsRequired": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "securedPacketExemptionBlocked": true,
  "policyRulesFromGroupPolicyMerged": true,
  "policyRulesFromGroupPolicyNotMerged": true
}
```






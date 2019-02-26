---
title: Ressourcentyp „windowsFirewallNetworkProfile“
description: Richtlinien im Windows-Firewall-Profil
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae504c8224be18766da49108a3b80c5aecb48b71
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149777"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Ressourcentyp „windowsFirewallNetworkProfile“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Richtlinien im Windows-Firewall-Profil

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Konfiguriert das Host Gerät so, dass die Firewall und die erweiterte Sicherheits Erzwingung für das Netzwerkprofil zugelassen oder blockiert werden. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|stealthModeRequired|Boolean|Der Server kann im Stealth-Modus betrieben werden. Wenn StealthModeRequired und StealthModeBlocked beide true sind, hat StealthModeBlocked Priorität.|
|stealthModeBlocked|Boolean|Verhindern, dass der Server im Stealth-Modus betrieben wird. Wenn StealthModeRequired und StealthModeBlocked beide true sind, hat StealthModeBlocked Priorität.|
|incomingTrafficRequired|Boolean|Konfiguriert die Firewall so, dass eingehender Datenverkehr gemäß anderen Richtlinieneinstellungen zugelassen wird. Wenn IncomingTrafficRequired und IncomingTrafficBlocked beide true sind, hat IncomingTrafficBlocked Priorität.|
|incomingTrafficBlocked|Boolean|Konfiguriert die Firewall so, dass der gesamte eingehende Datenverkehr unabhängig von anderen Richtlinieneinstellungen blockiert wird. Wenn IncomingTrafficRequired und IncomingTrafficBlocked beide true sind, hat IncomingTrafficBlocked Priorität.|
|unicastResponsesToMulticastBroadcastsRequired|Boolean|Konfiguriert die Firewall so, dass Unicast-Antworten auf Multicast-Broadcastdatenverkehr zulässig sind. Wenn UnicastResponsesToMulticastBroadcastsRequired und UnicastResponsesToMulticastBroadcastsBlocked beide true sind, hat UnicastResponsesToMulticastBroadcastsBlocked Priorität.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Konfiguriert die Firewall so, dass Unicast-Antworten auf Multicast-Broadcastdatenverkehr blockiert werden. Wenn UnicastResponsesToMulticastBroadcastsRequired und UnicastResponsesToMulticastBroadcastsBlocked beide true sind, hat UnicastResponsesToMulticastBroadcastsBlocked Priorität.|
|inboundNotificationsRequired|Boolean|Ermöglicht es der Firewall, Benachrichtigungen anzuzeigen, wenn eine Anwendung blockiert wird, um einen Anschluß zu überwachen. Wenn InboundNotificationsRequired und InboundNotificationsBlocked beide true sind, hat InboundNotificationsBlocked Priorität.|
|inboundNotificationsBlocked|Boolean|Verhindert, dass die Firewall Benachrichtigungen anzeigt, wenn eine Anwendung blockiert wird, um einen Anschluß zu überwachen. Wenn InboundNotificationsRequired und InboundNotificationsBlocked beide true sind, hat InboundNotificationsBlocked Priorität.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall so, dass autorisierte Anwendungsregeln aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn AuthorizedApplicationRulesFromGroupPolicyNotMerged und AuthorizedApplicationRulesFromGroupPolicyMerged beide true sind, hat AuthorizedApplicationRulesFromGroupPolicyMerged Priorität.|
|authorizedApplicationRulesFromGroupPolicyNotMerged|Boolean|Konfiguriert die Firewall, um zu verhindern, dass autorisierte Anwendungsregeln aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn AuthorizedApplicationRulesFromGroupPolicyNotMerged und AuthorizedApplicationRulesFromGroupPolicyMerged beide true sind, hat AuthorizedApplicationRulesFromGroupPolicyMerged Priorität.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall so, dass globale Portregel aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn GlobalPortRulesFromGroupPolicyNotMerged und GlobalPortRulesFromGroupPolicyMerged beide true sind, hat GlobalPortRulesFromGroupPolicyMerged Priorität.|
|globalPortRulesFromGroupPolicyNotMerged|Boolean|Konfiguriert die Firewall so, dass das Zusammenführen globaler Portregel aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher nicht ignoriert wird. Wenn GlobalPortRulesFromGroupPolicyNotMerged und GlobalPortRulesFromGroupPolicyMerged beide true sind, hat GlobalPortRulesFromGroupPolicyMerged Priorität.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall so, dass Verbindungssicherheitsregeln aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn ConnectionSecurityRulesFromGroupPolicyNotMerged und ConnectionSecurityRulesFromGroupPolicyMerged beide true sind, hat ConnectionSecurityRulesFromGroupPolicyMerged Priorität.|
|connectionSecurityRulesFromGroupPolicyNotMerged|Boolean|Konfiguriert die Firewall, um zu verhindern, dass Verbindungssicherheitsregeln aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn ConnectionSecurityRulesFromGroupPolicyNotMerged und ConnectionSecurityRulesFromGroupPolicyMerged beide true sind, hat ConnectionSecurityRulesFromGroupPolicyMerged Priorität.|
|outboundConnectionsRequired|Boolean|Konfiguriert die Firewall so, dass alle ausgehenden Verbindungen standardmäßig zugelassen werden. Wenn OutboundConnectionsRequired und OutboundConnectionsBlocked beide true sind, hat OutboundConnectionsBlocked Priorität.|
|outboundConnectionsBlocked|Boolean|Konfiguriert die Firewall so, dass alle ausgehenden Verbindungen standardmäßig blockiert werden. Wenn OutboundConnectionsRequired und OutboundConnectionsBlocked beide true sind, hat OutboundConnectionsBlocked Priorität.|
|inboundConnectionsRequired|Boolean|Konfiguriert die Firewall so, dass alle eingehenden Verbindungen standardmäßig zugelassen werden. Wenn InboundConnectionsRequired und InboundConnectionsBlocked beide true sind, hat InboundConnectionsBlocked Priorität.|
|inboundConnectionsBlocked|Boolean|Konfiguriert die Firewall so, dass alle eingehenden Verbindungen standardmäßig blockiert werden. Wenn InboundConnectionsRequired und InboundConnectionsBlocked beide true sind, hat InboundConnectionsBlocked Priorität.|
|securedPacketExemptionAllowed|Boolean|Konfiguriert die Firewall so, dass der Hostcomputer auf unangeforderten Netzwerkdatenverkehr dieses Datenverkehrs reagiert, auch wenn stealthModeBlocked auf true festgelegt ist. Wenn SecuredPacketExemptionBlocked und SecuredPacketExemptionAllowed beide true sind, hat SecuredPacketExemptionAllowed Priorität.|
|securedPacketExemptionBlocked|Boolean|Konfiguriert die Firewall, um zu verhindern, dass der Hostcomputer auf unangeforderten Netzwerkdatenverkehr dieses Datenverkehrs reagiert, auch wenn stealthModeBlocked auf true festgelegt ist. Wenn SecuredPacketExemptionBlocked und SecuredPacketExemptionAllowed beide true sind, hat SecuredPacketExemptionAllowed Priorität.|
|policyRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall so, dass Firewall-Regelrichtlinien aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn PolicyRulesFromGroupPolicyNotMerged und PolicyRulesFromGroupPolicyMerged beide true sind, hat PolicyRulesFromGroupPolicyMerged Priorität.|
|policyRulesFromGroupPolicyNotMerged|Boolean|Konfiguriert die Firewall, um zu verhindern, dass Firewall-Regelrichtlinien aus der Gruppenrichtlinie mit denen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn PolicyRulesFromGroupPolicyNotMerged und PolicyRulesFromGroupPolicyMerged beide true sind, hat PolicyRulesFromGroupPolicyMerged Priorität.|

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





---
title: Ressourcentyp „windowsFirewallNetworkProfile“
description: Richtlinien im Windows-Firewall-Profil
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e52555d8ac9b010028ee3bc716255db8a563e73
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250957"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Ressourcentyp „windowsFirewallNetworkProfile“

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Richtlinien im Windows-Firewall-Profil

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Konfiguriert das Host Gerät so, dass die Firewall und die erweiterte Sicherheits Erzwingung für das Netzwerkprofil zugelassen oder blockiert werden. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|stealthModeBlocked|Boolean|Verhindern, dass der Server im Stealth-Modus betrieben wird. Wenn StealthModeRequired und StealthModeBlocked beide true sind, hat StealthModeBlocked Priorität.|
|incomingTrafficBlocked|Boolean|Konfiguriert die Firewall so, dass der gesamte eingehende Datenverkehr unabhängig von anderen Richtlinieneinstellungen blockiert wird. Wenn IncomingTrafficRequired und IncomingTrafficBlocked beide true sind, hat IncomingTrafficBlocked Priorität.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Konfiguriert die Firewall so, dass Unicast-Antworten auf Multicast-Broadcastdatenverkehr blockiert werden. Wenn UnicastResponsesToMulticastBroadcastsRequired und UnicastResponsesToMulticastBroadcastsBlocked beide true sind, hat UnicastResponsesToMulticastBroadcastsBlocked Priorität.|
|inboundNotificationsBlocked|Boolean|Verhindert, dass die Firewall Benachrichtigungen anzeigt, wenn eine Anwendung blockiert wird, um einen Anschluß zu überwachen. Wenn InboundNotificationsRequired und InboundNotificationsBlocked beide true sind, hat InboundNotificationsBlocked Priorität.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall so, dass autorisierte Anwendungsregeln aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn AuthorizedApplicationRulesFromGroupPolicyNotMerged und AuthorizedApplicationRulesFromGroupPolicyMerged beide true sind, hat AuthorizedApplicationRulesFromGroupPolicyMerged Priorität.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall so, dass globale Portregel aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn GlobalPortRulesFromGroupPolicyNotMerged und GlobalPortRulesFromGroupPolicyMerged beide true sind, hat GlobalPortRulesFromGroupPolicyMerged Priorität.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall so, dass Verbindungssicherheitsregeln aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn ConnectionSecurityRulesFromGroupPolicyNotMerged und ConnectionSecurityRulesFromGroupPolicyMerged beide true sind, hat ConnectionSecurityRulesFromGroupPolicyMerged Priorität.|
|outboundConnectionsBlocked|Boolean|Konfiguriert die Firewall so, dass alle ausgehenden Verbindungen standardmäßig blockiert werden. Wenn OutboundConnectionsRequired und OutboundConnectionsBlocked beide true sind, hat OutboundConnectionsBlocked Priorität.|
|inboundConnectionsBlocked|Boolean|Konfiguriert die Firewall so, dass alle eingehenden Verbindungen standardmäßig blockiert werden. Wenn InboundConnectionsRequired und InboundConnectionsBlocked beide true sind, hat InboundConnectionsBlocked Priorität.|
|securedPacketExemptionAllowed|Boolean|Konfiguriert die Firewall so, dass der Hostcomputer auf unangeforderten Netzwerkdatenverkehr dieses Datenverkehrs reagiert, auch wenn stealthModeBlocked auf true festgelegt ist. Wenn SecuredPacketExemptionBlocked und SecuredPacketExemptionAllowed beide true sind, hat SecuredPacketExemptionAllowed Priorität.|
|policyRulesFromGroupPolicyMerged|Boolean|Konfiguriert die Firewall so, dass Firewall-Regelrichtlinien aus der Gruppenrichtlinie mit diesen aus dem lokalen Speicher zusammengeführt werden, statt die Regeln des lokalen Speichers zu ignorieren. Wenn PolicyRulesFromGroupPolicyNotMerged und PolicyRulesFromGroupPolicyMerged beide true sind, hat PolicyRulesFromGroupPolicyMerged Priorität.|

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




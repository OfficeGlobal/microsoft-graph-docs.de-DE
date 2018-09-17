# <a name="windowsfirewallnetworkprofile-resource-type"></a>Ressourcentyp „windowsFirewallNetworkProfile“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Richtlinien im Windows-Firewall-Profil
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Konfiguriert das Host-Gerät zum Zulassen oder Blockieren der Firewall und Erzwingung der erweiterten Sicherheit für das Netzwerkprofil. Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.|
|stealthModeBlocked|boolesch|Verhindert, dass der Server im geschützten Modus arbeitet. Wenn StealthModeRequired und StealthModeBlocked beide auf true gesetzt sind, so hat StealthModeBlocked Vorrang.|
|incomingTrafficBlocked|boolesch|Konfiguriert die Firewall so, dass sämtlicher eingehender Datenverkehr blockiert wird, unabhängig von anderen Richtlinieneinstellungen. Wenn IncomingTrafficRequired und IncomingTrafficBlocked beide auf true gesetzt sind, so hat IncomingTrafficBlocked Vorrang.|
|unicastResponsesToMulticastBroadcastsBlocked|boolesch|Konfiguriert die Firewall so, dass Unicastantworten auf Multicast-Broadcastdatenverkehr blockiert werden. Wenn UnicastResponsesToMulticastBroadcastsRequired und UnicastResponsesToMulticastBroadcastsBlocked beide auf true gesetzt sind, so hat UnicastResponsesToMulticastBroadcastsBlocked Vorrang.|
|inboundNotificationsBlocked|boolesch|Verhindert, dass die Firewall Benachrichtigungen anzeigt, sobald eine Anwendung nicht mehr auf einem Port zuhören darf. Wenn InboundNotificationsRequired und InboundNotificationsBlocked beide auf true gesetzt sind, so hat InboundNotificationsBlocked Vorrang.|
|authorizedApplicationRulesFromGroupPolicyMerged|boolesch|Konfiguriert die Firewall so, dass autorisierte Anwendungsregeln aus Gruppenrichtlinien mit den Regeln aus dem lokalen Speicher zusammengeführt werden. Die Regeln im lokalen Speicher werden also nicht mehr ignoriert. Wenn AuthorizedApplicationRulesFromGroupPolicyNotMerged und AuthorizedApplicationRulesFromGroupPolicyMerged beide auf true gesetzt sind, so hat AuthorizedApplicationRulesFromGroupPolicyMerged Vorrang.|
|globalPortRulesFromGroupPolicyMerged|boolesch|Konfiguriert die Firewall so, dass globale Portregeln aus Gruppenrichtlinien mit den Regeln aus dem lokalen Speicher zusammengeführt werden. Die Regeln im lokalen Speicher werden also nicht mehr ignoriert. Wenn GlobalPortRulesFromGroupPolicyNotMerged und GlobalPortRulesFromGroupPolicyMerged beide auf true gesetzt sind, so hat GlobalPortRulesFromGroupPolicyMerged Vorrang.|
|connectionSecurityRulesFromGroupPolicyMerged|boolesch|Konfiguriert die Firewall so, dass Verbindungssicherheitsregeln aus Gruppenrichtlinien mit den Regeln aus dem lokalen Speicher zusammengeführt werden. Die Regeln im lokalen Speicher werden also nicht mehr ignoriert. Wenn ConnectionSecurityRulesFromGroupPolicyNotMerged und ConnectionSecurityRulesFromGroupPolicyMerged beide auf true gesetzt sind, so hat ConnectionSecurityRulesFromGroupPolicyMerged Vorrang.|
|outboundConnectionsBlocked|boolesch|Konfiguriert die Firewall so, dass alle ausgehenden Verbindungen standardmäßig blockiert werden. Wenn OutboundConnectionsRequired und OutboundConnectionsBlocked beide auf true gesetzt sind, so hat OutboundConnectionsBlocked Vorrang.|
|inboundConnectionsBlocked|boolesch|Konfiguriert die Firewall so, dass alle eingehenden Verbindungen standardmäßig blockiert werden. Wenn InboundConnectionsRequired und InboundConnectionsBlocked beide auf true gesetzt sind, so hat InboundConnectionsBlocked Vorrang.|
|securedPacketExemptionAllowed|boolesch|Konfiguriert die Firewall so, dass der Hostcomputer auch dann auf unaufgefordert gesendeten Netzwerkdatenverkehr antworten darf, wenn „stealthModeBlocked“ auf „true“ gesetzt ist, vorausgesetzt, der Datenverkehr ist IPsec-gesichert. Wenn SecuredPacketExemptionBlocked und SecuredPacketExemptionAllowed beide auf true gesetzt sind, so hat SecuredPacketExemptionAllowed Vorrang.|
|policyRulesFromGroupPolicyMerged|boolesch|Konfiguriert die Firewall so, dass Firewallregelrichtlinien aus Gruppenrichtlinien mit den Richtlinien aus dem lokalen Speicher zusammengeführt werden. Die Richtlinien im lokalen Speicher werden also nicht mehr ignoriert. Wenn PolicyRulesFromGroupPolicyNotMerged und PolicyRulesFromGroupPolicyMerged beide auf true gesetzt sind, so hat PolicyRulesFromGroupPolicyMerged Vorrang.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}-->
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









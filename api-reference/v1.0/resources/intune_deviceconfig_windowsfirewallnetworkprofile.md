# <a name="windowsfirewallnetworkprofile-resource-type"></a>Ressourcentyp „windowsFirewallNetworkProfile“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Richtlinien im Windows-Firewall-Profil
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Aktiviert die Firewall sowie die Durchsetzung erweiterter Sicherheitsoptionen. Die möglichen Werte sind: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|boolesch|Verhindert, dass der Server im geschützten Modus arbeitet.|
|incomingTrafficBlocked|boolesch|Konfiguriert die Firewall so, dass sämtlicher eingehender Datenverkehr blockiert wird, unabhängig von anderen Richtlinieneinstellungen.|
|unicastResponsesToMulticastBroadcastsBlocked|boolesch|Konfiguriert die Firewall so, dass Unicastantworten auf Multicast-Broadcastdatenverkehr blockiert werden.|
|inboundNotificationsBlocked|boolesch|Verhindert, dass die Firewall Benachrichtigungen anzeigt, sobald eine Anwendung nicht mehr auf einem Port lauschen darf.|
|authorizedApplicationRulesFromGroupPolicyMerged|boolesch|Konfiguriert die Firewall so, dass autorisierte Anwendungsregeln aus Gruppenrichtlinien mit den Regeln aus dem lokalen Speicher zusammengeführt werden. Die Regeln im lokalen Speicher werden also nicht mehr ignoriert.|
|globalPortRulesFromGroupPolicyMerged|boolesch|Konfiguriert die Firewall so, dass globale Portregeln aus Gruppenrichtlinien mit den Regeln aus dem lokalen Speicher zusammengeführt werden. Die Regeln im lokalen Speicher werden also nicht mehr ignoriert.|
|connectionSecurityRulesFromGroupPolicyMerged|boolesch|Konfiguriert die Firewall so, dass Verbindungssicherheitsregeln aus Gruppenrichtlinien mit den Regeln aus dem lokalen Speicher zusammengeführt werden. Die Regeln im lokalen Speicher werden also nicht mehr ignoriert.|
|outboundConnectionsBlocked|boolesch|Konfiguriert die Firewall so, dass alle ausgehenden Verbindungen standardmäßig blockiert werden.|
|inboundConnectionsBlocked|boolesch|Konfiguriert die Firewall so, dass alle eingehenden Verbindungen standardmäßig blockiert werden.|
|securedPacketExemptionAllowed|boolesch|Konfiguriert die Firewall so, dass der Hostcomputer auch dann auf unaufgefordert gesendeten Netzwerkdatenverkehr antworten darf, wenn „stealthModeBlocked“ auf „true“ gesetzt ist, vorausgesetzt, der Datenverkehr ist IPsec-gesichert.|
|policyRulesFromGroupPolicyMerged|boolesch|Konfiguriert die Firewall so, dass Firewallregelrichtlinien aus Gruppenrichtlinien mit den Richtlinien aus dem lokalen Speicher zusammengeführt werden. Die Richtlinien im lokalen Speicher werden also nicht mehr ignoriert.|

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




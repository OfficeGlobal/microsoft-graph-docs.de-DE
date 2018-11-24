# <a name="firewallpacketqueueingmethodtype-enum-type"></a>FirewallPacketQueueingMethodType Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für firewallPacketQueueingMethod
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät|
|deaktiviert|1|Paket Warteschlangen deaktivieren|
|queueInbound|2|Eingehende, verschlüsselte Pakete Warteschlange|
|queueOutbound|3|Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung|
|queueBoth|4|Die Warteschlange eingehenden und ausgehenden Pakete|




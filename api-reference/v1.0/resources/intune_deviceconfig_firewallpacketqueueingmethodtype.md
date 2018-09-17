# <a name="firewallpacketqueueingmethodtype-enum-type"></a>FirewallPacketQueueingMethodType Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für firewallPacketQueueingMethod
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Von Intune wurde kein Wert konfiguriert, den vom Benutzer konfigurierten Standardwert für das Gerät nicht außer Kraft setzen|
|deaktiviert|1|Paket-Queuing deaktivieren|
|queueInbound|2|Eingehende verschlüsselte Pakete in Warteschlange stellen|
|queueOutbound|3|Entschlüsselte ausgehende Pakete zur Weiterleitung in Warteschlange stellen|
|queueBoth|4|Eingehende und ausgehende Pakete in Warteschlange stellen|









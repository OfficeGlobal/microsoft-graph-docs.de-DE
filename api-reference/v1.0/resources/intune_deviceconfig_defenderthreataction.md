# <a name="defenderthreataction-enum-type"></a>DefenderThreatAction Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Standard-Aktion des Defenders, um auf erkannte Malware-Bedrohungen zu reagieren.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Aktion basierend auf der Update-Definition anwenden.|
|clean|1|Die erkannte Bedrohung säubern.|
|Quarantäne|2|Die erkannte Bedrohung unter Quarantäne stellen.|
|remove|3|Erkannte Bedrohung entfernen.|
|Zulassen|4|Zulassen der erkannten Bedrohung.|
|userDefined|5|Erlaubt es dem Benutzer, die Aktion zu bestimmen, die bei einer erkannten Bedrohung durchgeführt werden soll.|
|Blockieren|6|Blockieren der erkannten Bedrohung.|




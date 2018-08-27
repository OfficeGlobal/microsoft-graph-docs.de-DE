# <a name="managedappdataencryptiontype-enum-type"></a>ManagedAppDataEncryptionType-Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt den Verschlüsselungsgrad von App-Daten für verwaltete Apps dar
## <a name="members"></a>Mitglieder
|Mitglied|Wert|Beschreibung|
|:---|:---|:---|
|useDeviceSettings|0|App-Daten werden basierend auf den Standardeinstellungen des Geräts verschlüsselt.|
|afterDeviceRestart|1|App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.|
|whenDeviceLockedExceptOpenFiles|2|App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist. Davon ausgenommen sind Daten in geöffneten Dateien.|
|whenDeviceLocked|3|App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist.|




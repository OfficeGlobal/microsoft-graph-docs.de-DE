# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState Enumerationstyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Geräte-Registrierungsstatus.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notRegistered|0|Das Gerät ist nicht registriert.|
|registered|2|Das Gerät ist registriert.|
|revoked|3|Das Gerät wurde blockiert, zurückgesetzt oder deaktiviert.|
|keyConflict|4|Das Gerät hat einen Konflikt mit einem Key.|
|approvalPending|5|Für das Gerät steht die Genehmigung noch aus.|
|certificateReset|6|Das Zertifikat des Geräts wurde zurückgesetzt.|
|notRegisteredPendingEnrollment|7|Das Gerät ist nicht registriert und die Anmeldung steht noch aus.|
|unknown|8|Der Registrierungsstatus des Geräts ist unbekannt.|




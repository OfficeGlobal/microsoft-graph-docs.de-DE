# <a name="iosupdatedevicestatus-resource-type"></a>iosUpdateDeviceStatus-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosUpdateDeviceStatuses auflisten](../api/intune_deviceconfig_iosupdatedevicestatus_list.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Objekte.|
|[iosUpdateDeviceStatus abrufen](../api/intune_deviceconfig_iosupdatedevicestatus_get.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|Lesen von Eigenschaften und Beziehungen des [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Objekts.|
|[iosUpdateDeviceStatus erstellen](../api/intune_deviceconfig_iosupdatedevicestatus_create.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|Erstellen eines neuen [IosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Objekts.|
|[iosUpdateDeviceStatus löschen](../api/intune_deviceconfig_iosupdatedevicestatus_delete.md)|Keine|Löscht einen [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).|
|[iosUpdateDeviceStatus aktualisieren](../api/intune_deviceconfig_iosupdatedevicestatus_update.md)|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)|Aktualisieren der Eigenschaften eines [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|installStatus|Zeichenfolge|Installationsstatus des Richtlinienberichts Mögliche Werte: `success`, `available`, `idle`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.|
|osVersion|Zeichenfolge|Gemeldete Geräteversion|
|deviceId|Zeichenfolge|Gemeldete Geräte-ID|
|userId|Zeichenfolge|Gemeldete Benutzer-ID|
|deviceDisplayName|Zeichenfolge|Gerätename des DevicePolicyStatus|
|userName|Zeichenfolge|Gemeldeter Benutzername|
|deviceModel|Zeichenfolge|Gemeldetes Gerätemodell|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität|
|status|Zeichenfolge|Compliance-Status des Richtlinienberichts Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|lastReportedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Richtlinienberichts|
|userPrincipalName|Zeichenfolge|Benutzer-Prinzipalname|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "String (identifier)",
  "installStatus": "String",
  "osVersion": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



# <a name="androidforworkenrollmentprofile-resource-type"></a>Ressourcentyp „androidForWorkEnrollmentProfile“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Registrierungsprofil zur Registrierung von COSU-Geräten, die Google Cloud Management verwenden
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „androidForWorkEnrollmentProfile“](../api/intune_androidforwork_androidforworkenrollmentprofile_list.md)|Sammlung von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) auf.|
|[Abrufen von „androidForWorkEnrollmentProfile“](../api/intune_androidforwork_androidforworkenrollmentprofile_get.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Erstellen von „androidForWorkEnrollmentProfile“](../api/intune_androidforwork_androidforworkenrollmentprofile_create.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Erstellt neue Objekte des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Löschen von „androidForWorkEnrollmentProfile“](../api/intune_androidforwork_androidforworkenrollmentprofile_delete.md)|Keiner|Löscht Objekte des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Aktualisieren von „androidForWorkEnrollmentProfile“](../api/intune_androidforwork_androidforworkenrollmentprofile_update.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Aktion „revokeToken“](../api/intune_androidforwork_androidforworkenrollmentprofile_revoketoken.md)|Keiner|Noch nicht dokumentiert|
|[Aktion „createToken“](../api/intune_androidforwork_androidforworkenrollmentprofile_createtoken.md)|Keiner|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|accountId|String|Mandanten-GUID, zu der das Registrierungsprofil gehört|
|id|String|Eindeutige GUID des Registrierungsprofils|
|name|String|Anzeigename des Registrierungsprofils (veraltet)|
|displayName|String|Anzeigename des Registrierungsprofils|
|description|String|Beschreibung des Registrierungsprofils|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Registrierungsprofils|
|modifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Registrierungsprofils (veraltet)|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Registrierungsprofils|
|tokenValue|String|Wert des zuletzt für das Registrierungsprofil erstellten Tokens|
|tokenExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens|
|totalEnrollmentCount|Int32|Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte (veraltet)|
|enrolledDeviceCount|Int32|Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte|
|qrCode|String|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird (veraltet)|
|qrCodeContent|String|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird|
|qrCodeImage|[mimeContent](../resources/intune_androidforwork_mimecontent.md)|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "name": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "totalEnrollmentCount": 1024,
  "enrolledDeviceCount": 1024,
  "qrCode": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




# <a name="device-resource-type"></a>Geräteressourcentyp

Stellt ein Gerät dar, das in der Organisation registriert ist. Geräte können auch mithilfe des Geräteregistrierungsdiensts oder von Intune in der Cloud erstellt werden. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. Diese Geräte können Desktopcomputer, Laptops sowie Mobiltelefone und Tablets umfassen. Erbt von [directoryObject](directoryobject.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Create device](../api/device_post_devices.md) | [Gerät](device.md) |Dient zum Erstellen eines neuen registrierten Geräts im Verzeichnis.|
|[Get device](../api/device_get.md) | [Gerät](device.md) |Dient zum Lesen der Eigenschaften und der Beziehungen eines Geräteobjekts.|
|[List devices](../api/device_list.md) | [Geräte](device.md)sammlung| Dient zum Abrufen einer Liste von Geräten, die in dem Verzeichnis registriert sind. |
|[Update device](../api/device_update.md) | [Gerät](device.md) |Dient zum Aktualisieren der Eigenschaften eines Geräteobjekts. |
|[Delete device](../api/device_delete.md) | Keine |Dient zum Löschen eines Geräteobjekts. |
|[Create registeredOwner](../api/device_post_registeredowners.md) |[directoryObject](directoryobject.md)| Dient zum Hinzufügen eines Benutzers als neuen Besitzer des Geräts durch die Veröffentlichung für die registeredOwners-Navigationseigenschaft.|
|[List registeredOwners](../api/device_list_registeredowners.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen der Benutzer, die registrierte Besitzer des Geräts in der registeredOwners-Navigationseigenschaft sind.|
|[Create registeredUser](../api/device_post_registeredusers.md) |[directoryObject](directoryobject.md)| Dient zum Hinzufügen eines registrierten Benutzers für das Gerät durch die Veröffentlichung für die registeredUsers-Navigationseigenschaft.|
|[List registeredUsers](../api/device_list_registeredusers.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen registrierter Benutzer des Geräts aus der registeredUsers-Navigationseigenschaft.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Erforderlich.|
|alternativeSecurityIds|[alternativeSecurityId](alternativesecurityid.md)-Sammlung| Der **any**-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Lässt keine Nullwerte zu. Erforderlich. |
|approximateLastSignInDateTime|DateTimeOffset| Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|deviceId|Guid| Eindeutige für den Client angegebenen GUID zur Darstellung des Geräts. Erforderlich. |
|deviceMetadata|String|    |
|deviceVersion|Int32|            |
|displayName|String|Der Anzeigename für das Gerät. Erforderlich. |
|id|String|Die eindeutige ID für das Gerät. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.|
|isCompliant|Boolean|**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**.|
|isManaged|Boolean|**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**.|
|onPremisesLastSyncDateTime|DateTimeOffset|Der Zeitpunkt der letzten Synchronisierung des Objekts mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|onPremisesSyncEnabled|Boolean|**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).|
|operatingSystem|String|Der Typ des Betriebssystems auf dem Gerät. Erforderlich. |
|operatingSystemVersion|String|Die Version des Betriebssystems auf dem Gerät. Erforderlich. |
|physicalIds|String collection| Lässt keine Nullwerte zu.            |
|trustType|String|    ||

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|registeredOwners|[directoryObject](directoryobject.md)-Sammlung|Benutzer, die registrierte Besitzer des Geräts sind. Schreibgeschützt. Lässt Nullwerte zu.|
|registeredUsers|[directoryObject](directoryobject.md)-Sammlung|Benutzer, die registrierte Benutzer des Geräts sind. Schreibgeschützt. Lässt Nullwerte zu.|



## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "trustType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

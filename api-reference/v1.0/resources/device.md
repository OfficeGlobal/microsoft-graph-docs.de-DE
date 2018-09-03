# <a name="device-resource-type"></a>Geräteressourcentyp

Stellt ein Gerät dar, das in der Organisation registriert ist. Geräte werden mithilfe des Geräteregistrierungsdiensts oder von Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. Diese Geräte können Desktopcomputer, Laptops sowie Mobiltelefone und Tablets umfassen. Erbt von [directoryObject](directoryobject.md).

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](../../../concepts/extensibility_overview.md) eigene Daten hinzuzufügen.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Get device](../api/device_get.md) | [Gerät](device.md) |Dient zum Lesen der Eigenschaften und der Beziehungen eines Geräteobjekts.|
|[List devices](../api/device_list.md) | [Geräte](device.md)sammlung| Dient zum Abrufen einer Liste von Geräten, die in dem Verzeichnis registriert sind. |
|[Update device](../api/device_update.md) | [Gerät](device.md) |Dient zum Aktualisieren der Eigenschaften eines Geräteobjekts. |
|[Delete device](../api/device_delete.md) | Keine |Dient zum Löschen eines Geräteobjekts. |
|[List registeredOwners](../api/device_list_registeredowners.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen der Benutzer, die registrierte Besitzer des Geräts in der registeredOwners-Navigationseigenschaft sind.|
|[List registeredUsers](../api/device_list_registeredusers.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen registrierter Benutzer des Geräts aus der registeredUsers-Navigationseigenschaft.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](../../../concepts/extensibility_schema_groups.md) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accountEnabled|Boolesch| **true**, wenn das Konto aktiviert ist; andernfalls **false**. Erforderlich.|
|alternativeSecurityIds|alternativeSecurityId-Sammlung| Nur für internen Gebrauch. Lässt keine Nullwerte zu. |
|approximateLastSignInDateTime|DateTimeOffset| Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'` Schreibgeschützt. |
|deviceId|Zeichenfolge| Der eindeutige Bezeichner, der vom Azure-Geräteregistrierungsdienst bei der Registrierung festgelegt wird. |
|deviceMetadata|Zeichenfolge| Nur für internen Gebrauch. Auf Null festgelegt. |
|deviceVersion|Int32| Nur für internen Gebrauch. |
|displayName|Zeichenfolge|Der Anzeigename für das Gerät. Erforderlich. |
|id|Zeichenfolge|Die eindeutige ID für das Gerät. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.|
|isCompliant|Boolesch|**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**. Schreibgeschützt. Die Aktualisierung kann für ein beliebiges Geräte-Betriebssystem nur durch Intune oder für Geräte mit Windows-Betriebssystem durch eine [genehmigte MDM-App](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) erfolgen.|
|isManaged|Boolesch|**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**. Die Aktualisierung kann für ein beliebiges Geräte-Betriebssystem nur durch Intune oder für Geräte mit Windows-Betriebssystem durch eine [genehmigte MDM-App](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) erfolgen. |
|onPremisesLastSyncDateTime|DateTimeOffset|Der Zeitpunkt der letzten Synchronisierung des Objekts mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'` Schreibgeschützt.|
|onPremisesSyncEnabled|Boolesch|**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard). Schreibgeschützt. |
|operatingSystem|Zeichenfolge| Der Typ des Betriebssystems auf dem Gerät. Erforderlich. |
|operatingSystemVersion|Zeichenfolge|Die Version des Betriebssystems auf dem Gerät. Erforderlich. |
|physicalIds|Zeichenfolgenauflistung| Nur für internen Gebrauch. Lässt keine Nullwerte zu. |
|trustType|Zeichenfolge| Typ von Vertrauensstellung für das beigetretene Gerät. Schreibgeschützt. Mögliche Werte: <br />**Arbeitsplatz** - Gibt an *, dass eigene persönliche Geräte mitgebracht werden sollen*<br />**AzureAd** - Nur Geräte, die mit der Cloud verknüpft sind<br />**ServerAd** - Lokale Geräte, die der Domäne beigetreten sind, die mit Azure AD verknüpft sind. Weitere Informationen hierzu finden Sie unter [Einführung in die Geräteverwaltung in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für das Gerät definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|
|registeredOwners|[directoryObject](directoryobject.md)-Sammlung|Der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat. Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt. Derzeit kann jeweils nur ein Besitzer vorhanden sein. Schreibgeschützt. Lässt Nullwerte zu. |
|registeredUsers|[directoryObject](directoryobject.md)-Sammlung|Auflistung von Benutzern, die registrierte Benutzer des Geräts sind. Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
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

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="contact-resource-type"></a>Ressourcentyp contact

Ein Kontakt ist ein Element in Outlook, in dem Sie Informationen über die Personen und Organisationen, mit denen Sie kommunizieren, organisieren und speichern können. Kontakte sind in Kontaktordnern enthalten.

Diese Ressource unterstützt Folgendes:

- Hinzufügen Ihrer eigenen Daten zu benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](../../../concepts/extensibility_overview.md).
- Verwenden einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/contact_delta.md)-Funktion.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Kontakt abrufen](../api/contact_get.md) | [Kontakt](contact.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des Kontaktobjekts.|
|[Erstellen](../api/user_post_contacts.md) | [Kontakt](contact.md) |Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Kontaktendpunkt eines anderen Kontaktordners.|
|[Aktualisieren](../api/contact_update.md) | [Kontakt](contact.md) |Dient zum Aktualisieren des Kontaktobjekts. |
|[Löschen](../api/contact_delete.md) | Keine |Dient zum Löschen des Kontaktobjekts. |
|[delta](../api/contact_delta.md)|[contact](contact.md)-Sammlung| Dient zum Abrufen eines Satzes von Kontakten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](../../../concepts/extensibility_schema_groups.md) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[Kontakt](contact.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Kontakt.   |
|[Ereignis mit erweiterter einwertiger Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty_get.md)  | [Kontakt](contact.md) | Ruft mithilfe von `$expand` oder `$filter` Kontakte mit einer bestimmten einwertigen erweiterten Eigenschaft ab. |
|[Erweiterte mehrwertige Eigenschaft erstellen](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [Kontakt](contact.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Kontakt.  |
|[Ereignis mit erweiterter mehrwertiger Eigenschaft abrufen](../api/multivaluelegacyextendedproperty_get.md)  | [Kontakt](contact.md) | Dient zum Abrufen eines Kontakts mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assistantName|String|Der Name des Assistenten des Kontakts.|
|birthday|DateTimeOffset|Das Geburtsdatum des Kontakts. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|businessAddress|[PhysicalAddress](physicaladdress.md)|Die Geschäftsadresse des Kontakts.|
|businessHomePage|String|Die geschäftliche Homepage des Kontakts.|
|businessPhones|String collection|Die geschäftlichen Telefonnummern des Kontakts.|
|categories|String collection|Die Kategorien, die mit dem Kontakt verknüpft sind.|
|changeKey|String|Gibt die Version des Kontakts an. Jedes Mal, wenn der Kontakt geändert wird, wird auch die Eigenschaft „changeKey“ geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.|
|children|String collection|Die Namen der Kinder des Kontakts.|
|companyName|String|Der Name des Unternehmens des Kontakts.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der Kontakt erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Abteilung|String|Die Abteilung des Kontakts.|
|displayName|String|Der Anzeigename des Kontakts.|
|emailAddresses|[EmailAddress](emailaddress.md) collection|Die E-Mail-Adressen des Kontakts.|
|Kennzeichnen|[followUpFlag](followupflag.md)|Der Wert des Flags, der den Status, das Startdatum, das Fälligkeitsdatum oder das Enddatum für die Nachricht angibt.|
|fileAs|String|Der Name, unter dem der Kontakt abgelegt ist.|
|generation|String|Die Generation des Kontakts.|
|givenName|String|Der Vorname des Kontakts.|
|homeAddress|[PhysicalAddress](physicaladdress.md)|Die Privatadresse des Kontakts.|
|homePhones|String collection|Die privaten Telefonnummern des Kontakts.|
|id|String|Eindeutiger Bezeichner für den Kontakt. Schreibgeschützt.|
|imAddresses|String collection|Instant Messaging Chatadressen des Kontakts.|
|initials|String|Die Initialen des Kontakts.|
|jobTitle|String|Die Position des Kontakts.|
|lastModifiedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der Kontakt geändert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|manager|String|Der Name des Vorgesetzten des Kontakts.
|middleName|String|Der zweite Vorname des Kontakts.|
|mobilePhone|String|Die Mobiltelefonnummer des Kontakts.|
|nickName|String|Der Spitzname des Kontakts.|
|officeLocation|String|Der Bürostandort des Kontakts.|
|otherAddress|[PhysicalAddress](physicaladdress.md)|Weitere Adressen für den Kontakt.|
|parentFolderId|String|Die ID des übergeordneten Ordners des Kontakts.|
|personalNotes|String|Die Notizen des Benutzers zu dem Kontakt.|
|profession|String|Der Beruf des Kontakts.|
|spouseName|Zeichenfolge|Der Name des Ehepartners/Partners des Kontakts|
|surname|String|Der Nachname des Kontakts.|
|title|String|Der Titel des Kontakts.|
|yomiCompanyName|String|Der phonetische japanische Firmenname des Kontakts.|
|yomiGivenName|String|Der phonetische japanische Vorname des Kontakts.|
|yomiSurname|String|Der phonetische japanische Nachname des Kontakts.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für den Kontakt definierten offenen Erweiterungen. Schreibgeschützt. Lässt NULL-Werte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Kontakt definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|
|Foto|[profilePhoto](profilephoto.md)| Optionales Kontaktbild. Sie können für einen Kontakt ein Foto abrufen oder einstellen.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für den Kontakt definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a>Siehe auch

- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](../../../concepts/delta_query_overview.md)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md)
- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

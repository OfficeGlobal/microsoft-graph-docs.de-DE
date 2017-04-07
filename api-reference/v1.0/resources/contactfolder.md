# <a name="contactfolder-resource-type"></a>Ressourcentyp contactFolder

Ein Ordner, der Kontakte enthält.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[contactFolder abrufen](../api/contactfolder_get.md) | [contactFolder](contactfolder.md) |Dient zum Abrufen eines Kontaktordners anhand der Kontaktordner-ID.|
|[Aktualisieren](../api/contactfolder_update.md) | [contactFolder](contactfolder.md) |Dient zum Aktualisieren des contactFolder-Objekts. |
|[Löschen](../api/contactfolder_delete.md) | Keine |Dient zum Löschen des contactFolder-Objekts. |
|[childFolders auflisten](../api/contactfolder_list_childfolders.md) |[ContactFolder](contactfolder.md)-Sammlung| Dient zum Abrufen einer Sammlung von untergeordneten Ordnern unter dem angegebenen Kontaktordner.|
|[Untergeordneten contactFolder erstellen](../api/contactfolder_post_childfolders.md) |[ContactFolder](contactfolder.md)| Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners.|
|[Kontakte im Ordner auflisten](../api/contactfolder_list_contacts.md) |[Contact](contact.md)-Sammlung| Dient zum Abrufen einer Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers (`.../me/contacts`) oder aus dem angegebenen Kontaktordner.|
|[Kontakt in Ordner erstellen](../api/contactfolder_post_contacts.md) |[Kontakt](contact.md)| Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.|
|[Create single-value extended property](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[contactFolder](contactFolder.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.   |
|[contactFolder mit erweiterter einwertiger Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty_get.md)  | [contactFolder](contactFolder.md) | Dient zum Abrufen von contactFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [contactFolder](contactFolder.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.  |
|[contactFolder mit erweiterter mehrwertiger Eigenschaft abrufen](../api/multivaluelegacyextendedproperty_get.md)  | [contactFolder](contactFolder.md) | Dient zum Abrufen eines contactFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |



## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|displayName|String|Der Anzeigename des Ordners.|
|id|String|Eindeutiger Bezeichner des Kontaktordners. Schreibgeschützt.|
|parentFolderId|String|Die ID des übergeordneten Ordners des Ordners.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|childFolders|[ContactFolder](contactfolder.md)-Sammlung|Die Sammlung der untergeordneten Ordner im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.|
|Kontakte|[Contact](contact.md)-Sammlung|Die Kontakte im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

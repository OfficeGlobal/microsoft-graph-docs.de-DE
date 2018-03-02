# <a name="referenceattachment-resource-type"></a>referenceAttachment-Ressourcentyp

Ein Link zu einer Datei (z. B. eine Textdatei oder ein Word-Dokument) auf einem OneDrive for Business-Cloudlaufwerk oder anderen unterstützten Speicherorten, der an ein Ereignis, eine Nachricht oder einen Beitrag angefügt ist.

Abgeleitet von [attachment](attachment.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen](../api/attachment_get.md) | [referenceAttachment](referenceattachment.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des referenceAttachment-Objekts.|
|[Delete](../api/attachment_delete.md) | Keine |Dient zum Löschen des referenceAttachment-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|contentType|String|Der Inhaltstyp der Anlage.|
|id|String|Die Anlagen-ID.  Schreibgeschützt.|
|isInline|Boolean|Wird auf „true“ festgelegt, wenn die Anlage inline im Text des einbettenden Objekts angezeigt wird.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Anlage. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|name|String|Der Text, der unter dem Symbol angezeigt wird, das die eingebettete Anlage darstellt. Dies muss nicht der tatsächliche Dateiname sein.|
|size|Int32|Die Größe der Metadaten, die in der Nachricht für die Anlage gespeichert sind, in Byte. Dieser Wert gibt nicht die Größe der tatsächlichen Datei an.|

## <a name="relationships"></a>Beziehungen
Keine



## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

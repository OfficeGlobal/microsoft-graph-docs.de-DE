# <a name="attachment-resource-type"></a>Ressourcentyp attachment

Sie können verwandte Inhalte in Form einer Anlage zu einem [Ereignis](../resources/event.md), einer [Nachricht](../resources/message.md) oder einem [Beitrag](../resources/post.md) hinzufügen.

**attachment** ist die Basisressource für die folgenden abgeleiteten Typen von Anlagen:

* Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)
* Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)
* Link zu einer Datei ([referenceAttachment](../resources/referenceAttachment.md)-Ressource)


## <a name="methods"></a>Methoden

Die folgenden Methoden gelten für alle abgeleiteten Typen von Anlagen (**fileAttachment**, **itemAttachment** oder **referenceAttachment**).

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Anlage abrufen](../api/attachment_get.md) | [attachment](attachment.md) |Lesen Sie die Eigenschaften und Beziehungen einer Anlage, die einem Ereignis, einer Nachricht oder einem Beitrag angehängt ist.|
|[Anlage einem Ereignis hinzufügen](../api/event_post_attachments.md) | [attachment](attachment.md) |Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Ereignis.|
|[Anlagen einer Nachricht hinzufügen](../api/message_post_attachments.md) | [attachment](attachment.md) |Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einer Nachricht.|
|[Anlage einem Beitrag hinzufügen](../api/post_post_attachments.md) | [attachment](attachment.md) |Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Beitrag.|
|[Anlagen eines Ereignisses auflisten](../api/event_list_attachments.md) | [attachment](attachment.md) collection | Liste der Anlagen für ein Ereignis abrufen |
|[Anlagen einer Nachricht auflisten](../api/message_list_attachments.md) | [attachment](attachment.md) collection | Liste der Anlagen für eine Nachricht abrufen |
|[Anlagen eines Beitrags auflisten](../api/post_list_attachments.md) | [attachment](attachment.md) collection | Liste der Anlagen für einen Beitrag abrufen |
|[Löschen](../api/attachment_delete.md) | Keine |Eine Anlage für ein Ereignis, eine Nachricht oder einen Beitrag löschen |


## <a name="properties"></a>Eigenschaften

Nachfolgend finden Sie die grundlegenden Eigenschaften von attachment-Ressourcen. Zusätzliche Eigenschaften finden Sie bei dem jeweiligen Anlagentyp ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) oder [referenceAttachment](../resources/referenceAttachment.md)).

| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|contentType|String|Der MIME-Typ.|
|id|String| Schreibgeschützt.|
|isInline|Boolean|`true`, wenn die Anlage eine Inlineanlage ist, andernfalls `false`.|
|lastModifiedDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|name|String|Der Dateiname der Anlage.|
|size|Int32|Die Länge der Anlage in Byte.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
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
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

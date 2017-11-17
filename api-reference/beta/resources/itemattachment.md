# <a name="itemattachment-resource-type"></a>itemAttachment-Ressourcentyp

Kontakt, Ereignis oder Nachricht, die an ein anderes Ereignis, eine andere Nachricht oder einen anderen Beitrag angefügt sind.  

Abgeleitet von [attachment](attachment.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen](../api/attachment_get.md) | [itemAttachment](itemattachment.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des itemAttachment-Objekts.|
|[Delete](../api/attachment_delete.md) | Keine |Dient zum Löschen des itemAttachment-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|contentType|String|Der Inhaltstyp der Anlage.|
|id|String| Die Anlagen-ID.|
|isInline|Boolean|Legen Sie diesen auf „true“ fest, wenn es sich um eine Inlineanlage handelt, z. B. ein eingebettetes Bild innerhalb des Textkörpers des Elements.|
|lastModifiedDateTime|DateTimeOffset|Letzte Uhrzeit und letztes Datum der Änderung der Anlage.|
|name|String|Der Anzeigename der Anlage.|
|size|Int32|Die Größe der Anlage in Byte.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|item|[OutlookItem](outlookitem.md)|Die angefügte Nachricht oder das angefügte Ereignis. Navigation-Eigenschaft|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
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
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

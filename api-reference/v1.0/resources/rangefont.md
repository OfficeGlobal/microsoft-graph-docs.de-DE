# <a name="rangefont-resource-type"></a>RangeFont-Ressourcentyp

Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeFont abrufen](../api/rangefont_get.md) | [WorkbookRangeFont](rangefont.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFont-Objekts.|
|[Aktualisieren](../api/rangefont_update.md) | [WorkbookRangeFont](rangefont.md)   |Dient zum Aktualisieren des RangeFont-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fett|boolesch|Stellt den Fett-Status der Schriftart dar.|
|Farbe|Zeichenfolge|HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.|
|kursiv|boolesch|Stellt den Kursiv-Status der Schriftart dar.|
|Name|Zeichenfolge|Schriftartname (z. B. "Calibri")|
|Größe|doppelt|Schriftgrad|
|unterstrichen|Zeichenfolge|Art der Unterstreichung für die Schriftart. Mögliche Werte sind: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
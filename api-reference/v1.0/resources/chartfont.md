# <a name="chartfont-resource-type"></a>ChartFont-Ressourcentyp

Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartFont abrufen](../api/chartfont_get.md) | [WorkbookChartFont](chartfont.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartFont-Objekts.|
|[Aktualisieren](../api/chartfont_update.md) | [WorkbookChartFont](chartfont.md)   |Dient zum Aktualisieren des ChartFont-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fett|boolesch|Stellt den Fett-Status der Schriftart dar.|
|farbe|Zeichenfolge|HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.|
|kursiv|boolesch|Stellt den Kursiv-Status der Schriftart dar.|
|Name|Zeichenfolge|Schriftartname (z. B. "Calibri")|
|Größe|doppelt|Der Schriftgrad (z. B. 11)|
|unterstreichen|Zeichenfolge|Art der Unterstreichung für die Schriftart. Die möglichen Werte sind: `None`, `Single`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
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
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
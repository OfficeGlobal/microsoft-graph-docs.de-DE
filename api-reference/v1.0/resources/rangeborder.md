# <a name="rangeborder-resource-type"></a>RangeBorder-Ressourcentyp

Stellt den Rahmen eines Objekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeBorder abrufen](../api/rangeborder_get.md) | [WorkbookRangeBorder](rangeborder.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeBorder-Objekts.|
|[Aktualisieren](../api/rangeborder_update.md) | [WorkbookRangeBorder](rangeborder.md) |Dient zum Aktualisieren des RangeBorder-Objekts. |
|[Liste](../api/rangeborder_list.md) | [WorkbookRangeBorder](rangeborder.md)-Sammlung |Dient zum Abrufen der RangeBorder-Objeksammlung. |
|[Itemat](../api/rangebordercollection_itemat.md)|[WorkbookRangeBorder](rangeborder.md)|Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|color|Zeichenfolge|HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.|
|id|Zeichenfolge|Stellt den Bezeichner des Rahmens dar. Mögliche Werte: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Schreibgeschützt.|
|sideIndex|Zeichenfolge|Konstanter Wert, der die bestimmte Seite des Rahmens angibt. Mögliche Werte: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Schreibgeschützt.|
|Formatvorlage|Zeichenfolge|Eine der Konstanten der Linienart, die die Linienart für den Rahmen angibt. Mögliche Werte: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.|
|weight|Zeichenfolge|Gibt die Stärke des Rahmens um einen Bereich an. Die möglichen Werte sind: `Hairline`, `Thin`, `Medium`, `Thick`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
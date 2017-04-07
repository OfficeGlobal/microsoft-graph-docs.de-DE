# <a name="rangeborder-resource-type"></a>RangeBorder-Ressourcentyp

Stellt den Rahmen eines Objekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeBorder abrufen](../api/rangeborder_get.md) | [RangeBorder](rangeborder.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeBorder-Objekts.|
|[Update](../api/rangeborder_update.md) | [RangeBorder](rangeborder.md)    |Dient zum Aktualisieren des RangeBorder-Objekts. |
|[List](../api/rangeborder_list.md) | [RangeBorder-Sammlung](rangeborder.md) |Dient zum Abrufen der RangeBorder-Objeksammlung. |
|[Itemat](../api/rangebordercollection_itemat.md)|[RangeBorder](rangeborder.md)|Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|color|string|HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.|
|id|string|Stellt die Rahmen-ID dar. Mögliche Werte: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Schreibgeschützt.|
|sideIndex|string|Konstanter Wert, der die bestimmte Seite des Rahmens angibt. Mögliche Werte: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Schreibgeschützt.|
|style|string|Eine der Konstanten der Linienart, die die Linienart für den Rahmen angibt. Mögliche Werte: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.|
|weight|string|Gibt die Stärke des Rahmens um einen Bereich an. Mögliche Werte: `Hairline`, `Thin`, `Medium`, `Thick`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
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
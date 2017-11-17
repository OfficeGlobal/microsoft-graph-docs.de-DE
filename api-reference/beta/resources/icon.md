# <a name="icon-resource-type"></a>Icon-Ressourcentyp

Stellt ein Zellensymbol dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Symbol abrufen](../api/icon_get.md) | [Icon](icon.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des icon-Objekts.|
|[Update](../api/icon_update.md) | [Icon](icon.md)    |Dient zum Aktualisieren des icon-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Index|int|Stellt den Index des Symbols im angegebenen Satz dar.|
|set|string|Stellt den Satz dar, zu dem das Symbol gehört. Mögliche Werte: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.icon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
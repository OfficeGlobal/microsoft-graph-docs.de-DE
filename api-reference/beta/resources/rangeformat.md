# <a name="rangeformat-resource-type"></a>RangeFormat-Ressourcentyp

Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeFormat abrufen](../api/rangeformat_get.md) | [RangeFormat](rangeformat.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFormat-Objekts.|
|[RangeBorder erstellen](../api/rangeformat_post_borders.md) |[RangeBorder](rangeborder.md)| Dient zum Erstellen eines neues RangeBorder durch Veröffentlichen in der Rahmensammlung.|
|[Rahmen auflisten](../api/rangeformat_list_borders.md) |[RangeBorder-Sammlung](rangeborder.md)| Dient zum Abrufen einer RangeBorder-Objeksammlung.|
|[Update](../api/rangeformat_update.md) | [RangeFormat](rangeformat.md)    |Dient zum Aktualisieren des RangeFormat-Objekts. |
|[Autofitcolumns](../api/rangeformat_autofitcolumns.md)|Keine|Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.|
|[Autofitrows](../api/rangeformat_autofitrows.md)|Keine|Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|columnWidth|double|Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.|
|horizontalAlignment|string|Stellt die horizontale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.|
|rowHeight|double|Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.|
|verticalAlignment|string|Stellt die vertikale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.|
|wrapText|boolean|Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|Borders|[RangeBorder-Sammlung](rangeborder.md)|Auflistung von Border-Objekten, die für den gesamten ausgewählten Bereich gelten, schreibgeschützt.|
|fill|[RangeFill](rangefill.md)|Gibt das Fill-Objekt an, das für den gesamten Bereich definiert ist. Schreibgeschützt.|
|font|[RangeFont](rangefont.md)|Gibt das Font-Objekt zurück, das für den gesamten ausgewählten Bereich definiert ist, schreibgeschützt.|
|Schutz|[FormatProtection](formatprotection.md)|Gibt das Formatschutz-Objekt für einen Bereich zurück. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
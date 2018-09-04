# <a name="visualinfo-resource-type"></a>Ressourcentyp visualInfo

Einen komplexen Typ für die Darstellung der **VisualElements** -Eigenschaft im [Aktivität](../resources/projectrome_activity.md) -Objekt.

Die Aktivität jedes Benutzers wird in der Zeitachse als eine adaptive Karte angezeigt. App-Entwickler werden ermutigt, eine benutzerdefinierte Karte bereitzustellen, die das Wesentliche der Aktivität in Ihrer App erfasst. Dies ist möglich, indem Sie eine benutzerdefinierte JSON-Karte in der Inhaltseigenschaft bereitstellen.

Zusätzlich zu visuellen Metadaten mit einer adaptiven Karte kann die App Inhaltsmetadaten angeben - Daten, die verwendet werden, um Rückschlüsse auf die Aktivität des Benutzers zu ziehen, um neue Aktivitäten für eine zukünftige Wiederverwendung anzubieten. Dies ist möglich, indem Sie mithilfe der Eigenschaft contentInfo der Aktivität ein JSON-Objekt bereitstellen, das schema.org-Eigenschaften zur Beschreibung des Inhalts nutzt.

Wenn keine benutzerdefinierte Karte bereitgestellt wird, wird mit den Eigenschaften Textanzeige und Beschreibung eine einfache Karte generiert. Benutzerdefinierte Karten werden empfohlen, um die besten Inhalte aus Ihrer App zu präsentieren.

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:------|:-----------|
|Anzeigetext | Zeichenfolge | Erforderlich. Kurze Beschreibung der eindeutigen Aktivität des Benutzers (z. B. Dokumentname in Fällen, in denen sich eine Aktivität auf die Dokumenterstellung bezieht)|
|Beschreibung | Zeichenfolge | Optional. Längere Textbeschreibung der eindeutigen Aktivität des Benutzers (Beispiel: Dokumentname, erster Satz und / oder Metadaten)|
|Hintergrundfarbe | Zeichenfolge | Optional. Hintergrundfarbe, mit der die Aktivität in der UI - Markenfarbe für die Anwendungsquelle der Aktivität gerendert wird. Muss eine gültige Hex-Farbe sein|
|Inhalt | Nicht typisiertes JSON-Objekt | Optional. Benutzerdefiniertes Datenelement - JSON-Objekt, das zum Bereitstellen benutzerdefinierter Inhalte zum Rendern der Aktivität in der Windows-Shell-Benutzeroberfläche verwendet wird|
|Zuschreibung | [imageInfo](../resources/projectrome_imageinfo.md) | Optional. JSON-Objekt zur Darstellung eines Symbols, das die Anwendung darstellt, die zum Generieren der Aktivität verwendet wurde|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

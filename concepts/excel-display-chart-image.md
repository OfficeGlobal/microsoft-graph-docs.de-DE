# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a>Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph

Wenn Sie einen [GET-Vorgang zum Abrufen eines Diagrammbilds](/api-reference/v1.0/api/chart_image.md) ausführen, gibt die Excel-API gibt das Bild als Base-64-Zeichenfolge zurück.

Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.

Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`. Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an. So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.

## <a name="see-also"></a>Siehe auch

* [Verwalten von Sitzungen in Excel mit Microsoft Graph](excel-manage-sessions.md)
* [Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph](excel-write-to-workbook.md)
* [Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph](excel-use-functions.md)
* [Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph](excel-update-range-format.md)
* [Verwenden der Excel-REST-API](../api-reference/v1.0/resources/excel.md)

# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a>Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph

In den folgenden Beispielen wird veranschaulicht, wie die Eigenschaften der [RangeFormat](../api-reference/v1.0/resources/rangeformat.md)-, [RangeFill](../api-reference/v1.0/resources/rangefill.md)- und [RangeFont](../api-reference/v1.0/resources/rangefont.md)-Eigenschaften eines bestimmten Bereichs aktualisiert werden können.

Das Ergebnis dieser Anforderungen ist eine Tabelle mit drei formatierten Zellen, wie in der folgenden Abbildung dargestellt.

![Excel-Diagrammtabelle mit drei Zellen, deren Format-, Füllungs- und Schrifteigenschaften aktualisiert wurden.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der ersten Zelle.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "General",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der ersten Zelle.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": true,
    "color": "#4B180E",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert die Hintergrundfarbe der ersten Zelle.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert die vertikale und horizontale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der zweiten Zelle.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Center",
    "rowHeight": 49,
    "verticalAlignment": "Center",
    "wrapText": false
}
```

##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert den Schriftschnitt und Schriftgrad der zweiten Zelle.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#000000",
    "italic": true,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert die Hintergrundfarbe der zweiten Zelle.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert die horizontale Ausrichtung, die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der dritten Zelle.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Right",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der dritten Zelle. Beachten Sie, dass die Underline-Eigenschaft die Werte **Single** oder **Double** akzeptiert.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#FFFFFF",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "Single"
}
```

##### <a name="request"></a>Anforderung
Diese Anforderung aktualisiert die Hintergrundfarbe der dritten Zelle.

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#0000FF"
}
```


## <a name="see-also"></a>Siehe auch
* [Verwalten von Sitzungen in Excel mit Microsoft Graph](excel-manage-sessions.md)
* [Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph](excel-write-to-workbook.md)
* [Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph](excel-use-functions.md)
* [Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph](excel-display-chart-image.md)
* [Verwenden der Excel-REST-API](../api-reference/v1.0/resources/excel.md)

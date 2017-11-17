# <a name="resource-resource-type"></a>resource-Ressourcentyp

Ein Bild oder eine andere Dateiressource auf einer OneNote-Seite. 

Sie können die Binärdaten einer Ressource abrufen, der Abruf einer JSON-Darstellung eines Ressourcenobjekts oder einer Ressourcensammlung wird jedoch nicht unterstützt.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

Rufen Sie die Binärdaten einer bestimmten Ressource ab, indem Sie eine GET-Anforderung an den Endpunkt `content` der Ressourcen senden:

```
GET ../onenote/resources/{id}/content
```

Der Ressourcen-URI der Datei wird zurückgegeben, wenn Sie den HTML-Inhalt einer Seite mit der folgenden Anforderung abrufen:

```
GET ../onenote/pages/{id}/content
```

Im HTML-Code der Seite schließt ein `img`-Tag Endpunkte für die ursprüngliche Bildressource in das Attribut `data-fullres-src` und das optimierte Bild in das Attribut `src` ein:
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

Ein `object`-Tag (das Dateien wie PDF, DOCX und PNG darstellt) schließt den Endpunkt für die Dateiressource in das Attribut `data` ein:

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a>Eigenschaften
Keine.

## <a name="relationships"></a>Beziehungen
Keine.


## <a name="methods"></a>Methoden
| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Binärdaten von Ressource abrufen](../api/resource_get.md) | Stream |Dient zum Abrufen der Binärdaten einer Datei- oder Bildressource.|


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
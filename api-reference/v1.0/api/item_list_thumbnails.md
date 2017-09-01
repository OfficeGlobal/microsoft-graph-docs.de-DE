# <a name="list-thumbnails-for-a-driveitem"></a>Miniaturansichten für ein DriveItem auflisten

Hier erklären wir Ihnen, wie Sie eine Liste der [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen einer [DriveItem](../resources/driveitem.md)-Ressource abrufen können.

Ein DriveItem kann durch 0 oder mehr [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen repräsentiert werden. Jedes **thumbnailSet** kann ein oder mehrere [**thumbnail**](../resources/thumbnail.md)-Objekte haben. Dabei handelt es sich um Bilder, die das jeweilige Element darstellen. Beispielsweise könnte ein **thumbnailSet** gängige **thumbnail**-Objekte wie `small`, `medium` oder `large` enthalten.

Es gibt viele Möglichkeiten, auf OneDrive mit Miniaturansichten zu arbeiten. Die häufigsten:

* Enumerieren der für ein Element verfügbaren Miniaturansichten
* Abrufen einer einzelnen Miniaturansicht für ein Element
* Abrufen von Miniaturansichtinhalten
* Abrufen von Miniaturansichten für mehrere Elemente in einer einzigen Anforderung
* Abrufen von benutzerdefinierten Miniaturansichtgrößen
* Hochladen einer benutzerdefinierten Miniaturansicht für ein Element
* Ermitteln, ob eine benutzerdefinierte Miniaturansicht hochgeladen wurde


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) von `$select` zur Anpassung der Antwort.

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode einen Antwortcode des Typs `200 OK` und eine Sammlung von [ThumbnailSet](../resources/thumbnailset.md)-Objekten im Antworttext zurück.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="retrieve-a-single-thumbnail"></a>Abrufen einer einzelnen Miniaturansicht

Sie können die Metadaten einer einzelnen Miniaturansicht sowie ihre Größe abrufen, indem Sie sie in einer Anforderung direkt adressieren.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a>Pfadparameter

| Name         | Typ   | Beschreibung                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| **item-id**  | string | Der eindeutige Bezeichner für das referenzierte Element                                      |
| **thumb-id** | number | Der Index der Miniaturansicht, in der Regel 0 bis 4                                            |
| **size**     | string | Die Größe der angeforderten Miniaturansicht. Dabei muss es sich um eine der aufgeführten Standardgrößen handeln. |

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a>Abrufen von Miniaturansichtinhalten

Sie können den Inhalt einer Miniaturansicht direkt abrufen, indem Sie die Eigenschaft **content** der Miniaturansicht anfordern.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a>Antwort

Der Dienst antwortet mit einer Umleitung auf die Miniaturansicht-URL.

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

URLs zu Miniaturansichtinhalten sind vorab authentifiziert. Der Download eines Autorisierungsheaders ist nicht erforderlich. Diese URLs sind kurzlebig und nur für wenige Stunden gültig. Sie sollten nicht von Apps zwischengespeichert werden.


## <a name="size-values"></a>Größenwerte

In dieser Tabelle sind die möglichen Miniaturansichtgrößen definiert. Zwar können Sie jede beliebige Miniaturansichtgröße anfordern; bei den definierten Werten ist es jedoch wahrscheinlich, dass sie existieren und dass schnell ein Wert zurückgegeben wird:

| Name           | Auflösung  | Seitenverhältnis | Beschreibung                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 longest
  | Original     | Kleine, stark komprimierte Miniaturansicht, zugeschnitten auf ein quadratisches Seitenverhältnis |
| `medium`       | 176 longest | Original     | Zugeschnitten auf die standardmäßige Elementgröße für die OneDrive-Webansicht         |
| `large`        | 800 longest
 | Original     | Miniaturansicht, bei der die längste Kante auf 800 Pixel skaliert wurde               |

## <a name="remarks"></a>Bemerkungen

**Hinweis:** Für OneDrive for Business und SharePoint gilt:

* Die folgenden Aufrufe können nicht zur Erweiterung der Miniaturansichtsammlung verwendet werden: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->

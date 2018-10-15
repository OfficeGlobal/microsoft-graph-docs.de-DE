---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Abrufen von Miniaturansichten für eine Datei oder einen Ordner
ms.openlocfilehash: 98bfa0bee80beabc9934ae603f317627facffb4a
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266835"
---
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
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) von `$select` zur Anpassung der Antwort.

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode einen Antwortcode des Typs `200 OK` und eine Sammlung von [ThumbnailSet](../resources/thumbnailset.md)-Objekten im Antworttext zurück.

## <a name="example"></a>Beispiel

Hier ist ein Beispiel für die Anforderung, die verfügbare Miniaturansichten für ein Element im OneDrive des aktuellen Benutzers abruft.

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

Diese gibt ein Array von verfügbaren **thumbnailSets** für das Element zurück. Ein beliebiges Element auf einem Laufwerk kann Null oder mehr Miniaturansichten aufweisen.

**Hinweis:** Sie können den _select_-Abfragezeichenfolgenparameter verwenden, um zu steuern, welche Miniaturansichtgrößen im **ThumbnailSet** zurückgegeben werden.
ruft beispielsweise nur die mittelgroßen Miniaturansichten ab.`/thumbnails?select=medium`


### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

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

## <a name="get-a-single-thumbnail"></a>Abrufen einer einzelnen Miniaturansicht

Sie können die Metadaten einer einzelnen Miniaturansicht sowie ihre Größe abrufen, indem Sie sie in einer Anforderung direkt adressieren.

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a>Pfadparameter

| Name         | Typ   | Beschreibung                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| **item-id**  | Zeichenfolge | Der eindeutige Bezeichner für das referenzierte Element                                           |
| **thumb-id** | Nummer | Der Index der Miniaturansicht, in der Regel 0 bis 4. Wenn es eine benutzerdefinierte Miniaturansicht gibt, ist ihr Index 0. |
| **size**     | Zeichenfolge | Die Größe der angeforderten Miniaturansicht. Dabei kann es sich um eine der nachfolgend aufgeführten Standardgrößen oder um eine benutzerdefinierte Größe handeln. |

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

## <a name="retrieve-thumbnail-binary-content"></a>Abrufen von binären Miniaturansichtinhalten

Sie können den Inhalt einer Miniaturansicht direkt abrufen, indem Sie die Eigenschaft **content** der Miniaturansicht anfordern.

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a>Antwort

Der Dienst antwortet mit einer Umleitung auf die Miniaturansicht-URL.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

Miniaturansicht-URLs sind cachesicher. Die URL ändert sich, wenn sich das Element derart ändert, dass eine neue Miniaturansicht generiert werden muss.


## <a name="getting-thumbnails-while-listing-driveitems"></a>Abrufen von Miniaturansichten beim Auflisten von DriveItems

Wenn Sie eine Liste der anzuzeigenden DriveItem-Ressourcen abrufen, können Sie mit dem _$expand_-Abfragezeichenfolge-Parameter außerdem die Miniaturansichten für diese Ressourcen aufnehmen.
Dadurch kann Ihre App Miniaturansichten und Elemente in einer einzelnen Anforderung abrufen, statt viele Anforderungen auszuführen.

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a>Antwort

Die Dienstantworten mit der Liste der DriveItems und ihren Miniaturansichten.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "182331E8-2788-4932-B52A-A6550577043F",
      "name": "my photo.jpg",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    },
    {
      "id": "2D223953-A56B-4D9B-ADF3-13E7820673A2",
      "name": "presentation.pptx",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    }
  ]
}
```

## <a name="size-options"></a>Größenoptionen

In dieser Tabelle sind die möglichen Miniaturansichtgrößen definiert. Zwar können Sie jede beliebige Miniaturansichtgröße anfordern; bei den definierten Werten ist es jedoch wahrscheinlich, dass sie existieren und dass schnell ein Wert zurückgegeben wird:

| Name           | Auflösung  | Seitenverhältnis | Beschreibung                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 längste  | Original     | Kleine, stark komprimierte Miniaturansicht, zugeschnitten auf ein quadratisches Seitenverhältnis |
| `medium`       | 176 längste | Original     | Zugeschnitten auf die standardmäßige Elementgröße für die OneDrive-Webansicht         |
| `large`        | 800 längste | Original     | Miniaturansicht, bei der die längste Kante auf 800 Pixel skaliert wurde               |
| `smallSquare`  | 96x96       | Quadratisches Zuschneiden  | Kleines Quadrat (Miniaturansicht)                                               |
| `mediumSquare` | 176x176     | Quadratisches Zuschneiden  | Kleines Quadrat (Miniaturansicht)                                               |
| `largeSquare`  | 800x800     | Quadratisches Zuschneiden  | Großes Quadrat (Miniaturansicht)                                               |

## <a name="requesting-custom-thumbnail-sizes"></a>Anfordern von benutzerdefinierten Miniaturansichtgrößen

Zusätzlich zu den definierten Größen kann Ihre App eine benutzerdefinierte Miniaturansichtsgröße anfordern, indem die Dimensionen der Miniaturansicht mit dem Präfix `c` angegeben werden.
Wenn Ihre App zum Beispiel Miniaturansichten mit einer Größe von 300 x 400 benötigt, können Sie diese Größe wie folgt anfordern:

<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

Die Antwort ist die benutzerdefinierte Miniaturansichtsgröße:

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_Crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

Sie können die folgenden Optionen nach der Größe der angeforderten Miniaturansicht angeben:

### <a name="examples-of-custom-identifiers"></a>Beispiele für benutzerdefinierte Bezeichner

| Miniaturansicht-ID | Auflösung             | Seitenverhältnis | Beschreibung                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| c300x400             | Begrenzt durch 300 x 400-Feld | Original     | Generiert eine Miniaturansicht, die in ein Feld von 300 x 400 Pixel passt; dabei wird das Seitenverhältnis beibehalten                                                                 |
| c300x400_Crop        | 300x400                | Zugeschnitten      | Erstellt eine Miniaturansicht mit 300 x 400 Pixel. Dies funktioniert, indem Sie die Größe des Bilds so ändern, dass das Feld von 300 x 400 Pixel gefüllt wird, und alles zuschneiden, was über dieses Feld hinausgeht. |

**Hinweis:** Die zurückgegebenen Miniaturansicht stimmt möglicherweise nicht exakt mit den angeforderten Pixel-Abmessungen überein, , das Seitenverhältnis stimmt jedoch.
In einigen Fällen wird möglicherweise eine größere Miniaturansicht zurückgegeben als angefordert wurde, wenn die Miniaturansicht bereits vorhanden ist und einfach skaliert werden kann, damit sie der angeforderten Auflösung entspricht.

## <a name="remarks"></a>Hinweise

**Hinweis:** Für OneDrive for Business und SharePoint gilt:

Die folgenden Aufrufe können nicht zur Erweiterung der Miniaturansichtsammlung verwendet werden:

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

Miniaturansichten werden unter SharePoint Server 2016 nicht unterstützt.

### <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/driveitem_list_thumbnails.md:
      Unable to map some markdown elements into schema.
         Unmapped methods:
      enum-item-thumbnails, get-one-thumbnail, get-thumbnail-content, get-thumbnail-while-listing, get-thumbnail-custom-size
         Unmapped tables:
      Permissions - AuthScopes, Path parameters - PathParameters, Size options - Unknown, Examples of custom identifiers - Unknown",
    "Warning: Couldn't serialize request for path /me/drive/items/{var}/thumbnails/{var}/{var}/content into EDMX: System.InvalidOperationException: Uri path requires navigating into unknown object hierarchy: missing property '{var}' on 'thumbnailSet'. Possible issues:
         1) Doc bug where '{var}' isn't defined on the resource.         2) Doc bug where '{var}' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.       3) Doc bug where 'thumbnailSet' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation
     at ApiDocs.Publishing.CSDL.CsdlWriter.ParseRequestTargetType(String requestPath, MethodCollection requestMethodCollection, EntityFramework edmx, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 1145
     at ApiDocs.Publishing.CSDL.CsdlWriter.ProcessRestRequestPaths(EntityFramework edmx, String[] baseUrlsToRemove, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 821"
  ],
  "tocPath": "Items/Thumbnails"
} -->

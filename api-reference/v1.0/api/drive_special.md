# <a name="get-a-special-folder-by-name"></a>Speziellen Ordner nach Name abrufen

Verwenden Sie spezielle Auflistung, um auf einen speziellen Ordner basierend auf dem Namen zuzugreifen.

Spezielle Ordner bieten einfache Aliase für den Zugriff auf bekannte Ordner in OneDrive, ohne dass der Ordner anhand des Pfads nachgeschlagen werden muss (wofür eine Lokalisierung erforderlich wäre) oder anhand einer ID auf den Ordner verwiesen werden muss. Wenn ein spezieller Ordner umbenannt oder an eine andere Position innerhalb des Laufwerks verschoben wird, kann mit dieser Syntax weiterhin nach diesem Ordner gesucht werden.

Spezielle Ordner werden automatisch erstellt, wenn eine Anwendung das erste Mal versucht, einen Ordner zu schreiben, wenn noch keiner vorhanden ist. Wenn ein Benutzer einen speziellen Ordner löscht, wird dieser neu erstellt, wenn erneut in den Ordner geschrieben wird.

**Hinweis:**  Wenn Sie nur über Leseberechtigungen verfügen und einen speziellen Ordner anfordern, der nicht vorhanden ist, wird ein `403 Forbidden`-Fehler angezeigt.

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:

  * Files.Read
  * Files.ReadWrite

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader

| Name          | Typ   | Beschreibung               |
|:--------------|:-------|:--------------------------|
| Authorization | string | Bearer <token>. Required. |


## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [driveItem](../resources/driveitem.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung
Hier ist ein Beispiel für die Anforderung der Laufwerke des Benutzers.

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a>Bemerkungen

Um die untergeordneten Elemente eines speziellen Ordners anzufordern, können Sie die `children`-Sammlung anfordern oder die Option [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) verwenden, um die Sammlung untergeordneter Elemente zu erweitern.


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->

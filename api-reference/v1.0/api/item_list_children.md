# <a name="list-children-of-a-driveitem"></a>Untergeordnete Elemente eines DriveItem auflisten

Eine Auflistung von [DriveItems](../resources/driveitem.md) im **untergeordneten** Verhältnis eines DriveItem zurückgeben.

DriveItems mit einem nicht-NULL-Werte-**Ordner oder einer Paket**-Facette können ein oder mehrere untergeordnete DriveItems haben.


## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:

  * Files.Read
  * Files.ReadWrite

## <a name="http-request"></a>HTTP-Anforderung
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader

| Name          | Typ   | Beschreibung                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung
Es folgt eine Beispiel für eine Anforderung, die DriveItems in den Stammordner des aktuellen Benutzers in OneDrive zurückgibt.zugeben.

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

**Hinweis:** Wenn eine Auflistung die Standardseitengröße (200 Artikel) überschreitet, wird die Eigenschaft **@odata.nextLink** in der Antwort zurückgegeben, damit angezeigt wird, dass mehr Elemente zur Verfügung, und die Anfrage-URL für die nächste Seite von Elementen zurückzugeben.

Sie können die Seitengröße über [Optionale Abfragezeichenfolge-Parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) steuern.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->

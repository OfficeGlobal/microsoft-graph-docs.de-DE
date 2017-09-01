# <a name="search-for-a-driveitem-within-a-drive"></a>DriveItem in einem Laufwerk suchen

Durchsuchen Sie die Hierarchie der Elemente nach Elementen, die mit einer Abfrage übereinstimmen. Sie können eine Ordnerhierarchie, ein gesamtes Laufwerk oder die für den aktuellen Benutzer freigegebenen Dateien durchsuchen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```
GET /me/drive/root/search(q='{search-text}')
GET /me/drive/items/{item-id}/search(q='{search-text}')
GET /me/drive/root:/{item-path}:/search(q='{search-text}')
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) von `$expand`, `$select`, `$skipToken`, `$top` und `$orderby` zur Anpassung der Antwort.

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

#### <a name="function-parameters"></a>Funktionsparameter

| Name | Wert  | Beschreibung                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| `q`  | string | Der zum Durchsuchen der Elemente verwendete Abfragetext. Werte werden möglicherweise mit mehreren Feldern wie Dateiname, Metadaten und Dateiinhalt abgeglichen. |

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Es folgt ein Beispiel für die Anforderung zum Durchsuchen von OneDrive des aktuellen Benutzers
<!-- {
  "blockType": "request",
  "name": "item_search"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/search(q='{search-query}')
```

##### <a name="response"></a>Antwort
Diese Methode gibt ein Objekt mit einer Sammlung von [DriveItems](../resources/driveitem.md)-Elementen zurück, die den Suchkriterien entsprechen. Wenn keine Elemente gefunden werden, wird eine leere Sammlung zurückgegeben.

Wenn diese Methode zu viele Ergebnisse zurückgibt, ist die Antwort seitennummeriert und enthält eine **@odata.nextLink**-Eigenschaft mit einer URL zur nächsten Ergebnisseite. Sie können den `$top`-Abfrageparameter zum Angeben der Anzahl der Elemente auf einer Seite verwenden.

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
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a>Suchen nach Elementen, auf die Benutzer zugreifen können

Neben Elementen in einem Laufwerk kann Ihre App die Suche auf Elemente erweitern, die für den aktuellen Benutzer freigegeben wurden. Verwenden Sie zum Erweitern des Suchbereichs die **search**-Methode für die [Laufwerk](../resources/drive.md)ressource.

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "item_search_all"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/search(q='{search-query}')
```

##### <a name="response"></a>Antwort
Die Antworten können beim Durchsuchen der **Laufwerk**ressource Elemente enthalten, die sich außerhalb des Laufwerks befinden (Elemente, die für den aktuellen Benutzer freigegeben sind). Diese Elemente enthalten das [**remoteItem**](../resources/remoteitem.md)-Facet, das angibt, dass sie außerhalb des Ziellaufwerks gespeichert sind. 

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
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: search",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Items/Search items"
}-->

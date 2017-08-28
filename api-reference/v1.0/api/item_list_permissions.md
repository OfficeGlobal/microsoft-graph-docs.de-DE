# <a name="list-permissions-on-a-driveitem"></a>Auflisten von Berechtigungen für DriveItem

Listen Sie geltende Berechtigungen für ein [DriveItem](../resources/driveitem.md)-Objekt auf.

Die **permissions**-Beziehungen eines DriveItem-Elements können nicht im Rahmen eines Aufrufs von [get DriveItem](item_get.md) oder einer Sammlung von DriveItems erweitert werden. Sie müssen direkt auf die permissions-Eigenschaft zugreifen.

## <a name="access-to-permissions"></a>Zugriff auf Berechtigungen

Die Berechtigungssammlung umfasst potenziell vertrauliche Informationen und ist möglicherweise nicht für alle Aufrufer verfügbar.

* Für den Besitzer des Elements werden alle Berechtigungen zurückgegeben. Dies umfasst Mitbesitzer.
* Für Aufrufer, die keine Besitzer sind, werden nur die Berechtigungen zurückgegeben, die für den Aufrufer gelten.
* Berechtigungseigenschaften, die Geheimnisse enthalten (z. B. `shareId` und `webUrl`), werden nur für Aufrufer zurückgegeben, die Berechtigungen erstellen können.

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
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Typ   | Beschreibung                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | string | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen eTag in dem Element übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben. |

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von [Permission](../resources/permission.md)-Ressourcen im Antworttext zurück.

Geltende Berechtigungen eines Elements können aus zwei Quellen stammen:

* Berechtigungen, die direkt für das Element selbst gelten
* Berechtigungen, die von Vorgängerelementen geerbt werden

Aufrufer können prüfen, ob die Berechtigung geerbt wurde, indem sie die **inheritedFrom**-Eigenschaft prüfen. Diese Eigenschaft ist eine [**itemReference**](../resources/itemreference.md)-Ressource, die auf das Vorgängerelement verweist, von dem die Berechtigung vererbt wurde.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

Weitere Informationen zum Abrufen einer einzelnen Berechtigungsressource finden Sie unter [Abrufen von Berechtigungen](permission_get.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->

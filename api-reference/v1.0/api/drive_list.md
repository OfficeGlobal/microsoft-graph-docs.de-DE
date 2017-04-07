# <a name="list-available-drives"></a>Verfügbare Laufwerke auflisten

Dient zum Abrufen der Liste der [Laufwerk](../resources/drive.md)-Ressourcen für einen Ziel-[Benutzer](../resources/user.md) oder eine Ziel-[Gruppe](../resources/group.md). Ihre App kann auch den Satz von Dokumentbibliotheken auf der SharePoint-Stammwebsite anfordern.
## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:

  * Files.Read
  * Files.ReadWrite
  * Sites.Read.All

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /drives
GET /me/drives
GET /groups/{id}/drives
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Drive](../resources/drive.md)-Objekten im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung
Hier ist ein Beispiel für die Anforderung der Laufwerke des Benutzers.

<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drives
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.drive",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 579

{
  "value": [
    {
      "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
      "driveType": "business",    
      "owner": {
          "user": {
              "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
              "displayName": "Ryan Gregg"
          }
      },
      "quota": {
          "deleted": 256938,
          "remaining": 1099447353539,
          "state": "normal",
          "total": 1099511627776
      }
    }
  ]
}
```

## <a name="remarks"></a>Bemerkungen

Die meisten Benutzer verfügen nur über eine einzige Laufwerkressource. Gruppen und einige Benutzer verfügen möglicherweise über mehrere Laufwerke.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/List Drives"
}-->

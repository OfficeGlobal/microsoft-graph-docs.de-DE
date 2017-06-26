# <a name="list-recent-files"></a>Zuletzt verwendete Dateien auflisten

Dient zum Auflisten eines Satzes von Elementen, die zuletzt von dem angemeldeten Benutzer verwendet wurden. Diese Sammlung enthält Elemente, die sich in dem Laufwerk des Benutzers befinden sowie Elemente in anderen Laufwerken, auf die dieser Zugriff hat.

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:

* Files.Read
* Files.ReadWrite
* Files.Read.All
* Files.ReadWrite.All
* Sites.Read.All
* Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/recent
```

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="example"></a>Beispiel

<!-- { "blockType": "request", "name": "drive-recent", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/recent
```

## <a name="response"></a>Antwort

Dadurch wird eine Sammlung von [DriveItem](../resources/driveitem.md)-Ressourcen für Elemente zurückgegeben, auf die der Besitzer des Laufwerks vor kurzem zugegriffen hat. Elemente außerhalb des Laufwerks des Benutzers enthalten das [RemoteItem](../resources/remoteitem.md)-Facet, das Informationen zum Zugriff auf das freigegebene Element bereitstellt.


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      }
    }
  ]
}
```

## <a name="remarks"></a>Bemerkungen

Einige driveItems, die von der **recent**-Aktion zurückgegeben werden, enthalten immer das **remoteItem**-Facet, das angibt, dass es sich um Elemente von einem anderen Laufwerk handelt. Um auf das ursprüngliche DriveItem-Objekt zuzugreifen, müssen Sie eine Anforderung anhand der Angaben in **remoteItem** im folgenden Format stellen:

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->

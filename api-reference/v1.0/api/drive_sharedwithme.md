# <a name="list-items-shared-with-the-signed-in-user"></a>Elemente auflisten, die für den angemeldeten Benutzer freigegeben sind

Mit dieser API können Sie eine Sammlung von Ressourcen des Typs [DriveItem](../resources/driveitem.md) abrufen, die für den Besitzer der Ressource des Typs [Drive](../resources/drive.md) freigegeben wurden.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

Zusätzlich gilt: Ohne eine der Berechtigungen des Typs **All** ist kein Zugriff auf die von dieser API zurückgegebenen freigegebenen Elemente möglich.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/sharedWithMe
```

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="example"></a>Beispiel

<!-- { "blockType": "request", "name": "drive-sharedwithme", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/sharedWithMe
```

## <a name="response"></a>Antwort

Dadurch wird eine Sammlung von [DriveItem](../resources/driveitem.md)-Ressourcen, zurückgegeben, die die DriveItem-Ressourcen enthalten, die für den Besitzer des Laufwerks freigegeben wurden. Da es sich bei dem Laufwerk um das Standardlaufwerk des Benutzers handelt, werden in diesem Beispiel Elemente zurückgegeben, die für den angemeldeten Benutzer freigegeben sind.


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
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
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>Bemerkungen

DriveItems, die von der **SharedWithMe**-Aktion zurückgegeben werden, enthalten immer das [**remoteItem**](../resources/remoteitem.md)-Facet, das angibt, dass es sich um Elemente von einem anderen Laufwerk handelt. Um auf die freigegebenen DriveItem Ressourcen zuzugreifen, müssen Sie eine Anforderung anhand der Angaben in **remoteItem** im folgenden Format stellen:

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.parentReference.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->

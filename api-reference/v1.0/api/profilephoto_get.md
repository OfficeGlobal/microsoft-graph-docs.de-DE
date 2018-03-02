# <a name="get-photo"></a>Foto abrufen

Rufen Sie das angegebene [profilePhoto](../resources/profilephoto.md) oder die Metadaten (profilePhoto-Eigenschaften) ab.

Ein GET-Vorgang sucht nach dem angegebenen Foto im Postfach des Benutzers in Exchange Online.

> **Hinweis:** Dieser Vorgang in Version 1.0 unterstützt ausschließlich Postfächer in Geschäfts-, Schul- oder Unikonten des Benutzers. Persönliche Postfächer werden nicht unterstützt.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

*   Profilfotos aller Benutzer im Mandanten, einschließlich des angemeldeten Benutzers: User.ReadBasic.All, User.Read.All, User.ReadWrite.All
*   Profilfoto des angemeldeten Benutzers: User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All
* Profilfoto einer **Gruppe**: Group.Read.All, Group.ReadWrite.All
* Foto eines **Kontakts**: Contacts.Read, Contacts.ReadWrite

## <a name="http-request-to-get-the-photo"></a>HTTP-Anforderung zum Abrufen des Fotos
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="http-request-to-get-the-metadata-of-the-photo"></a>HTTP-Anforderung zum Abrufen von Metadaten des Fotos
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response-for-getting-the-photo"></a>Antwort für Abrufen des Fotos
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und binäre Daten des angeforderten Fotos zurückgegeben.  Wenn kein Foto vorhanden ist, gibt der Vorgang `404 Not Found` zurück.
## <a name="response-for-getting-the-metadata-of-the-photo"></a>Antwort für Abrufen der Metadaten des Fotos
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [profilePhoto](../resources/profilePhoto.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request-1"></a>Anforderung 1
Diese Anforderung ruft das Foto des angemeldeten Benutzers mit der größten verfügbaren Größe ab.
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a>Antwort 1
Enthält die binären Daten des angeforderten Fotos. Der HTTP-Antwortcode ist 200.

##### <a name="request-2"></a>Anforderung 2
Diese Anforderung ruft die Metadaten des Benutzerfotos des angemeldeten Benutzers.
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-2"></a>Antwort 2

Die folgenden Antwortdaten zeigen die Metadaten des Fotos. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

Die folgenden Antwortdaten zeigen die Inhalte einer Antwort, wenn für den Benutzer noch kein Foto hochgeladen wurde. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a>Verwenden der Binärdaten des angeforderten Fotos

Wenn Sie den `/photo/$value`-Endpunkt zum Abrufen der Binärdaten für ein Profilfoto verwenden, müssen Sie die Daten in eine Base-64-Zeichenfolge konvertieren, damit sie als E-Mail-Anlage hinzugefügt werden können. Das folgende Beispiel in JavaScript zeigt das Erstellen eines Arrays, das Sie als Wert des `Attachments`-Parameters einer [Outlook-Nachricht](user_post_messages.md) übergeben können.

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

Unter [Microsoft Graph Connect-Beispiel für Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) finden Sie eine Implementierung dieses Beispiels.

Wenn Sie das Bild auf einer Webseite anzeigen möchten, erstellen Sie ein Objekt im Arbeitsspeicher aus dem Bild, und verwenden Sie das Objekt als Quelle eines Bildelements. Hier ist ein Beispiel in JavaScript für diesen Vorgang.

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

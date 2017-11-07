# <a name="list-contacts"></a>Kontakte auflisten

Mit dieser API können Sie eine Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers abrufen.


### <a name="get-contacts-in-another-users-contact-folder"></a>Abrufen von Kontakten aus dem Kontaktordner eines anderen Benutzers

Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Kontakte aus dem Kontaktordner eines anderen Benutzers anzeigen. Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.

Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John. Der Benutzer Garth hat einen Kontaktordner für John freigegeben. Sie können die Kontakte in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

Diese Funktion gilt für alle unterstützten GET-Kontaktvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten). Sie gilt auch, wenn Garth sein gesamtes Postfachs an John delegiert hat.

Wenn Garth weder seinen Kontaktordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben. In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um Kontakte aus dem Kontaktordner eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
```

Diese Funktion ist nur in GET-Vorgängen verfügbar für:

- Freigegebene Kontaktordner, Kalender und Nachrichtenordner 
- Kontakte, Ereignisse und Nachrichten in freigegebenen Ordnern
- Die oben aufgeführten Ressourcen in delegierten Postfächern

Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse, Nachrichten und deren Ordner nicht zur Verfügung.


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Contacts.Read, Contacts.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Contacts.Read, Contacts.ReadWrite    |
|Anwendung | Contacts.Read, Contacts.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung

So rufen Sie alle Kontakte in einem Benutzerpostfach ab:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

So rufen Sie Kontakte in einem spezifischen Ordner in einem Benutzerpostfach ab:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.

Zum Beispiel können Sie die `$filter` Abfrageparameter verwenden, um Kontakte auf Basis der Domäne mit ihren E-Mail-Adressen filtern:

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type   | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contact](../resources/contact.md)-Objekten im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

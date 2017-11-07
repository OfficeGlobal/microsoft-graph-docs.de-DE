# <a name="get-contact"></a>Kontakt abrufen

Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kontaktobjekts abrufen.


### <a name="get-contacts-in-another-users-contact-folder"></a>Abrufen von Kontakten aus dem Kontaktordner eines anderen Benutzers

Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Kontakte aus dem Kontaktordner eines anderen Benutzers anzeigen. Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.

Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John. Der Benutzer Garth hat einen Kontaktordner für John freigegeben. Sie können einen Kontakt in diesem freigegebenen Ordner aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts/{id}
```

Diese Funktion gilt für alle unterstützten GET-Kontaktvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten). Sie gilt auch, wenn Garth sein gesamtes Postfachs an John delegiert hat.

Wenn Garth weder seinen Kontaktordner für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben. In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um einen Kontakt aus dem Kontaktordner eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}
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
<!-- { "blockType": "ignored" } -->
Ein [Kontakt](../resources/contact.md) aus dem standardmäßigen [contactFolder](../resources/contactfolder.md) eines Benutzers.
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
|Name|Wert|Beschreibung|
|:---------------|:--------|:-------|
|$expand|string|Durch Trennzeichen getrennte Liste der Beziehungen, die in der Antwort erweitert und aufgenommen werden. Unterstützte Namen finden Sie in der Beziehungstabelle des [contact](../resources/contact.md)-Objekts. |
|$select|string|Durch Trennzeichen getrennte Liste der Eigenschaften, die in der Antwort aufgenommen werden.|

## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "http://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {},
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

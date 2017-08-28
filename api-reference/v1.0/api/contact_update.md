# <a name="update-contact"></a>Kontakt aktualisieren

Mit dieser API können Sie die Eigenschaften eines Kontaktobjekts aktualisieren.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Contacts.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Contacts.ReadWrite    |
|Anwendung | Contacts.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
Ein [Kontakt](../resources/contact.md) aus dem standardmäßigen [contactFolder](../resources/contactfolder.md) eines Benutzers.
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json. Erforderlich.   |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assistantName|String|Der Name des Assistenten des Kontakts.|
|birthday|DateTimeOffset|Das Geburtsdatum des Kontakts.|
|businessAddress|[PhysicalAddress](../resources/physicaladdress.md)|Die Geschäftsadresse des Kontakts.|
|businessHomePage|String|Die geschäftliche Homepage des Kontakts.|
|businessPhones|String|Die geschäftlichen Telefonnummern des Kontakts.|
|categories|String|Die Kategorien, die mit dem Kontakt verknüpft sind.|
|children|String|Die Namen der Kinder des Kontakts.|
|companyName|String|Der Name des Unternehmens des Kontakts.|
|department|String|Die Abteilung des Kontakts.|
|displayName|String|Der Anzeigename des Kontakts.|
|emailAddresses|[EmailAddress](../resources/emailaddress.md) collection|Die E-Mail-Adressen des Kontakts.|
|fileAs|String|Der Name, unter dem der Kontakt abgelegt ist.|
|generation|String|Die Generation des Kontakts.|
|givenName|String|Der Vorname des Kontakts.|
|homeAddress|[PhysicalAddress](../resources/physicaladdress.md)|Die Privatadresse des Kontakts.|
|homePhones|String collection|Die privaten Telefonnummern des Kontakts.|
|imAddresses|String|Instant Messaging Chatadressen des Kontakts.|
|initials|String|Die Initialen des Kontakts.|
|jobTitle|String|Die Position des Kontakts.|
|manager|String|Der Name des Vorgesetzten des Kontakts.
|middleName|String|Der zweite Vorname des Kontakts.|
|mobilePhone|String|Die Mobiltelefonnummer des Kontakts.|
|nickName|String|Der Spitzname des Kontakts.|
|officeLocation|String|Der Bürostandort des Kontakts.|
|otherAddress|[PhysicalAddress](../resources/physicaladdress.md)|Weitere Adressen für den Kontakt.|
|parentFolderId|String|Die ID des übergeordneten Ordners des Kontakts.|
|personalNotes|String|Die Notizen des Benutzers zu dem Kontakt.|
|profession|String|Der Beruf des Kontakts.|
|spouseName|String|Der Name des Ehepartners des Kontakts|
|surname|String|Der Nachname des Kontakts.|
|title|String|Der Titel des Kontakts.|
|yomiCompanyName|String|Der phonetische japanische Firmenname des Kontakts. Diese Eigenschaft ist optional.|
|yomiGivenName|String|Der phonetische japanische Vorname des Kontakts. Diese Eigenschaft ist optional.|
|yomiSurname|String|Der phonetische japanische Nachname des Kontakts. Diese Eigenschaft ist optional.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contacts/{id}
Content-type: application/json
Content-length: 1977

{
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "birthday": "1974-07-22"
}
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
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
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
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

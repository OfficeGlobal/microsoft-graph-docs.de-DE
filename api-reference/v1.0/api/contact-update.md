---
title: Kontakt aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Kontaktobjekts aktualisieren.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 381aa191639e32677d4fccbf9e9f48c99f3d988f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927905"
---
# <a name="update-contact"></a>Kontakt aktualisieren

Mit dieser API können Sie die Eigenschaften eines Kontaktobjekts aktualisieren.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Contacts.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Contacts.ReadWrite    |
|Anwendung | Contacts.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->[Wenden Sie sich](../resources/contact.md) von einem Benutzer standardmäßig [ContactFolder](../resources/contactfolder.md).
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
| Header       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json. Erforderlich.   |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assistantName|Zeichenfolge|Der Name des Assistenten des Kontakts.|
|birthday|DateTimeOffset|Das Geburtsdatum des Kontakts.|
|businessAddress|[PhysicalAddress](../resources/physicaladdress.md)|Die Geschäftsadresse des Kontakts.|
|businessHomePage|Zeichenfolge|Die geschäftliche Homepage des Kontakts.|
|businessPhones|Zeichenfolge|Die geschäftlichen Telefonnummern des Kontakts.|
|categories|Zeichenfolge|Die Kategorien, die mit dem Kontakt verknüpft sind.|
|children|Zeichenfolge|Die Namen der Kinder des Kontakts.|
|companyName|Zeichenfolge|Der Name des Unternehmens des Kontakts.|
|department|Zeichenfolge|Die Abteilung des Kontakts.|
|displayName|Zeichenfolge|Der Anzeigename des Kontakts. Beachten Sie, dass es sich bei spätere Aktualisierungen mit anderen Eigenschaften verursachen einen automatisch generierten Wert den Wert DisplayName überschrieben, den Sie angegeben haben. Um einen bereits vorhandenen Wert zu erhalten, immer als schließen Sie DisplayName in einem Aktualisierungsvorgang ein.|
|emailAddresses|[EmailAddress](../resources/emailaddress.md) collection|Die E-Mail-Adressen des Kontakts.|
|fileAs|Zeichenfolge|Der Name, unter dem der Kontakt abgelegt ist.|
|generation|Zeichenfolge|Die Generation des Kontakts.|
|givenName|Zeichenfolge|Der Vorname des Kontakts.|
|homeAddress|[PhysicalAddress](../resources/physicaladdress.md)|Die Privatadresse des Kontakts.|
|homePhones|Zeichenfolgenauflistung|Die privaten Telefonnummern des Kontakts.|
|imAddresses|Zeichenfolge|Instant Messaging Chatadressen des Kontakts.|
|initials|Zeichenfolge|Die Initialen des Kontakts.|
|jobTitle|Zeichenfolge|Die Position des Kontakts.|
|manager|Zeichenfolge|Der Name des Vorgesetzten des Kontakts.
|middleName|Zeichenfolge|Der zweite Vorname des Kontakts.|
|mobilePhone|Zeichenfolge|Die Mobiltelefonnummer des Kontakts.|
|nickName|Zeichenfolge|Der Spitzname des Kontakts.|
|officeLocation|Zeichenfolge|Der Bürostandort des Kontakts.|
|otherAddress|[PhysicalAddress](../resources/physicaladdress.md)|Weitere Adressen für den Kontakt.|
|parentFolderId|Zeichenfolge|Die ID des übergeordneten Ordners des Kontakts.|
|personalNotes|Zeichenfolge|Die Notizen des Benutzers zu dem Kontakt.|
|profession|Zeichenfolge|Der Beruf des Kontakts.|
|spouseName|Zeichenfolge|Der Name des Ehepartners/Partners des Kontakts|
|surname|Zeichenfolge|Der Nachname des Kontakts.|
|title|Zeichenfolge|Der Titel des Kontakts.|
|yomiCompanyName|Zeichenfolge|Der phonetische japanische Firmenname des Kontakts. Diese Eigenschaft ist optional.|
|yomiGivenName|Zeichenfolge|Der phonetische japanische Vorname des Kontakts. Diese Eigenschaft ist optional.|
|yomiSurname|Zeichenfolge|Der phonetische japanische Nachname des Kontakts. Diese Eigenschaft ist optional.|

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
  "businessHomePage": "https://www.contoso.com",
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

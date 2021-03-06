---
title: Personenressourcentyp
description: Eine Ansammlung von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: c92709143ee7def0ede98dfdb81a419df43c4493
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940295"
---
# <a name="person-resource-type"></a>Personenressourcentyp

Eine Ansammlung von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[List people](../api/user-list-people.md) | **Person** |Dient zum Abrufen einer Sammlung von person-Objekten, sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md).|

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|birthday|Zeichenfolge|Der Geburtstag der Person.|
|companyName|Zeichenfolge|Der Name des Unternehmens der Person.|
|department|Zeichenfolge|Die Abteilung der Person.|
|displayName|Zeichenfolge|Der Anzeigename der Person.|
|scoredEmailAddresses|[scoredEmailAddress](scoredemailaddress.md)-Sammlung|Die E-Mail-Adressen der Person.|
|givenName|Zeichenfolge|Der Vorname der Person.|
|id|Zeichenfolge|Eindeutiger Bezeichner für die Person. Schreibgeschützt.|
|imAddress|Zeichenfolge|Die VOIP-SIP-Adresse (Voice oder IP; Session Initiation Protocol) der Chatnachricht für den Benutzer. Schreibgeschützt.|
|isFavorite|Boolesch|`true`, wenn der Benutzer diese Person als Favorit gekennzeichnet hat.|
|jobTitle|Zeichenfolge|Die Position der Person.|
|officeLocation|Zeichenfolge|Der Bürostandort der Person.|
|personNotes|String|Frei formatierbare Notizen, die der Benutzer zu dieser Person hinzugefügt hat.|
|personType|[personType](persontype.md) |Der Personentyp.|
|phones|[phone](phone.md)-Sammlung|Die Telefonnummern der Person.|
|postalAddresses|[location](location.md)-Sammlung|Die Adressen der Person.|
|profession|Zeichenfolge|Der Beruf der Person.|
|surname|Zeichenfolge|Der Nachname der Person.|
|userPrincipalName|Zeichenfolge|Der Benutzerprinzipalname der Person. Der UPN ist ein Anmeldename der Person im Internetformat, der auf dem Internetstandard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) basiert. Gemäß der Konvention sollte er dem E-Mail-Namen der Person zugeordnet sein. Das allgemeine Format lautet alias@domäne.|
|websites|[website](website.md)-Sammlung|Die Websites der Person.|
|yomiCompany|Zeichenfolge|Der phonetische japanische Firmenname des Unternehmens der Person.|

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

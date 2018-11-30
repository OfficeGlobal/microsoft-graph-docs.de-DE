---
title: Personenressourcentyp
description: Die Aggregation von Informationen über die von einer Person über e-Mail, Kontakte und sozialen Netzwerken. Personen können lokalen Kontakten, Kontakte aus für soziale Netzwerke, Ihrer Organisation Verzeichnis und Personen von letzte Kommunikation (wie e-Mail und Skype) sein.
ms.openlocfilehash: d9533c3550ec870c887b1e447fd0daf114bcfc83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058258"
---
# <a name="person-resource-type"></a>Personenressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Aggregation von Informationen über die von einer Person über e-Mail, Kontakte und sozialen Netzwerken. Personen können lokalen Kontakten, Kontakte aus für soziale Netzwerke, Ihrer Organisation Verzeichnis und Personen von letzte Kommunikation (wie e-Mail und Skype) sein.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[List people](../api/user-list-people.md) | **Person** |Dient zum Abrufen einer Sammlung von person-Objekten, sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md).|

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|birthday|string|Der Geburtstag der Person.|
|companyName|string|Der Name des Unternehmens der Person.|
|department|string|Die Abteilung der Person.|
|displayName|string|Der Anzeigename der Person.|
|emailAddresses|[RankedEmailAddress](rankedemailaddress.md) -Auflistung|Die E-Mail-Adressen der Person.|
|givenName|string|Der Vorname der Person.|
|id|string|Eindeutiger Bezeichner für die Person. Schreibgeschützt.|
|isFavorite|Boolean|`true`, wenn der Benutzer diese Person als Favorit gekennzeichnet hat.|
|mailboxType|string|Der Typ des Postfachs an, die durch die e-Mail-Adresse der Person dargestellt wird.|
|officeLocation|string|Der Bürostandort der Person.|
|personNotes|string|Frei formatierbare Notizen, die der Benutzer zu dieser Person hinzugefügt hat.|
|personType|string|Der Typ der Person, beispielsweise Verteilerliste.|
|phones|[phone](phone.md)-Sammlung|Die Telefonnummern der Person.|
|postalAddresses|[location](location.md)-Sammlung|Die Adressen der Person.|
|profession|string|Der Beruf der Person.|
|sources|[PersonDataSource](persondatasource.md) -Auflistung|Die Quellen die Benutzerdaten stammen aus, beispielsweise Verzeichnis oder Outlook-Kontakte.|
|surname|string|Der Nachname der Person.|
|title|string|Titel der Person.|
|userPrincipalName|string|Der Benutzerprinzipalname der Person. Der UPN ist ein Anmeldename der Person im Internetformat, der auf dem Internetstandard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) basiert. Gemäß der Konvention sollte er dem E-Mail-Namen der Person zugeordnet sein. Das allgemeine Format lautet alias@domäne.|
|websites|[website](website.md)-Sammlung|Die Websites der Person.|
|yomiCompany|string|Der phonetische japanische Firmenname des Unternehmens der Person.|

## <a name="relationships"></a>Beziehungen

Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
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

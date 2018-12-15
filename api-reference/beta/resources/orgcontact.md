---
title: Ressourcentyp orgContact
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 90d25d3ef7688372e4e961220bc454a2b5607344
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283668"
---
# <a name="orgcontact-resource-type"></a>Ressourcentyp orgContact

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von orgContact](../api/orgcontact-get.md) | [orgContact](orgcontact.md) |Lesen Sie Eigenschaften und Beziehungen des OrgContact-Objekts.|
|[Get-manager](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| Rufen Sie den Manager des Kontakts.|
|[List directReports](../api/orgcontact-list-directreports.md) |[directoryObject](directoryobject.md) collection| Der Kontakt direkt unterstellte aufgelistet.|
|[memberOf auflisten](../api/orgcontact-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Get-Auflistung ein Mitglied-Objekts.|
|[Delete](../api/orgcontact-delete.md) | Keine |OrgContact-Objekt zu löschen. |
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|Zeichenfolgenauflistung| Überprüfen Sie die Mitgliedschaft in der Gruppe. |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|Zeichenfolgenauflistung| Zurückgeben Sie aller Gruppen, denen der angegebene Kontakt ein Mitglied ist. |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|Zeichenfolgenauflistung| Gibt eine Liste der DirectoryObjects, den, denen der Kontakt ein Mitglied ist. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| addresses                    | [physicalOfficeAddress](physicalofficeaddress.md)            | Postanschriften für diesen Kontakt Organisationseinheit. Jetzt kann ein Kontakt nur eine physische Adresse haben. |
| companyName                  | String                                                    | Name des Unternehmens, die diesen Kontakt Organisationseinheit angehören.                                                                                                                                                                                                                                                                                                                 |
| department                   | String                                                     | Der Name für die Abteilung, in der der Kontakt arbeitet.                                                                                                                                                                                                                                                                                                                                |
| displayName                  | String                                                     | Der Anzeigename für diesen Kontakt Organisationseinheit.                                                                                                                                                                                                                                                                                                                                   |
| givenName                    | String                                                     | Vorname für diesen Kontakt Organisationseinheit.                                                                                                                                                                                                                                                                                                                                     |
| id                           | String                                                     | Eindeutiger Bezeichner für diesen Kontakt Organisationseinheit.                                                                                                                                                                                                                                                                                                                             |
| imAddresses                  | Zeichenfolgenauflistung                          | Liste der Instant Messaging-Adressen für diesen Kontakt Organisationseinheit. Jetzt kann ein Kontakt nur eine SIP-Adresse haben.                                                                                                                                                                                                                        |
| jobTitle                     | String                                                     | Position für diesen Kontakt Organisationseinheit.                                                                                                                                                                                                                                                                                                                                      |
|mail|String| Die SMTP-Adresse für den Kontakt, z. B. "jeff@contoso.onmicrosoft.com". |
| mailNickname                 | String                                                     | E-Mail-Alias (e-Mail-Adresse vor dem ausstehenden Teil der @-Zeichen) für diesen Kontakt Organisationseinheit.                                                                                                                                                                                                                                                                                |
| onPremisesLastSyncDateTime   | DateTimeOffset                                             | Datum und Uhrzeit, wann diese Organisationseinheit Kontakt zuletzt, synchronisiert aus lokalen AD. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise könnte Uhr UTC auf 1 Jan 2014 wie folgt aussehen: "2014-01-01T00:00:00Z'.   |
| onPremisesProvisioningErrors |[OnPremisesProvisioningError](onpremisesprovisioningerror.md) -Auflistung       | Liste der Fehler für diesen Kontakt Organisationseinheit provisioning Synchronisierung.                                                                                                                                                                                                                                                                                                |
|onPremisesSyncEnabled|Boolescher Wert|**true,** Wenn dieses Objekt aus einem lokalen Verzeichnis synchronisiert ist. **false,** Wenn dieses Objekt wurde ist aus einem lokalen Verzeichnis synchronisiert, aber nicht mehr synchronisiert und jetzt gesteuert im Exchange; **null,** Wenn dieses Objekt aus einem lokalen Verzeichnis (Standard) nie synchronisiert wurden.|
| phones                       | [phone](phone.md)-Sammlung                            | Liste der Telefone für diesen Kontakt Organisationseinheit. Telefon-Typen können Mobile, Geschäfts- und geschäftlich Fax sein. Nur eine der einzelnen Typen kann jemals in der Auflistung vorhanden sein.                                                                                                                       |
| proxyAddresses               | Zeichenfolgenauflistung                                         | Beispiel: ["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]. Der **any** -Operator ist für Filterausdrücke auf mehrwertige Eigenschaften erforderlich. Unterstützt \$Filter.                                                                                                                                                                               |
| surname                      | String                                                     | Nachname für diesen Kontakt Organisationseinheit.                          |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|directReports|[directoryObject](directoryobject.md) collection| Mitarbeiter des Kontakts. (Die Benutzer und Kontakte, die die Manager-Eigenschaft, die auf diesen Kontakt festgelegt werden.)  Schreibgeschützt. Lässt Nullwerte zu.|
|manager|[directoryObject](directoryobject.md)| Der Benutzer oder Kontakt, der Vorgesetzte des Kontakts ist. Schreibgeschützt.|
|memberOf|[directoryObject](directoryobject.md)-Sammlung| Gruppen, denen diesen Kontakt ein Mitglied ist. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "@odata.type": "microsoft.graph.orgcontact"
}-->

```json
{
  "addresses": [{"@odata.type": "microsoft.graph.physicalOfficeAddress"}],
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "string (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "proxyAddresses": ["string"],
  "surname": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
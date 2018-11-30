---
title: Ressourcentyp orgContact
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: fb0970b2eb973e516761ba1145d66b3af7fdef5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063654"
---
# <a name="orgcontact-resource-type"></a>Ressourcentyp orgContact

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "officeLocation": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "proxyAddresses": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|city|String| Die Stadt, in die sich der Kontakt befindet. |
|Land|String| Das Land/Region, in dem sich der Kontakt befindet. |
|department|String| Der Name für die Abteilung, in der der Kontakt arbeitet. |
|onPremisesSyncEnabled|Boolean|**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).|
|displayName|String| Der Anzeigename für den Kontakt. |
|givenName|String| Dem angegebenen Namen (Vorname) des Kontakts. |
|jobTitle|String| Position des Kontakts. |
|onPremisesLastSyncDateTime|DateTimeOffset|Gibt das letzte Mal an dem das Objekt mit dem lokalen Verzeichnis synchronisiert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|onPremisesProvisioningErrors|[OnPremisesProvisioningError](onpremisesprovisioningerror.md) -Auflistung| Fehler beim Microsoft Synchronisierung während der Bereitstellung verwenden. |
|Mail|String| Die SMTP-Adresse für den Kontakt, z. B. "jeff@contoso.onmicrosoft.com". |
|mailNickname|String| Der e-Mail-Alias für den Kontakt. |
|mobilePhone|String| Die Anzahl der primären Mobiltelefon für den Kontakt. |
|id|String| Der eindeutige Bezeichner für den Kontakt. Schreibgeschützt.|
|officeLocation|String| Der Standort des Büros des Kontakts direkt Unternehmens. |
|postalCode|String| Die Postleitzahl für die Adresse des Kontakts. Die Postleitzahl ist spezifisch für Land/Region des Kontakts. In den USA enthält dieses Attribut die Postleitzahl. |
|proxyAddresses|Zeichenfolgenauflistung| Beispiel: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **any** -Operator ist für Filterausdrücke auf mehrwertige Eigenschaften erforderlich. Schreibgeschützt. Lässt keine Nullwerte zu. Unterstützt $filter. |
|state|String| Bundesland oder Kanton für die Adresse des Kontakts. |
|streetAddress|String| Die Straße des Kontakts Ort des Unternehmens. |
|surname|String| Den Nachnamen des Kontakts (Familie oder Nachnamen). |
|businessPhones|String| Die primäre Telefonnummer des Kontakts Sitz des Business. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|directReports|[directoryObject](directoryobject.md) collection| Mitarbeiter des Kontakts. (Die Benutzer und Kontakte, die die Manager-Eigenschaft, die auf diesen Kontakt festgelegt werden.)  Schreibgeschützt. Lässt Nullwerte zu.|
|manager|[directoryObject](directoryobject.md)| Der Benutzer oder Kontakt, der Vorgesetzte des Kontakts ist. Schreibgeschützt.|
|memberOf|[directoryObject](directoryobject.md)-Sammlung| Gruppen, denen diesen Kontakt ein Mitglied ist. Schreibgeschützt. Lässt Nullwerte zu.|

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
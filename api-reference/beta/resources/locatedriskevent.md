---
title: Ressourcentyp locatedRiskEvent
description: 'Ein Risikoereignis von Azure Active Directory-Identität Protection, die auf Standortdaten basiert erkannt. Befindet sich Risikotypen werden unterstützt:'
localization_priority: Normal
ms.openlocfilehash: 256c7a980fb9540e7e80337a5b8aad29fe73f26a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867557"
---
# <a name="locatedriskevent-resource-type"></a>Ressourcentyp locatedRiskEvent

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , das auf Standortdaten erkannt. Befindet sich Risikotypen werden unterstützt:
* [Anmeldungen von anonymen IP-Adressen](anonymousipriskevent.md)
* [Anmeldungen von Geräten Malware infiziert](malwareriskevent.md)
* [unmöglich Reisen zu untypischen Speicherorte](impossibletravelriskevent.md)
* [Anmeldungen von verdächtigen IP-Adressen](suspiciousipriskevent.md)
* [Anmeldungen von unbekannten Standorten](unfamiliarlocationriskevent.md) Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von locatedRiskEvent](../api/locatedriskevent-get.md) | [locatedRiskEvent](locatedriskevent.md) |Lesen Sie Eigenschaften und Beziehungen des LocatedRiskEvent-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Datum und Uhrzeit, die das Risikoereignis geschlossen wurde|
|createdDateTime|dateTimeOffset| Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde. Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst. Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.|
|id|string| Schreibgeschützt.|
|ipAddress|string| Die IP-Adresse von der Anmeldung|
|location|string| Die Position, die IP-Adresse von der Anmeldung zugeordnet ist|
|riskEventDateTime|dateTimeOffset| Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist|
|riskEventStatus|string| Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.|
|riskLevel|string| Mögliche Werte sind: `low`, `medium` und `high`.|
|riskEventType|string| Der Typ des Risikos|
|userDisplayName|string| Der Name des Benutzers gefährdet|
|userId|string| Die Id des Benutzers gefährdet|
|userPrincipalName|string| Der Benutzerprinzipalname des Benutzers gefährdet|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|impactedUser|[Benutzer](user.md)| Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locatedRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Ressourcentyp impossibleTravelRiskEvent
description: Ein Risikoereignis von Azure Active Directory-Identität Protection, in dem zwei Konto Anmeldungen von Speicherorten für den Benutzer untypischen auftreten, und es ist nicht möglich, zwischen den Standorten in die Dauer zwischen den Anmelde-ins umfassende Informationen zum Reisen, erkannt Risikoereignisse finden Sie in der Dokumentation zu Azure AD-Schutz.
ms.openlocfilehash: 38e61927121f520e79fd1fec8b8e6443fa8b76e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058451"
---
# <a name="impossibletravelriskevent-resource-type"></a>Ressourcentyp impossibleTravelRiskEvent

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , in dem zwei Konto Anmeldungen von Speicherorten für den Benutzer untypischen auftreten, und es ist nicht möglich, zwischen den Standorten in die Dauer zwischen den Anmelde-Ins vollständig Reisen, erkannt Informationen zu Risiken-Ereignissen finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |Lesen Sie Eigenschaften und Beziehungen des ImpossibleTravelRiskEvent-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Datum und Uhrzeit, die das Risikoereignis geschlossen wurde|
|createdDateTime|dateTimeOffset| Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde. Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst. Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.|
|deviceInformation|string| Informationen über das Gerät|
|id|string| Schreibgeschützt.|
|ipAddress|string| Die IP-Adresse des zweiten Anmeldung|
|isAtypicalLocation|Boolean| Wenn eine der Speicherorte untypischen für den Benutzer ist.|
|location|string| Die Position, die IP-Adresse des zweiten Anmeldung zugeordnet ist|
|previousIPAddress|string| Die IP-Adresse von der ersten Anmeldung|
|previousLocation|string| Die Position, die IP-Adresse von der ersten Anmeldung zugeordnet ist|
|previousSigninDateTime|dateTimeOffset| Datum und Uhrzeit der ersten Anmeldung|
|riskEventDateTime|dateTimeOffset| Datum und Uhrzeit des zweiten Anmeldung|
|riskEventStatus|string| Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.|
|riskLevel|string| Mögliche Werte sind: `low`, `medium` und `high`.|
|riskEventType|string| Der Typ des Risikos|
|userAgent|string| Benutzeragentzeichenfolge des Browsers|
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
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
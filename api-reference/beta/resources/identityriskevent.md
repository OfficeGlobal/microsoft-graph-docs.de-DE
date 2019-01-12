---
title: Ressourcentyp identityRiskEvent
description: 'Ein Risikoereignis von Azure Active Directory-Identität Protection erkannt. Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: be5e4afaa5bf85581c904ed94f07433243651ee9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953649"
---
# <a name="identityriskevent-resource-type"></a>Ressourcentyp identityRiskEvent

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)erkannt. Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:

| Ereignistyp         | Beschreibung|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | Anmeldungen von anonymen IP-Adressen. |
|[malwareRiskEvent](malwareriskevent.md) | Anmeldungen von Geräten Malware infiziert. |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | Unmöglich Reisen zu untypischen Speicherorte. |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | Benutzer mit verlorene Anmeldeinformationen. |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | Anmeldungen von verdächtigen IP-Adressen. |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | Anmeldungen von Speicherorten nicht vertraut sind. |

Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von identityRiskEvent](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |Lesen Sie Eigenschaften und Beziehungen des IdentityRiskEvent-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Datum und Uhrzeit, die das Risikoereignis geschlossen wurde|
|createdDateTime|dateTimeOffset| Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde. Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst. Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.|
|id|string| Schreibgeschützt.|
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
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
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
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

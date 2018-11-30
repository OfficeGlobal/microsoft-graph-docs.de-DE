---
title: Ressourcentyp riskyUsers
description: Stellt Azure AD-Benutzer, die gefährdet sind. Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.
ms.openlocfilehash: 5d51c303d25a781f8e432badb42acb48cf135217
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059966"
---
# <a name="riskyusers-resource-type"></a>Ressourcentyp riskyUsers

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt Azure AD-Benutzer, die gefährdet sind. Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.

Weitere Informationen zu Risiken-Ereignissen finden Sie unter [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).

## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[Liste riskyUsers](../api/riskyusers-list.md) | [riskyUsers](riskyuser.md) |Liste riskant Benutzer und deren Eigenschaften.|
|[Abrufen von riskyUsers](../api/riskyusers-get.md) | [riskyUsers](riskyuser.md)|Rufen Sie einen bestimmten Benutzer riskant und seine Eigenschaften.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|`id`|`string`|Eindeutige Id des Benutzers gefährdet|
|`isDeleted`|`bool`|Gibt an, ob der Benutzer gelöscht wurde. Mögliche Werte sind: `true`,`false`|
|`isGuest`|`bool`|Gibt an, ob der Benutzer ein Gastbenutzer ist. Mögliche Werte sind: `true` und `false`. True, wenn die Identität des Benutzers im Hinblick auf die außerhalb der Mandant in Erwägung. Dieser Benutzer kann sein, eine B2B oder B2C Benutzer mit der Identität in Azure AD, MSA oder 3. Partei Identitätsanbieter vertraut wird. False, wenn die Identität des Benutzers im Hinblick auf die in den Mandanten in Erwägung|
|`riskDetail`|`riskDetail`|Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde.|
|`riskLevel`|`riskLevel`|Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.|
|`riskState`|`riskState`|Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|`riskLastUpdatedDateTime`|`datetime`|Datum und Uhrzeit der letzten Aktualisierung der Benutzer riskant.|
|`userDisplayName`|`string`|Anzeigename des Benutzers riskant.|
|`userPrincipalName`|`string`|Benutzerprinzipalname riskant.|

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ |Beschreibung|
|:---------------|:--------|:----------|
|id|UserObjectId| Der eindeutige Bezeichner des Benutzers, mit denen ein bestimmtes Risiko-Ereignis zugeordnet ist.|
|isGuest|isGuest| Ein riskant Benutzer kann entweder ein Home-Benutzer (B2E) oder ein Gast (B2B, B2C) sein.|
|isDeleted|isDeleted| Ein Benutzer kann oder kann nicht gelöscht werden. |
|riskState|riskState| Ein Benutzer riskant konnte in einem mehrerer Zustände vorhanden sein. |
|riskDetail|riskDetail| Ein riskant Benutzer konnte aus mehreren Gründen in einem bestimmten Zustand sein. |
|riskLevel|riskLevel| Ein riskant Benutzer kann eine der mehrere Risikoebenen betrachtet werden. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"}
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

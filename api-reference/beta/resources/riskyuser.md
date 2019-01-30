---
title: Ressourcentyp riskyUsers
description: Stellt Azure AD-Benutzer, die gefährdet sind. Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 27c189a81d6ba4e088c1242acfd2cf0d0f5c56c5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643909"
---
# <a name="riskyusers-resource-type"></a>Ressourcentyp riskyUsers

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt Azure AD-Benutzer, die gefährdet sind. Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.

> **Hinweis:** Diese API ist eine Azure AD Premium P2-Lizenz erforderlich.

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
|`riskDetail`|`riskDetail`|Gibt den "Grund" für einen bestimmten Status eines riskanten Benutzers, einer Anmeldung oder eines Risikoereignisses an. Mögliche Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Der Wert `none` bedeutet, dass bisher keine Aktion für den Benutzer oder die Anmeldung ausgeführt wurde.|
|`riskLevel`|`riskLevel`|Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Mögliche Werte sind: `none`, `low`, `medium`, `high`, `hidden` und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung nicht für Azure AD Identity Protection aktiviert war.|
|`riskState`|`riskState`|Gibt den "Risikostatus" eines riskanten Benutzers, einer Anmeldung oder eines Risikoereignisses an. Mögliche Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
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
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/riskyuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

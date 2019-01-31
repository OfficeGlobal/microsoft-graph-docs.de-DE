---
title: signIn-Ressourcentyp
description: 'Diese Ressource enthält Informationen zu den Anmeldeaktivitäten von Benutzern oder Anwendungen in Ihrem Verzeichnis. '
localization_priority: Priority
ms.openlocfilehash: a2ccb84daee642d207919217aa2857745846c769
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640966"
---
# <a name="signin-resource-type"></a>signIn-Ressourcentyp
Diese Ressource enthält Informationen zu den Anmeldeaktivitäten von Benutzern oder Anwendungen in Ihrem Verzeichnis. 

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[List signIn](../api/signin-list.md) | [signIn](signin.md) |Lesen von Eigenschaften und Beziehungen von signIn-Objekten.|
|[Get signIn](../api/signin-get.md) | [signIn](signin.md) |Lesen von Eigenschaften und Beziehungen des signIn-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|appDisplayName|String|Bezieht sich auf den im Azure-Portal angezeigten Anwendungsnamen.|
|appId|String|Bezieht sich auf die eindeutige GUID, die die Anwendungs-ID in Azure Active Directory darstellt.|
|clientAppUsed|String|Gibt den Legacyclient an, der für die Anmeldeaktivtät verwendet wird. Beispiel: Browser, Exchange Active Sync, moderne Clients, IMAP, MAPI, SMTP, POP.|
|appliedConditionalAccessPolicy|[conditionalAccessPolicy](conditionalaccesspolicy.md)-Sammlung|Stellt eine Liste von Richtlinien für bedingte Zugriffe bereit, die durch die entsprechende Anmeldeaktivität ausgelöst werden.|
|conditionalAccessStatus|string| Stellt den Status der ausgelösten bedingten Zugriffsrichtlinie bereit. Mögliche Werte: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|originalRequestId|String|Die Anforderungs-ID der ersten Anforderung in der Authentifizierungssequenz.|
|isInteractive|Boolesch|Gibt an, ob eine Anmeldung interaktiv ist.|
|tokenIssuerName|String|Der Name des Identitätsanbieters (z. B. sts.microsoft.com).|
|tokenIssuerType|String|Stellt den Typ des identityProvider bereit. Mögliche Werte sind `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|correlationId|String|Bezieht sich auf die ID, die vom Client gesendet wird, wenn die Anmeldung initiiert wird. Diese Angabe wird für die Problembehandlung der entsprechenden Anmeldeaktivität bei Inanspruchnahme von Helpdesk oder Support verwendet.|
|createdDateTime|DateTimeOffset|Gibt das Datum und die Uhrzeit der Initiierung der Anmeldung an. Der Zeitstempeltyp liegt immer in UTC-Zeit vor. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|deviceDetail|[deviceDetail](devicedetail.md)|Gibt die Geräteinformationen an, von wo aus die Anmeldung erfolgt ist. Umfasst Informationen wie die Geräte-ID, das Betriebssystem und den Browser. |
|id|String|Gibt die eindeutige ID an, die die Anmeldeaktivität darstellt.|
|ipAddress|String|Gibt die IP-Adresse des Clients an, von dem aus die Anmeldung erfolgt ist.|
|location|[signInLocation](signinlocation.md)|Gibt den Ort, das Bundesland und den aus 2 Buchstaben bestehenden Ländercode für die Anmeldung an.|
|processingTimeInMilliseconds|Int|Gibt die Anforderungsverarbeitungszeit in Millisekunden in AD STS an.|
|riskDetail|`riskDetail`|Gibt den "Grund" für einen bestimmten Status eines riskanten Benutzers, einer Anmeldung oder eines Risikoereignisses an. Mögliche Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Der Wert `none` bedeutet, dass bisher keine Aktion für den Benutzer oder die Anmeldung ausgeführt wurde. **Hinweis:** Details für diese Eigenschaft sind nur für Kunden von Azure AD Premium P2 verfügbar. Für alle anderen Kunden wird `hidden` zurückgegeben.|
|riskLevelAggregated|`riskLevel`|Stellt die aggregierten Risikostufe bereit. Mögliche Werte sind: `none`, `low`, `medium`, `high`, `hidden` und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung nicht für Azure AD Identity Protection aktiviert war. **Hinweis:** Details für diese Eigenschaft sind nur für Kunden von Azure AD Premium P2 verfügbar. Für alle anderen Kunden wird `hidden` zurückgegeben.|
|riskLevelDuringSignIn|`riskLevel`|Gibt die Risikostufe während der Anmeldung an. Mögliche Werte sind: `none`, `low`, `medium`, `high`, `hidden` und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung nicht für Azure AD Identity Protection aktiviert war. **Hinweis:** Details für diese Eigenschaft sind nur für Kunden von Azure AD Premium P2 verfügbar. Für alle anderen Kunden wird `hidden` zurückgegeben.|
|riskEventTypes|`riskEventTypes`|Gibt die Liste der mit der Anmeldung verbundenen Risikoereignistypen an. Mögliche Werte sind: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic` und `unknownFutureValue`.|
|riskState|`riskState`|Gibt den "Risikostatus" eines riskanten Benutzers, einer Anmeldung oder eines Risikoereignisses an. Mögliche Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|mfaDetail|[mfaDetail](mfadetail.md)|Gibt die MFA-bezogenen Informationen wie "MFA erforderlich", "MFA-Status" für die entsprechende Anmeldung an.|
|networkLocationDetail|[networkLocationDetail](networklocationdetail.md)|Gibt Details zur Netzwerkadresse an.|
|riskLevel|string| Gibt die mit der Anmeldung verbundene Risikostufe an. Mögliche Werte sind: `low`, `medium`, `high`.|
|status|[signInStatus](signinstatus.md)|Gibt den Anmeldestatus an. Mögliche Werte sind `Success` und `Failure`.|
|userDisplayName|String|Gibt den Anzeigenamen des Benutzers an.|
|userId|String|Gibt die userId des Benutzers an.|
|userPrincipalName|String|Gibt den UPN des Benutzers an.|
|resourceDisplayName|String|Gibt den Namen der Ressource an, bei der sich der Benutzer angemeldet hat.|
|resourceId|String|Gibt die ID der Ressource an, bei der sich der Benutzer angemeldet hat.|
|authenticationMethodsUsed|String|Gibt die Liste der verwendeten Authentifizierungsmethoden an.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signIn"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "originalRequestId": "String",
  "isInteractive": "String",
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": "string",
  "resourceDisplayName": "string",
  "resourceId": "string",
  "authenticationMethodsUsed": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

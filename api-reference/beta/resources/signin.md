---
title: Anmeldung Ressourcentyp
description: 'Diese Ressource werden Benutzer oder eine Anwendung Anmeldung Aktivitäten in Ihrem Verzeichnis. '
ms.openlocfilehash: 2bc6c8b961f0626a6409d9be868235f285f48e52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065006"
---
# <a name="signin-resource-type"></a>Anmeldung Ressourcentyp
Diese Ressource werden Benutzer oder eine Anwendung Anmeldung Aktivitäten in Ihrem Verzeichnis. 

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Anmeldung](../api/signin-list.md) | [Anmeldung](signin.md) |Lesen Sie Eigenschaften und Beziehungen von Anmeldung-Objekten.|
|[Erste Anmeldung](../api/signin-get.md) | [Anmeldung](signin.md) |Lesen Sie Eigenschaften und Beziehungen Anmeldung-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|appDisplayName|String|Bezieht sich auf den Namen der Anwendung in der Azure-Verwaltungsportal angezeigt.|
|appId|Zeichenfolge|Bezieht sich auf die eindeutige GUID, die Id der Anwendung in Azure Active Directory darstellt.|
|authenticationProcessingDetails|`authenticationProcessingDetails`|Ausführliche Authentifizierung Prozessor zugeordnet.|
|clientAppUsed|String|Enthält den älteren Client für die Anmeldung activty.E.g verwendet. enthält Browser, Exchange Active Sync, moderne Clients, IMAP, MAPI, SMTP, POP.|
|appliedConditionalAccessPolicy|[ConditionalAccessPolicy](conditionalaccesspolicy.md) -Auflistung|Enthält eine Liste der bedingten Zugriffsrichtlinien, die von der entsprechenden Anmeldung Aktivität ausgelöst werden.|
|conditionalAccessStatus|string| Enthält den Status der bedingten Richtlinie ausgelöst. Mögliche Werte: sind `success`, `failure`, `notApplied` und `unknownFutureValue`.|
|originalRequestId|String|Die Anforderung-Id der ersten Anforderung in der Reihenfolge für die Authentifizierung.|
|isInteractive|Boolesch|Gibt an, ob eine Anmeldung interaktiv ist.|
|tokenIssuerName|String|Name der Identität Provider (z. B. sts.microsoft.com)|
|tokenIssuerType|String|Stellt den Typ des IdentityProvider bereit. Mögliche Werte sind `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|correlationId|String|Bezieht sich auf die ID, die vom Client gesendet wird, wenn der Anmeldung gestartet wird. Hiermit wird die entsprechende Aktivität-Anmeldung beim Aufrufen von Helpdesk oder Unterstützung bei der Problembehandlung.|
|createdDateTime|DateTimeOffset|Enthält das Datum und Uhrzeit der Anmeldung initiiert wurde. Der Zeitstempel-Typ ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|deviceDetail|[deviceDetail](devicedetail.md)|Enthält die Geräteinformationen aus, wo die Anmeldung aufgetreten. Es Inclules Informationen wie Geräte-ID, Betriebssystem, Browser. |
|id|String|Gibt die eindeutige ID für die Anmeldung Aktivität an.|
|ipAddress|Zeichenfolge|Enthält die IP-Adresse des Clients aus, wo die Anmeldung aufgetreten.|
|location|[signInLocation](signinlocation.md)|Enthält den Ort, Bundesland und 2 Buchstaben Ländercode aus, wo die Anmeldung aufgetreten.|
|processingTimeInMilliseconds|Int|Stellt die Zeit in Millisekunden in AD STS Verarbeitung die Anforderung|
|riskDetail|`riskDetail`|Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde.|
|riskLevelAggregated|`riskLevel`|Enthält die aggregierten Risikostufe. Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.|
|riskLevelDuringSignIn|`riskLevel`|Enthält die Risikostufe während der Anmeldung an. Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.|
|riskEventTypes|`riskEventTypes`|Enthält eine Liste der Risiko Ereignistypen der Anmeldung zugeordnet. Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecurePasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.|
|riskState|`riskState`|Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|mfaDetail|[mfaDetail](mfadetail.md)|Enthält die mehrstufiger Authentifizierung das weiterführende Informationen wie mehrstufiger Authentifizierung das erforderlich, mehrstufiger Authentifizierung das Status für die entsprechenden anmelden.|
|networkLocationDetail|[networkLocationDetail](networklocationdetail.md)|Enthält Informationen zu den Speicherort im Netzwerk.|
|riskLevel|string| Enthält die Risikostufe der Anmeldung zugeordnet. Mögliche Werte sind: `low`, `medium`, `high`.|
|status|[signInStatus](signinstatus.md)|Enthält die Anmeldestatus. Mögliche Werte sind `Success` und `Failure`.|
|userDisplayName|String|Gibt die Anzeige des Benutzers an.|
|userId|String|Gibt die Benutzer-ID des Benutzers an.|
|userPrincipalName|String|Gibt den UPN des Benutzers an.|
|resourceDisplayName|String|Gibt den Namen der Ressource, der der Benutzer bei angemeldet.|
|resourceId|Zeichenfolge|Gibt die Id der Ressource, der der Benutzer bei angemeldet.|
|authenticationMethodsUsed|String|Gibt die Liste der verwendeten Authentifizierungsmethoden|

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
  "riskLevel": "string",
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
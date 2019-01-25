---
title: Risiko Ressourcentyp
description: Aggregiert die Risikostufe, Risiko Zustand und Risiko Detailebene für die riskant Benutzer anmelden oder Risiko-Ereignis.
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 48fda9624e45072240bc694b8b5e152fe3ef0764
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524821"
---
# <a name="risk-resource-type"></a>Risiko Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aggregiert die Risikostufe, Risiko Zustand und Risiko Detailebene für die riskant Benutzer anmelden oder Risiko-Ereignis.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|`stateDetail`|riskDetail|Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde. |
|`riskLevelAggregated`|riskLevel|Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.|
|`riskLevelDuringSignIn`|riskLeve|Enthält die Risikostufe eine Anmeldung bei der Anmeldung (d. h. basierend auf die Risikoereignisse in Echtzeit). Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`. Der Wert `hidden` bedeutet, dass der Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.|
|`state`|riskState|Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit. Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
    "stateDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
    "riskLevelAggregated":  {"@odata.type": "microsoft.graph.riskLevel"},
    "riskLevelDuringSignIn":  {"@odata.type": "microsoft.graph.riskLevel"},
    "state":  {"@odata.type": "microsoft.graph.riskState"}
  }
  ```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/risk.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

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
# <a name="risk-resource-type"></a><span data-ttu-id="b9921-103">Risiko Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b9921-103">risk resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9921-104">Aggregiert die Risikostufe, Risiko Zustand und Risiko Detailebene für die riskant Benutzer anmelden oder Risiko-Ereignis.</span><span class="sxs-lookup"><span data-stu-id="b9921-104">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="b9921-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b9921-105">Properties</span></span>

| <span data-ttu-id="b9921-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9921-106">Property</span></span>   | <span data-ttu-id="b9921-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b9921-107">Type</span></span>|<span data-ttu-id="b9921-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9921-108">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="b9921-109">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b9921-109">riskDetail</span></span>|<span data-ttu-id="b9921-110">Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="b9921-110">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b9921-111">Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b9921-111">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="b9921-112">Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="b9921-112">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="b9921-113">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b9921-113">riskLevel</span></span>|<span data-ttu-id="b9921-114">Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="b9921-114">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b9921-115">Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b9921-115">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="b9921-116">Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="b9921-116">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="b9921-117">riskLeve</span><span class="sxs-lookup"><span data-stu-id="b9921-117">riskLeve</span></span>|<span data-ttu-id="b9921-118">Enthält die Risikostufe eine Anmeldung bei der Anmeldung (d. h. basierend auf die Risikoereignisse in Echtzeit).</span><span class="sxs-lookup"><span data-stu-id="b9921-118">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="b9921-119">Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b9921-119">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="b9921-120">Der Wert `hidden` bedeutet, dass der Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="b9921-120">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="b9921-121">riskState</span><span class="sxs-lookup"><span data-stu-id="b9921-121">riskState</span></span>|<span data-ttu-id="b9921-122">Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="b9921-122">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b9921-123">Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b9921-123">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9921-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b9921-124">JSON representation</span></span>

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

---
title: Risiko Ressourcentyp
description: Aggregiert die Risikostufe, Risiko Zustand und Risiko Detailebene für die riskant Benutzer anmelden oder Risiko-Ereignis.
localization_priority: Normal
ms.openlocfilehash: da198ba27ca6cd0b762f322863f8c9bfd56a5cb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810668"
---
# <a name="risk-resource-type"></a><span data-ttu-id="50dac-103">Risiko Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="50dac-103">risk resource type</span></span>

> <span data-ttu-id="50dac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="50dac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50dac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50dac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50dac-106">Aggregiert die Risikostufe, Risiko Zustand und Risiko Detailebene für die riskant Benutzer anmelden oder Risiko-Ereignis.</span><span class="sxs-lookup"><span data-stu-id="50dac-106">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="50dac-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50dac-107">Properties</span></span>

| <span data-ttu-id="50dac-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50dac-108">Property</span></span>   | <span data-ttu-id="50dac-109">Typ</span><span class="sxs-lookup"><span data-stu-id="50dac-109">Type</span></span>|<span data-ttu-id="50dac-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50dac-110">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="50dac-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="50dac-111">riskDetail</span></span>|<span data-ttu-id="50dac-112">Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="50dac-112">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="50dac-113">Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="50dac-113">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="50dac-114">Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="50dac-114">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="50dac-115">riskLevel</span><span class="sxs-lookup"><span data-stu-id="50dac-115">riskLevel</span></span>|<span data-ttu-id="50dac-116">Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="50dac-116">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="50dac-117">Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="50dac-117">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="50dac-118">Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="50dac-118">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="50dac-119">riskLeve</span><span class="sxs-lookup"><span data-stu-id="50dac-119">riskLeve</span></span>|<span data-ttu-id="50dac-120">Enthält die Risikostufe eine Anmeldung bei der Anmeldung (d. h. basierend auf die Risikoereignisse in Echtzeit).</span><span class="sxs-lookup"><span data-stu-id="50dac-120">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="50dac-121">Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="50dac-121">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="50dac-122">Der Wert `hidden` bedeutet, dass der Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="50dac-122">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="50dac-123">riskState</span><span class="sxs-lookup"><span data-stu-id="50dac-123">riskState</span></span>|<span data-ttu-id="50dac-124">Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="50dac-124">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="50dac-125">Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="50dac-125">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50dac-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50dac-126">JSON representation</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

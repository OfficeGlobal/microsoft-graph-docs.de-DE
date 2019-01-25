---
title: Ressourcentyp riskyUsers
description: Stellt Azure AD-Benutzer, die gefährdet sind. Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 27c189a81d6ba4e088c1242acfd2cf0d0f5c56c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515713"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="92711-105">Ressourcentyp riskyUsers</span><span class="sxs-lookup"><span data-stu-id="92711-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92711-106">Stellt Azure AD-Benutzer, die gefährdet sind.</span><span class="sxs-lookup"><span data-stu-id="92711-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="92711-107">Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko.</span><span class="sxs-lookup"><span data-stu-id="92711-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="92711-108">Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="92711-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="92711-109">**Hinweis:** Diese API ist eine Azure AD Premium P2-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="92711-109">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="92711-110">Weitere Informationen zu Risiken-Ereignissen finden Sie unter [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="92711-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="92711-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="92711-111">Methods</span></span>

| <span data-ttu-id="92711-112">Methode</span><span class="sxs-lookup"><span data-stu-id="92711-112">Method</span></span>   | <span data-ttu-id="92711-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="92711-113">Return Type</span></span>|<span data-ttu-id="92711-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92711-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92711-115">Liste riskyUsers</span><span class="sxs-lookup"><span data-stu-id="92711-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="92711-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="92711-116">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="92711-117">Liste riskant Benutzer und deren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="92711-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="92711-118">Abrufen von riskyUsers</span><span class="sxs-lookup"><span data-stu-id="92711-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="92711-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="92711-119">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="92711-120">Rufen Sie einen bestimmten Benutzer riskant und seine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="92711-120">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="92711-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="92711-121">Properties</span></span>

| <span data-ttu-id="92711-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92711-122">Property</span></span>   | <span data-ttu-id="92711-123">Typ</span><span class="sxs-lookup"><span data-stu-id="92711-123">Type</span></span>|<span data-ttu-id="92711-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92711-124">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="92711-125">Eindeutige Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="92711-125">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="92711-126">Gibt an, ob der Benutzer gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="92711-126">Indicates whether the user is deleted.</span></span> <span data-ttu-id="92711-127">Mögliche Werte sind: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="92711-127">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="92711-128">Gibt an, ob der Benutzer ein Gastbenutzer ist.</span><span class="sxs-lookup"><span data-stu-id="92711-128">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="92711-129">Mögliche Werte sind: `true` und `false`.</span><span class="sxs-lookup"><span data-stu-id="92711-129">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="92711-130">True, wenn die Identität des Benutzers im Hinblick auf die außerhalb der Mandant in Erwägung.</span><span class="sxs-lookup"><span data-stu-id="92711-130">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="92711-131">Dieser Benutzer kann sein, eine B2B oder B2C Benutzer mit der Identität in Azure AD, MSA oder 3. Partei Identitätsanbieter vertraut wird.</span><span class="sxs-lookup"><span data-stu-id="92711-131">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="92711-132">False, wenn die Identität des Benutzers im Hinblick auf die in den Mandanten in Erwägung</span><span class="sxs-lookup"><span data-stu-id="92711-132">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="92711-133">Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="92711-133">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="92711-134">Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="92711-134">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="92711-135">Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="92711-135">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="92711-136">Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="92711-136">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="92711-137">Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="92711-137">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="92711-138">Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="92711-138">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="92711-139">Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="92711-139">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="92711-140">Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="92711-140">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="92711-141">Datum und Uhrzeit der letzten Aktualisierung der Benutzer riskant.</span><span class="sxs-lookup"><span data-stu-id="92711-141">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="92711-142">Anzeigename des Benutzers riskant.</span><span class="sxs-lookup"><span data-stu-id="92711-142">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="92711-143">Benutzerprinzipalname riskant.</span><span class="sxs-lookup"><span data-stu-id="92711-143">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="92711-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="92711-144">Relationships</span></span>

| <span data-ttu-id="92711-145">Beziehung</span><span class="sxs-lookup"><span data-stu-id="92711-145">Relationship</span></span> | <span data-ttu-id="92711-146">Typ</span><span class="sxs-lookup"><span data-stu-id="92711-146">Type</span></span> |<span data-ttu-id="92711-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92711-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92711-148">id</span><span class="sxs-lookup"><span data-stu-id="92711-148">id</span></span>|<span data-ttu-id="92711-149">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="92711-149">UserObjectId</span></span>| <span data-ttu-id="92711-150">Der eindeutige Bezeichner des Benutzers, mit denen ein bestimmtes Risiko-Ereignis zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="92711-150">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="92711-151">isGuest</span><span class="sxs-lookup"><span data-stu-id="92711-151">isGuest</span></span>|<span data-ttu-id="92711-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="92711-152">isGuest</span></span>| <span data-ttu-id="92711-153">Ein riskant Benutzer kann entweder ein Home-Benutzer (B2E) oder ein Gast (B2B, B2C) sein.</span><span class="sxs-lookup"><span data-stu-id="92711-153">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="92711-154">isDeleted</span><span class="sxs-lookup"><span data-stu-id="92711-154">isDeleted</span></span>|<span data-ttu-id="92711-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="92711-155">isDeleted</span></span>| <span data-ttu-id="92711-156">Ein Benutzer kann oder kann nicht gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="92711-156">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="92711-157">riskState</span><span class="sxs-lookup"><span data-stu-id="92711-157">riskState</span></span>|<span data-ttu-id="92711-158">riskState</span><span class="sxs-lookup"><span data-stu-id="92711-158">riskState</span></span>| <span data-ttu-id="92711-159">Ein Benutzer riskant konnte in einem mehrerer Zustände vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="92711-159">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="92711-160">riskDetail</span><span class="sxs-lookup"><span data-stu-id="92711-160">riskDetail</span></span>|<span data-ttu-id="92711-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="92711-161">riskDetail</span></span>| <span data-ttu-id="92711-162">Ein riskant Benutzer konnte aus mehreren Gründen in einem bestimmten Zustand sein.</span><span class="sxs-lookup"><span data-stu-id="92711-162">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="92711-163">riskLevel</span><span class="sxs-lookup"><span data-stu-id="92711-163">riskLevel</span></span>|<span data-ttu-id="92711-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="92711-164">riskLevel</span></span>| <span data-ttu-id="92711-165">Ein riskant Benutzer kann eine der mehrere Risikoebenen betrachtet werden.</span><span class="sxs-lookup"><span data-stu-id="92711-165">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92711-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92711-166">JSON representation</span></span>

<span data-ttu-id="92711-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92711-167">Here is a JSON representation of the resource.</span></span>

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

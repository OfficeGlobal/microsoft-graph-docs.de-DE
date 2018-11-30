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
# <a name="riskyusers-resource-type"></a><span data-ttu-id="c072f-105">Ressourcentyp riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c072f-105">riskyUsers resource type</span></span>

> <span data-ttu-id="c072f-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c072f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c072f-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c072f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c072f-108">Stellt Azure AD-Benutzer, die gefährdet sind.</span><span class="sxs-lookup"><span data-stu-id="c072f-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="c072f-109">Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko.</span><span class="sxs-lookup"><span data-stu-id="c072f-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="c072f-110">Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c072f-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="c072f-111">Weitere Informationen zu Risiken-Ereignissen finden Sie unter [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="c072f-111">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="c072f-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="c072f-112">Methods</span></span>

| <span data-ttu-id="c072f-113">Methode</span><span class="sxs-lookup"><span data-stu-id="c072f-113">Method</span></span>   | <span data-ttu-id="c072f-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c072f-114">Return Type</span></span>|<span data-ttu-id="c072f-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c072f-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c072f-116">Liste riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c072f-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="c072f-117">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c072f-117">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="c072f-118">Liste riskant Benutzer und deren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c072f-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="c072f-119">Abrufen von riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c072f-119">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="c072f-120">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c072f-120">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="c072f-121">Rufen Sie einen bestimmten Benutzer riskant und seine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="c072f-121">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="c072f-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c072f-122">Properties</span></span>

| <span data-ttu-id="c072f-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c072f-123">Property</span></span>   | <span data-ttu-id="c072f-124">Typ</span><span class="sxs-lookup"><span data-stu-id="c072f-124">Type</span></span>|<span data-ttu-id="c072f-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c072f-125">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="c072f-126">Eindeutige Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="c072f-126">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="c072f-127">Gibt an, ob der Benutzer gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="c072f-127">Indicates whether the user is deleted.</span></span> <span data-ttu-id="c072f-128">Mögliche Werte sind: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="c072f-128">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="c072f-129">Gibt an, ob der Benutzer ein Gastbenutzer ist.</span><span class="sxs-lookup"><span data-stu-id="c072f-129">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="c072f-130">Mögliche Werte sind: `true` und `false`.</span><span class="sxs-lookup"><span data-stu-id="c072f-130">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="c072f-131">True, wenn die Identität des Benutzers im Hinblick auf die außerhalb der Mandant in Erwägung.</span><span class="sxs-lookup"><span data-stu-id="c072f-131">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="c072f-132">Dieser Benutzer kann sein, eine B2B oder B2C Benutzer mit der Identität in Azure AD, MSA oder 3. Partei Identitätsanbieter vertraut wird.</span><span class="sxs-lookup"><span data-stu-id="c072f-132">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="c072f-133">False, wenn die Identität des Benutzers im Hinblick auf die in den Mandanten in Erwägung</span><span class="sxs-lookup"><span data-stu-id="c072f-133">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="c072f-134">Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="c072f-134">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="c072f-135">Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c072f-135">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="c072f-136">Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="c072f-136">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="c072f-137">Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="c072f-137">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="c072f-138">Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c072f-138">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="c072f-139">Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="c072f-139">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="c072f-140">Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="c072f-140">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="c072f-141">Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c072f-141">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="c072f-142">Datum und Uhrzeit der letzten Aktualisierung der Benutzer riskant.</span><span class="sxs-lookup"><span data-stu-id="c072f-142">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="c072f-143">Anzeigename des Benutzers riskant.</span><span class="sxs-lookup"><span data-stu-id="c072f-143">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="c072f-144">Benutzerprinzipalname riskant.</span><span class="sxs-lookup"><span data-stu-id="c072f-144">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="c072f-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c072f-145">Relationships</span></span>

| <span data-ttu-id="c072f-146">Beziehung</span><span class="sxs-lookup"><span data-stu-id="c072f-146">Relationship</span></span> | <span data-ttu-id="c072f-147">Typ</span><span class="sxs-lookup"><span data-stu-id="c072f-147">Type</span></span> |<span data-ttu-id="c072f-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c072f-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c072f-149">id</span><span class="sxs-lookup"><span data-stu-id="c072f-149">id</span></span>|<span data-ttu-id="c072f-150">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="c072f-150">UserObjectId</span></span>| <span data-ttu-id="c072f-151">Der eindeutige Bezeichner des Benutzers, mit denen ein bestimmtes Risiko-Ereignis zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="c072f-151">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="c072f-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="c072f-152">isGuest</span></span>|<span data-ttu-id="c072f-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="c072f-153">isGuest</span></span>| <span data-ttu-id="c072f-154">Ein riskant Benutzer kann entweder ein Home-Benutzer (B2E) oder ein Gast (B2B, B2C) sein.</span><span class="sxs-lookup"><span data-stu-id="c072f-154">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="c072f-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c072f-155">isDeleted</span></span>|<span data-ttu-id="c072f-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c072f-156">isDeleted</span></span>| <span data-ttu-id="c072f-157">Ein Benutzer kann oder kann nicht gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="c072f-157">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="c072f-158">riskState</span><span class="sxs-lookup"><span data-stu-id="c072f-158">riskState</span></span>|<span data-ttu-id="c072f-159">riskState</span><span class="sxs-lookup"><span data-stu-id="c072f-159">riskState</span></span>| <span data-ttu-id="c072f-160">Ein Benutzer riskant konnte in einem mehrerer Zustände vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="c072f-160">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="c072f-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c072f-161">riskDetail</span></span>|<span data-ttu-id="c072f-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c072f-162">riskDetail</span></span>| <span data-ttu-id="c072f-163">Ein riskant Benutzer konnte aus mehreren Gründen in einem bestimmten Zustand sein.</span><span class="sxs-lookup"><span data-stu-id="c072f-163">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="c072f-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c072f-164">riskLevel</span></span>|<span data-ttu-id="c072f-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c072f-165">riskLevel</span></span>| <span data-ttu-id="c072f-166">Ein riskant Benutzer kann eine der mehrere Risikoebenen betrachtet werden.</span><span class="sxs-lookup"><span data-stu-id="c072f-166">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c072f-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c072f-167">JSON representation</span></span>

<span data-ttu-id="c072f-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c072f-168">Here is a JSON representation of the resource.</span></span>

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

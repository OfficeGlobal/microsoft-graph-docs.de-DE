---
title: Ressourcentyp riskyUsers
description: Stellt Azure AD-Benutzer, die gefährdet sind. Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: bb1dab6461a3b235d461720a68855f1e8f3f70d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871554"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="e424a-105">Ressourcentyp riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e424a-105">riskyUsers resource type</span></span>

> <span data-ttu-id="e424a-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e424a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e424a-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e424a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e424a-108">Stellt Azure AD-Benutzer, die gefährdet sind.</span><span class="sxs-lookup"><span data-stu-id="e424a-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="e424a-109">Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko.</span><span class="sxs-lookup"><span data-stu-id="e424a-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="e424a-110">Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e424a-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="e424a-111">**Hinweis:** Diese API ist eine Azure AD Premium P2-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e424a-111">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="e424a-112">Weitere Informationen zu Risiken-Ereignissen finden Sie unter [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="e424a-112">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="e424a-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="e424a-113">Methods</span></span>

| <span data-ttu-id="e424a-114">Methode</span><span class="sxs-lookup"><span data-stu-id="e424a-114">Method</span></span>   | <span data-ttu-id="e424a-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e424a-115">Return Type</span></span>|<span data-ttu-id="e424a-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e424a-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e424a-117">Liste riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e424a-117">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="e424a-118">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e424a-118">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="e424a-119">Liste riskant Benutzer und deren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="e424a-119">List risky users and their properties.</span></span>|
|[<span data-ttu-id="e424a-120">Abrufen von riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e424a-120">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="e424a-121">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e424a-121">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="e424a-122">Rufen Sie einen bestimmten Benutzer riskant und seine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="e424a-122">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="e424a-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e424a-123">Properties</span></span>

| <span data-ttu-id="e424a-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e424a-124">Property</span></span>   | <span data-ttu-id="e424a-125">Typ</span><span class="sxs-lookup"><span data-stu-id="e424a-125">Type</span></span>|<span data-ttu-id="e424a-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e424a-126">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="e424a-127">Eindeutige Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="e424a-127">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="e424a-128">Gibt an, ob der Benutzer gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="e424a-128">Indicates whether the user is deleted.</span></span> <span data-ttu-id="e424a-129">Mögliche Werte sind: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="e424a-129">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="e424a-130">Gibt an, ob der Benutzer ein Gastbenutzer ist.</span><span class="sxs-lookup"><span data-stu-id="e424a-130">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="e424a-131">Mögliche Werte sind: `true` und `false`.</span><span class="sxs-lookup"><span data-stu-id="e424a-131">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="e424a-132">True, wenn die Identität des Benutzers im Hinblick auf die außerhalb der Mandant in Erwägung.</span><span class="sxs-lookup"><span data-stu-id="e424a-132">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="e424a-133">Dieser Benutzer kann sein, eine B2B oder B2C Benutzer mit der Identität in Azure AD, MSA oder 3. Partei Identitätsanbieter vertraut wird.</span><span class="sxs-lookup"><span data-stu-id="e424a-133">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="e424a-134">False, wenn die Identität des Benutzers im Hinblick auf die in den Mandanten in Erwägung</span><span class="sxs-lookup"><span data-stu-id="e424a-134">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="e424a-135">Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="e424a-135">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="e424a-136">Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e424a-136">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="e424a-137">Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="e424a-137">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="e424a-138">Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="e424a-138">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="e424a-139">Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e424a-139">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="e424a-140">Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e424a-140">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="e424a-141">Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="e424a-141">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="e424a-142">Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e424a-142">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="e424a-143">Datum und Uhrzeit der letzten Aktualisierung der Benutzer riskant.</span><span class="sxs-lookup"><span data-stu-id="e424a-143">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="e424a-144">Anzeigename des Benutzers riskant.</span><span class="sxs-lookup"><span data-stu-id="e424a-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="e424a-145">Benutzerprinzipalname riskant.</span><span class="sxs-lookup"><span data-stu-id="e424a-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="e424a-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e424a-146">Relationships</span></span>

| <span data-ttu-id="e424a-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e424a-147">Relationship</span></span> | <span data-ttu-id="e424a-148">Typ</span><span class="sxs-lookup"><span data-stu-id="e424a-148">Type</span></span> |<span data-ttu-id="e424a-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e424a-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e424a-150">id</span><span class="sxs-lookup"><span data-stu-id="e424a-150">id</span></span>|<span data-ttu-id="e424a-151">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="e424a-151">UserObjectId</span></span>| <span data-ttu-id="e424a-152">Der eindeutige Bezeichner des Benutzers, mit denen ein bestimmtes Risiko-Ereignis zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="e424a-152">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="e424a-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="e424a-153">isGuest</span></span>|<span data-ttu-id="e424a-154">isGuest</span><span class="sxs-lookup"><span data-stu-id="e424a-154">isGuest</span></span>| <span data-ttu-id="e424a-155">Ein riskant Benutzer kann entweder ein Home-Benutzer (B2E) oder ein Gast (B2B, B2C) sein.</span><span class="sxs-lookup"><span data-stu-id="e424a-155">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="e424a-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e424a-156">isDeleted</span></span>|<span data-ttu-id="e424a-157">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e424a-157">isDeleted</span></span>| <span data-ttu-id="e424a-158">Ein Benutzer kann oder kann nicht gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="e424a-158">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="e424a-159">riskState</span><span class="sxs-lookup"><span data-stu-id="e424a-159">riskState</span></span>|<span data-ttu-id="e424a-160">riskState</span><span class="sxs-lookup"><span data-stu-id="e424a-160">riskState</span></span>| <span data-ttu-id="e424a-161">Ein Benutzer riskant konnte in einem mehrerer Zustände vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="e424a-161">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="e424a-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e424a-162">riskDetail</span></span>|<span data-ttu-id="e424a-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e424a-163">riskDetail</span></span>| <span data-ttu-id="e424a-164">Ein riskant Benutzer konnte aus mehreren Gründen in einem bestimmten Zustand sein.</span><span class="sxs-lookup"><span data-stu-id="e424a-164">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="e424a-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e424a-165">riskLevel</span></span>|<span data-ttu-id="e424a-166">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e424a-166">riskLevel</span></span>| <span data-ttu-id="e424a-167">Ein riskant Benutzer kann eine der mehrere Risikoebenen betrachtet werden.</span><span class="sxs-lookup"><span data-stu-id="e424a-167">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e424a-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e424a-168">JSON representation</span></span>

<span data-ttu-id="e424a-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e424a-169">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

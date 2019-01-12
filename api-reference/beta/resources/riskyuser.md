---
title: Ressourcentyp riskyUsers
description: Stellt Azure AD-Benutzer, die gefährdet sind. Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko. Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 2e4cf47ea78583958c79750e0b2ad4fa12230d22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950732"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="1489d-105">Ressourcentyp riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1489d-105">riskyUsers resource type</span></span>

> <span data-ttu-id="1489d-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1489d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1489d-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1489d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1489d-108">Stellt Azure AD-Benutzer, die gefährdet sind.</span><span class="sxs-lookup"><span data-stu-id="1489d-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="1489d-109">Azure AD ständig wertet basierend auf verschiedenen Signale und Computer Learning Benutzer Risiko.</span><span class="sxs-lookup"><span data-stu-id="1489d-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="1489d-110">Diese API ermöglicht den programmgesteuerten Zugriff auf alle Risiko Benutzer in Ihrer Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1489d-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="1489d-111">**Hinweis:** Diese API ist eine Azure AD Premium P2-Lizenz erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1489d-111">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="1489d-112">Weitere Informationen zu Risiken-Ereignissen finden Sie unter [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="1489d-112">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="1489d-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="1489d-113">Methods</span></span>

| <span data-ttu-id="1489d-114">Methode</span><span class="sxs-lookup"><span data-stu-id="1489d-114">Method</span></span>   | <span data-ttu-id="1489d-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1489d-115">Return Type</span></span>|<span data-ttu-id="1489d-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1489d-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1489d-117">Liste riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1489d-117">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="1489d-118">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1489d-118">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="1489d-119">Liste riskant Benutzer und deren Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="1489d-119">List risky users and their properties.</span></span>|
|[<span data-ttu-id="1489d-120">Abrufen von riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1489d-120">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="1489d-121">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1489d-121">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="1489d-122">Rufen Sie einen bestimmten Benutzer riskant und seine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="1489d-122">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="1489d-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1489d-123">Properties</span></span>

| <span data-ttu-id="1489d-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1489d-124">Property</span></span>   | <span data-ttu-id="1489d-125">Typ</span><span class="sxs-lookup"><span data-stu-id="1489d-125">Type</span></span>|<span data-ttu-id="1489d-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1489d-126">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="1489d-127">Eindeutige Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="1489d-127">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="1489d-128">Gibt an, ob der Benutzer gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="1489d-128">Indicates whether the user is deleted.</span></span> <span data-ttu-id="1489d-129">Mögliche Werte sind: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="1489d-129">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="1489d-130">Gibt an, ob der Benutzer ein Gastbenutzer ist.</span><span class="sxs-lookup"><span data-stu-id="1489d-130">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="1489d-131">Mögliche Werte sind: `true` und `false`.</span><span class="sxs-lookup"><span data-stu-id="1489d-131">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="1489d-132">True, wenn die Identität des Benutzers im Hinblick auf die außerhalb der Mandant in Erwägung.</span><span class="sxs-lookup"><span data-stu-id="1489d-132">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="1489d-133">Dieser Benutzer kann sein, eine B2B oder B2C Benutzer mit der Identität in Azure AD, MSA oder 3. Partei Identitätsanbieter vertraut wird.</span><span class="sxs-lookup"><span data-stu-id="1489d-133">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="1489d-134">False, wenn die Identität des Benutzers im Hinblick auf die in den Mandanten in Erwägung</span><span class="sxs-lookup"><span data-stu-id="1489d-134">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="1489d-135">Stellt die "Ursache" hinter einem bestimmten Zustand eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="1489d-135">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="1489d-136">Die möglichen Werte sind: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1489d-136">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="1489d-137">Der Wert `none` bedeutet, dass keine Aktion in der Benutzer oder die Anmeldung bisher ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="1489d-137">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="1489d-138">Stellt die allgemeinen Risikostufe eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="1489d-138">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="1489d-139">Die möglichen Werte sind: `none`, `low`, `medium`, `high`, `hidden`, und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1489d-139">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="1489d-140">Der Wert `hidden` bedeutet, dass der Benutzer oder die Anmeldung wurde für den Schutz von Azure Active Directory-Identität nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="1489d-140">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="1489d-141">Stellt den 'Risiko Zustand"eines Benutzers riskant, Anmeldung oder ein Risikoereignis bereit.</span><span class="sxs-lookup"><span data-stu-id="1489d-141">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="1489d-142">Die möglichen Werte sind: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1489d-142">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="1489d-143">Datum und Uhrzeit der letzten Aktualisierung der Benutzer riskant.</span><span class="sxs-lookup"><span data-stu-id="1489d-143">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="1489d-144">Anzeigename des Benutzers riskant.</span><span class="sxs-lookup"><span data-stu-id="1489d-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="1489d-145">Benutzerprinzipalname riskant.</span><span class="sxs-lookup"><span data-stu-id="1489d-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="1489d-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1489d-146">Relationships</span></span>

| <span data-ttu-id="1489d-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1489d-147">Relationship</span></span> | <span data-ttu-id="1489d-148">Typ</span><span class="sxs-lookup"><span data-stu-id="1489d-148">Type</span></span> |<span data-ttu-id="1489d-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1489d-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1489d-150">id</span><span class="sxs-lookup"><span data-stu-id="1489d-150">id</span></span>|<span data-ttu-id="1489d-151">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="1489d-151">UserObjectId</span></span>| <span data-ttu-id="1489d-152">Der eindeutige Bezeichner des Benutzers, mit denen ein bestimmtes Risiko-Ereignis zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="1489d-152">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="1489d-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="1489d-153">isGuest</span></span>|<span data-ttu-id="1489d-154">isGuest</span><span class="sxs-lookup"><span data-stu-id="1489d-154">isGuest</span></span>| <span data-ttu-id="1489d-155">Ein riskant Benutzer kann entweder ein Home-Benutzer (B2E) oder ein Gast (B2B, B2C) sein.</span><span class="sxs-lookup"><span data-stu-id="1489d-155">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="1489d-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1489d-156">isDeleted</span></span>|<span data-ttu-id="1489d-157">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1489d-157">isDeleted</span></span>| <span data-ttu-id="1489d-158">Ein Benutzer kann oder kann nicht gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="1489d-158">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="1489d-159">riskState</span><span class="sxs-lookup"><span data-stu-id="1489d-159">riskState</span></span>|<span data-ttu-id="1489d-160">riskState</span><span class="sxs-lookup"><span data-stu-id="1489d-160">riskState</span></span>| <span data-ttu-id="1489d-161">Ein Benutzer riskant konnte in einem mehrerer Zustände vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="1489d-161">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="1489d-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="1489d-162">riskDetail</span></span>|<span data-ttu-id="1489d-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="1489d-163">riskDetail</span></span>| <span data-ttu-id="1489d-164">Ein riskant Benutzer konnte aus mehreren Gründen in einem bestimmten Zustand sein.</span><span class="sxs-lookup"><span data-stu-id="1489d-164">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="1489d-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1489d-165">riskLevel</span></span>|<span data-ttu-id="1489d-166">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1489d-166">riskLevel</span></span>| <span data-ttu-id="1489d-167">Ein riskant Benutzer kann eine der mehrere Risikoebenen betrachtet werden.</span><span class="sxs-lookup"><span data-stu-id="1489d-167">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1489d-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1489d-168">JSON representation</span></span>

<span data-ttu-id="1489d-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1489d-169">Here is a JSON representation of the resource.</span></span>

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

---
title: Ressourcentyp identityRiskEvent
description: 'Ein Risikoereignis von Azure Active Directory-Identität Protection erkannt. Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:'
ms.openlocfilehash: e61f5e0dc2dae2c055636e3fd3737e16b2558458
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059833"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="11e83-104">Ressourcentyp identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-104">identityRiskEvent resource type</span></span>

> <span data-ttu-id="11e83-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="11e83-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11e83-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11e83-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11e83-107">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)erkannt.</span><span class="sxs-lookup"><span data-stu-id="11e83-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="11e83-108">Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:</span><span class="sxs-lookup"><span data-stu-id="11e83-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="11e83-109">Ereignistyp</span><span class="sxs-lookup"><span data-stu-id="11e83-109">Event type</span></span>         | <span data-ttu-id="11e83-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11e83-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="11e83-111">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="11e83-112">Anmeldungen von anonymen IP-Adressen.</span><span class="sxs-lookup"><span data-stu-id="11e83-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="11e83-113">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="11e83-114">Anmeldungen von Geräten Malware infiziert.</span><span class="sxs-lookup"><span data-stu-id="11e83-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="11e83-115">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="11e83-116">Unmöglich Reisen zu untypischen Speicherorte.</span><span class="sxs-lookup"><span data-stu-id="11e83-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="11e83-117">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="11e83-118">Benutzer mit verlorene Anmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="11e83-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="11e83-119">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="11e83-120">Anmeldungen von verdächtigen IP-Adressen.</span><span class="sxs-lookup"><span data-stu-id="11e83-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="11e83-121">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="11e83-122">Anmeldungen von Speicherorten nicht vertraut sind.</span><span class="sxs-lookup"><span data-stu-id="11e83-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="11e83-123">Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="11e83-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="11e83-124">Methoden</span><span class="sxs-lookup"><span data-stu-id="11e83-124">Methods</span></span>

| <span data-ttu-id="11e83-125">Methode</span><span class="sxs-lookup"><span data-stu-id="11e83-125">Method</span></span>           | <span data-ttu-id="11e83-126">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="11e83-126">Return Type</span></span>    |<span data-ttu-id="11e83-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11e83-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11e83-128">Abrufen von identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="11e83-129">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11e83-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="11e83-130">Lesen Sie Eigenschaften und Beziehungen des IdentityRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="11e83-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11e83-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11e83-131">Properties</span></span>
| <span data-ttu-id="11e83-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11e83-132">Property</span></span>     | <span data-ttu-id="11e83-133">Typ</span><span class="sxs-lookup"><span data-stu-id="11e83-133">Type</span></span>   |<span data-ttu-id="11e83-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11e83-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11e83-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="11e83-135">closedDateTime</span></span>|<span data-ttu-id="11e83-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11e83-136">dateTimeOffset</span></span>| <span data-ttu-id="11e83-137">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="11e83-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="11e83-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11e83-138">createdDateTime</span></span>|<span data-ttu-id="11e83-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11e83-139">dateTimeOffset</span></span>| <span data-ttu-id="11e83-140">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="11e83-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="11e83-141">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="11e83-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="11e83-142">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="11e83-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="11e83-143">id</span><span class="sxs-lookup"><span data-stu-id="11e83-143">id</span></span>|<span data-ttu-id="11e83-144">string</span><span class="sxs-lookup"><span data-stu-id="11e83-144">string</span></span>| <span data-ttu-id="11e83-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="11e83-145">Read-only</span></span>|
|<span data-ttu-id="11e83-146">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="11e83-146">riskEventDateTime</span></span>|<span data-ttu-id="11e83-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11e83-147">dateTimeOffset</span></span>| <span data-ttu-id="11e83-148">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="11e83-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="11e83-149">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="11e83-149">riskEventStatus</span></span>|<span data-ttu-id="11e83-150">string</span><span class="sxs-lookup"><span data-stu-id="11e83-150">string</span></span>| <span data-ttu-id="11e83-151">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="11e83-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="11e83-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="11e83-152">riskLevel</span></span>|<span data-ttu-id="11e83-153">string</span><span class="sxs-lookup"><span data-stu-id="11e83-153">string</span></span>| <span data-ttu-id="11e83-154">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="11e83-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="11e83-155">riskEventType</span><span class="sxs-lookup"><span data-stu-id="11e83-155">riskEventType</span></span>|<span data-ttu-id="11e83-156">string</span><span class="sxs-lookup"><span data-stu-id="11e83-156">string</span></span>| <span data-ttu-id="11e83-157">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="11e83-157">The type of risk</span></span>|
|<span data-ttu-id="11e83-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="11e83-158">userDisplayName</span></span>|<span data-ttu-id="11e83-159">string</span><span class="sxs-lookup"><span data-stu-id="11e83-159">string</span></span>| <span data-ttu-id="11e83-160">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="11e83-160">The name of the user at risk</span></span>|
|<span data-ttu-id="11e83-161">userId</span><span class="sxs-lookup"><span data-stu-id="11e83-161">userId</span></span>|<span data-ttu-id="11e83-162">string</span><span class="sxs-lookup"><span data-stu-id="11e83-162">string</span></span>| <span data-ttu-id="11e83-163">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="11e83-163">The id of the user at risk</span></span>|
|<span data-ttu-id="11e83-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="11e83-164">userPrincipalName</span></span>|<span data-ttu-id="11e83-165">string</span><span class="sxs-lookup"><span data-stu-id="11e83-165">string</span></span>| <span data-ttu-id="11e83-166">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="11e83-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="11e83-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="11e83-167">Relationships</span></span>
| <span data-ttu-id="11e83-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="11e83-168">Relationship</span></span> | <span data-ttu-id="11e83-169">Typ</span><span class="sxs-lookup"><span data-stu-id="11e83-169">Type</span></span>   |<span data-ttu-id="11e83-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11e83-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11e83-171">impactedUser</span><span class="sxs-lookup"><span data-stu-id="11e83-171">impactedUser</span></span>|[<span data-ttu-id="11e83-172">Benutzer</span><span class="sxs-lookup"><span data-stu-id="11e83-172">user</span></span>](user.md)| <span data-ttu-id="11e83-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="11e83-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11e83-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11e83-175">JSON representation</span></span>

<span data-ttu-id="11e83-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11e83-176">Here is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
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
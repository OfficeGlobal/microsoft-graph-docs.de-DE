---
title: Ressourcentyp identityRiskEvent
description: 'Ein Risikoereignis von Azure Active Directory-Identität Protection erkannt. Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:'
author: cloudhandler
ms.openlocfilehash: 4abe473b47d3ce52fd5b75b6adfd08dbc4af54fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351738"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="7c11f-104">Ressourcentyp identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-104">identityRiskEvent resource type</span></span>

> <span data-ttu-id="7c11f-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7c11f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c11f-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c11f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c11f-107">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)erkannt.</span><span class="sxs-lookup"><span data-stu-id="7c11f-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="7c11f-108">Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:</span><span class="sxs-lookup"><span data-stu-id="7c11f-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="7c11f-109">Ereignistyp</span><span class="sxs-lookup"><span data-stu-id="7c11f-109">Event type</span></span>         | <span data-ttu-id="7c11f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c11f-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="7c11f-111">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="7c11f-112">Anmeldungen von anonymen IP-Adressen.</span><span class="sxs-lookup"><span data-stu-id="7c11f-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="7c11f-113">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="7c11f-114">Anmeldungen von Geräten Malware infiziert.</span><span class="sxs-lookup"><span data-stu-id="7c11f-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="7c11f-115">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="7c11f-116">Unmöglich Reisen zu untypischen Speicherorte.</span><span class="sxs-lookup"><span data-stu-id="7c11f-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="7c11f-117">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="7c11f-118">Benutzer mit verlorene Anmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="7c11f-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="7c11f-119">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="7c11f-120">Anmeldungen von verdächtigen IP-Adressen.</span><span class="sxs-lookup"><span data-stu-id="7c11f-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="7c11f-121">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="7c11f-122">Anmeldungen von Speicherorten nicht vertraut sind.</span><span class="sxs-lookup"><span data-stu-id="7c11f-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="7c11f-123">Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="7c11f-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="7c11f-124">Methoden</span><span class="sxs-lookup"><span data-stu-id="7c11f-124">Methods</span></span>

| <span data-ttu-id="7c11f-125">Methode</span><span class="sxs-lookup"><span data-stu-id="7c11f-125">Method</span></span>           | <span data-ttu-id="7c11f-126">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7c11f-126">Return Type</span></span>    |<span data-ttu-id="7c11f-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c11f-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c11f-128">Abrufen von identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="7c11f-129">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7c11f-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="7c11f-130">Lesen Sie Eigenschaften und Beziehungen des IdentityRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7c11f-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c11f-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7c11f-131">Properties</span></span>
| <span data-ttu-id="7c11f-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c11f-132">Property</span></span>     | <span data-ttu-id="7c11f-133">Typ</span><span class="sxs-lookup"><span data-stu-id="7c11f-133">Type</span></span>   |<span data-ttu-id="7c11f-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c11f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c11f-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c11f-135">closedDateTime</span></span>|<span data-ttu-id="7c11f-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c11f-136">dateTimeOffset</span></span>| <span data-ttu-id="7c11f-137">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="7c11f-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="7c11f-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c11f-138">createdDateTime</span></span>|<span data-ttu-id="7c11f-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c11f-139">dateTimeOffset</span></span>| <span data-ttu-id="7c11f-140">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7c11f-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="7c11f-141">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="7c11f-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="7c11f-142">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="7c11f-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="7c11f-143">id</span><span class="sxs-lookup"><span data-stu-id="7c11f-143">id</span></span>|<span data-ttu-id="7c11f-144">string</span><span class="sxs-lookup"><span data-stu-id="7c11f-144">string</span></span>| <span data-ttu-id="7c11f-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7c11f-145">Read-only</span></span>|
|<span data-ttu-id="7c11f-146">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="7c11f-146">riskEventDateTime</span></span>|<span data-ttu-id="7c11f-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c11f-147">dateTimeOffset</span></span>| <span data-ttu-id="7c11f-148">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="7c11f-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="7c11f-149">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="7c11f-149">riskEventStatus</span></span>|<span data-ttu-id="7c11f-150">string</span><span class="sxs-lookup"><span data-stu-id="7c11f-150">string</span></span>| <span data-ttu-id="7c11f-151">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="7c11f-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="7c11f-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="7c11f-152">riskLevel</span></span>|<span data-ttu-id="7c11f-153">string</span><span class="sxs-lookup"><span data-stu-id="7c11f-153">string</span></span>| <span data-ttu-id="7c11f-154">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="7c11f-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="7c11f-155">riskEventType</span><span class="sxs-lookup"><span data-stu-id="7c11f-155">riskEventType</span></span>|<span data-ttu-id="7c11f-156">string</span><span class="sxs-lookup"><span data-stu-id="7c11f-156">string</span></span>| <span data-ttu-id="7c11f-157">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="7c11f-157">The type of risk</span></span>|
|<span data-ttu-id="7c11f-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7c11f-158">userDisplayName</span></span>|<span data-ttu-id="7c11f-159">string</span><span class="sxs-lookup"><span data-stu-id="7c11f-159">string</span></span>| <span data-ttu-id="7c11f-160">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="7c11f-160">The name of the user at risk</span></span>|
|<span data-ttu-id="7c11f-161">userId</span><span class="sxs-lookup"><span data-stu-id="7c11f-161">userId</span></span>|<span data-ttu-id="7c11f-162">string</span><span class="sxs-lookup"><span data-stu-id="7c11f-162">string</span></span>| <span data-ttu-id="7c11f-163">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="7c11f-163">The id of the user at risk</span></span>|
|<span data-ttu-id="7c11f-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7c11f-164">userPrincipalName</span></span>|<span data-ttu-id="7c11f-165">string</span><span class="sxs-lookup"><span data-stu-id="7c11f-165">string</span></span>| <span data-ttu-id="7c11f-166">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="7c11f-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c11f-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7c11f-167">Relationships</span></span>
| <span data-ttu-id="7c11f-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7c11f-168">Relationship</span></span> | <span data-ttu-id="7c11f-169">Typ</span><span class="sxs-lookup"><span data-stu-id="7c11f-169">Type</span></span>   |<span data-ttu-id="7c11f-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c11f-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c11f-171">impactedUser</span><span class="sxs-lookup"><span data-stu-id="7c11f-171">impactedUser</span></span>|[<span data-ttu-id="7c11f-172">Benutzer</span><span class="sxs-lookup"><span data-stu-id="7c11f-172">user</span></span>](user.md)| <span data-ttu-id="7c11f-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7c11f-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c11f-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7c11f-175">JSON representation</span></span>

<span data-ttu-id="7c11f-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7c11f-176">Here is a JSON representation of the resource.</span></span> 

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
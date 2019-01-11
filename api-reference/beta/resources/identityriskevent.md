---
title: Ressourcentyp identityRiskEvent
description: 'Ein Risikoereignis von Azure Active Directory-Identität Protection erkannt. Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:'
author: cloudhandler
localization_priority: Normal
ms.openlocfilehash: 0735599c260fac178b54ee4ba54a17f5ea027e23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858996"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="7caac-104">Ressourcentyp identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-104">identityRiskEvent resource type</span></span>

> <span data-ttu-id="7caac-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7caac-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7caac-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7caac-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7caac-107">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)erkannt.</span><span class="sxs-lookup"><span data-stu-id="7caac-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="7caac-108">Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:</span><span class="sxs-lookup"><span data-stu-id="7caac-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="7caac-109">Ereignistyp</span><span class="sxs-lookup"><span data-stu-id="7caac-109">Event type</span></span>         | <span data-ttu-id="7caac-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7caac-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="7caac-111">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="7caac-112">Anmeldungen von anonymen IP-Adressen.</span><span class="sxs-lookup"><span data-stu-id="7caac-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="7caac-113">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="7caac-114">Anmeldungen von Geräten Malware infiziert.</span><span class="sxs-lookup"><span data-stu-id="7caac-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="7caac-115">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="7caac-116">Unmöglich Reisen zu untypischen Speicherorte.</span><span class="sxs-lookup"><span data-stu-id="7caac-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="7caac-117">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="7caac-118">Benutzer mit verlorene Anmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="7caac-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="7caac-119">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="7caac-120">Anmeldungen von verdächtigen IP-Adressen.</span><span class="sxs-lookup"><span data-stu-id="7caac-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="7caac-121">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="7caac-122">Anmeldungen von Speicherorten nicht vertraut sind.</span><span class="sxs-lookup"><span data-stu-id="7caac-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="7caac-123">Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="7caac-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="7caac-124">Methoden</span><span class="sxs-lookup"><span data-stu-id="7caac-124">Methods</span></span>

| <span data-ttu-id="7caac-125">Methode</span><span class="sxs-lookup"><span data-stu-id="7caac-125">Method</span></span>           | <span data-ttu-id="7caac-126">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7caac-126">Return Type</span></span>    |<span data-ttu-id="7caac-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7caac-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7caac-128">Abrufen von identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="7caac-129">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7caac-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="7caac-130">Lesen Sie Eigenschaften und Beziehungen des IdentityRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7caac-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7caac-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7caac-131">Properties</span></span>
| <span data-ttu-id="7caac-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7caac-132">Property</span></span>     | <span data-ttu-id="7caac-133">Typ</span><span class="sxs-lookup"><span data-stu-id="7caac-133">Type</span></span>   |<span data-ttu-id="7caac-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7caac-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7caac-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="7caac-135">closedDateTime</span></span>|<span data-ttu-id="7caac-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7caac-136">dateTimeOffset</span></span>| <span data-ttu-id="7caac-137">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="7caac-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="7caac-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7caac-138">createdDateTime</span></span>|<span data-ttu-id="7caac-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7caac-139">dateTimeOffset</span></span>| <span data-ttu-id="7caac-140">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7caac-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="7caac-141">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="7caac-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="7caac-142">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="7caac-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="7caac-143">id</span><span class="sxs-lookup"><span data-stu-id="7caac-143">id</span></span>|<span data-ttu-id="7caac-144">string</span><span class="sxs-lookup"><span data-stu-id="7caac-144">string</span></span>| <span data-ttu-id="7caac-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7caac-145">Read-only</span></span>|
|<span data-ttu-id="7caac-146">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="7caac-146">riskEventDateTime</span></span>|<span data-ttu-id="7caac-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7caac-147">dateTimeOffset</span></span>| <span data-ttu-id="7caac-148">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="7caac-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="7caac-149">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="7caac-149">riskEventStatus</span></span>|<span data-ttu-id="7caac-150">string</span><span class="sxs-lookup"><span data-stu-id="7caac-150">string</span></span>| <span data-ttu-id="7caac-151">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="7caac-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="7caac-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="7caac-152">riskLevel</span></span>|<span data-ttu-id="7caac-153">string</span><span class="sxs-lookup"><span data-stu-id="7caac-153">string</span></span>| <span data-ttu-id="7caac-154">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="7caac-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="7caac-155">riskEventType</span><span class="sxs-lookup"><span data-stu-id="7caac-155">riskEventType</span></span>|<span data-ttu-id="7caac-156">string</span><span class="sxs-lookup"><span data-stu-id="7caac-156">string</span></span>| <span data-ttu-id="7caac-157">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="7caac-157">The type of risk</span></span>|
|<span data-ttu-id="7caac-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7caac-158">userDisplayName</span></span>|<span data-ttu-id="7caac-159">string</span><span class="sxs-lookup"><span data-stu-id="7caac-159">string</span></span>| <span data-ttu-id="7caac-160">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="7caac-160">The name of the user at risk</span></span>|
|<span data-ttu-id="7caac-161">userId</span><span class="sxs-lookup"><span data-stu-id="7caac-161">userId</span></span>|<span data-ttu-id="7caac-162">string</span><span class="sxs-lookup"><span data-stu-id="7caac-162">string</span></span>| <span data-ttu-id="7caac-163">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="7caac-163">The id of the user at risk</span></span>|
|<span data-ttu-id="7caac-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7caac-164">userPrincipalName</span></span>|<span data-ttu-id="7caac-165">string</span><span class="sxs-lookup"><span data-stu-id="7caac-165">string</span></span>| <span data-ttu-id="7caac-166">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="7caac-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="7caac-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7caac-167">Relationships</span></span>
| <span data-ttu-id="7caac-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7caac-168">Relationship</span></span> | <span data-ttu-id="7caac-169">Typ</span><span class="sxs-lookup"><span data-stu-id="7caac-169">Type</span></span>   |<span data-ttu-id="7caac-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7caac-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7caac-171">impactedUser</span><span class="sxs-lookup"><span data-stu-id="7caac-171">impactedUser</span></span>|[<span data-ttu-id="7caac-172">Benutzer</span><span class="sxs-lookup"><span data-stu-id="7caac-172">user</span></span>](user.md)| <span data-ttu-id="7caac-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7caac-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7caac-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7caac-175">JSON representation</span></span>

<span data-ttu-id="7caac-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7caac-176">Here is a JSON representation of the resource.</span></span> 

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

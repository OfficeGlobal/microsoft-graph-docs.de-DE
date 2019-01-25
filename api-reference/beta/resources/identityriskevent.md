---
title: Ressourcentyp identityRiskEvent
description: 'Ein Risikoereignis von Azure Active Directory-Identität Protection erkannt. Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514180"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="69e2c-104">Ressourcentyp identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69e2c-105">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)erkannt.</span><span class="sxs-lookup"><span data-stu-id="69e2c-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="69e2c-106">Es ist den Basistyp für jede bestimmte Risiko Ereignistyp:</span><span class="sxs-lookup"><span data-stu-id="69e2c-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="69e2c-107">Ereignistyp</span><span class="sxs-lookup"><span data-stu-id="69e2c-107">Event type</span></span>         | <span data-ttu-id="69e2c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69e2c-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="69e2c-109">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="69e2c-110">Anmeldungen von anonymen IP-Adressen.</span><span class="sxs-lookup"><span data-stu-id="69e2c-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="69e2c-111">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="69e2c-112">Anmeldungen von Geräten Malware infiziert.</span><span class="sxs-lookup"><span data-stu-id="69e2c-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="69e2c-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="69e2c-114">Unmöglich Reisen zu untypischen Speicherorte.</span><span class="sxs-lookup"><span data-stu-id="69e2c-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="69e2c-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="69e2c-116">Benutzer mit verlorene Anmeldeinformationen.</span><span class="sxs-lookup"><span data-stu-id="69e2c-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="69e2c-117">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="69e2c-118">Anmeldungen von verdächtigen IP-Adressen.</span><span class="sxs-lookup"><span data-stu-id="69e2c-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="69e2c-119">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="69e2c-120">Anmeldungen von Speicherorten nicht vertraut sind.</span><span class="sxs-lookup"><span data-stu-id="69e2c-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="69e2c-121">Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="69e2c-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="69e2c-122">Methoden</span><span class="sxs-lookup"><span data-stu-id="69e2c-122">Methods</span></span>

| <span data-ttu-id="69e2c-123">Methode</span><span class="sxs-lookup"><span data-stu-id="69e2c-123">Method</span></span>           | <span data-ttu-id="69e2c-124">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="69e2c-124">Return Type</span></span>    |<span data-ttu-id="69e2c-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69e2c-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69e2c-126">Abrufen von identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="69e2c-127">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="69e2c-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="69e2c-128">Lesen Sie Eigenschaften und Beziehungen des IdentityRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="69e2c-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69e2c-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69e2c-129">Properties</span></span>
| <span data-ttu-id="69e2c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69e2c-130">Property</span></span>     | <span data-ttu-id="69e2c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="69e2c-131">Type</span></span>   |<span data-ttu-id="69e2c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69e2c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69e2c-133">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="69e2c-133">closedDateTime</span></span>|<span data-ttu-id="69e2c-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e2c-134">dateTimeOffset</span></span>| <span data-ttu-id="69e2c-135">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="69e2c-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="69e2c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69e2c-136">createdDateTime</span></span>|<span data-ttu-id="69e2c-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e2c-137">dateTimeOffset</span></span>| <span data-ttu-id="69e2c-138">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="69e2c-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="69e2c-139">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="69e2c-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="69e2c-140">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="69e2c-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="69e2c-141">id</span><span class="sxs-lookup"><span data-stu-id="69e2c-141">id</span></span>|<span data-ttu-id="69e2c-142">string</span><span class="sxs-lookup"><span data-stu-id="69e2c-142">string</span></span>| <span data-ttu-id="69e2c-143">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="69e2c-143">Read-only</span></span>|
|<span data-ttu-id="69e2c-144">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="69e2c-144">riskEventDateTime</span></span>|<span data-ttu-id="69e2c-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e2c-145">dateTimeOffset</span></span>| <span data-ttu-id="69e2c-146">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="69e2c-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="69e2c-147">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="69e2c-147">riskEventStatus</span></span>|<span data-ttu-id="69e2c-148">string</span><span class="sxs-lookup"><span data-stu-id="69e2c-148">string</span></span>| <span data-ttu-id="69e2c-149">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="69e2c-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="69e2c-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="69e2c-150">riskLevel</span></span>|<span data-ttu-id="69e2c-151">string</span><span class="sxs-lookup"><span data-stu-id="69e2c-151">string</span></span>| <span data-ttu-id="69e2c-152">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="69e2c-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="69e2c-153">riskEventType</span><span class="sxs-lookup"><span data-stu-id="69e2c-153">riskEventType</span></span>|<span data-ttu-id="69e2c-154">string</span><span class="sxs-lookup"><span data-stu-id="69e2c-154">string</span></span>| <span data-ttu-id="69e2c-155">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="69e2c-155">The type of risk</span></span>|
|<span data-ttu-id="69e2c-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="69e2c-156">userDisplayName</span></span>|<span data-ttu-id="69e2c-157">string</span><span class="sxs-lookup"><span data-stu-id="69e2c-157">string</span></span>| <span data-ttu-id="69e2c-158">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="69e2c-158">The name of the user at risk</span></span>|
|<span data-ttu-id="69e2c-159">userId</span><span class="sxs-lookup"><span data-stu-id="69e2c-159">userId</span></span>|<span data-ttu-id="69e2c-160">string</span><span class="sxs-lookup"><span data-stu-id="69e2c-160">string</span></span>| <span data-ttu-id="69e2c-161">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="69e2c-161">The id of the user at risk</span></span>|
|<span data-ttu-id="69e2c-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="69e2c-162">userPrincipalName</span></span>|<span data-ttu-id="69e2c-163">string</span><span class="sxs-lookup"><span data-stu-id="69e2c-163">string</span></span>| <span data-ttu-id="69e2c-164">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="69e2c-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="69e2c-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69e2c-165">Relationships</span></span>
| <span data-ttu-id="69e2c-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="69e2c-166">Relationship</span></span> | <span data-ttu-id="69e2c-167">Typ</span><span class="sxs-lookup"><span data-stu-id="69e2c-167">Type</span></span>   |<span data-ttu-id="69e2c-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69e2c-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69e2c-169">impactedUser</span><span class="sxs-lookup"><span data-stu-id="69e2c-169">impactedUser</span></span>|[<span data-ttu-id="69e2c-170">user</span><span class="sxs-lookup"><span data-stu-id="69e2c-170">user</span></span>](user.md)| <span data-ttu-id="69e2c-p104">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="69e2c-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69e2c-173">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69e2c-173">JSON representation</span></span>

<span data-ttu-id="69e2c-174">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="69e2c-174">Here is a JSON representation of the resource.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

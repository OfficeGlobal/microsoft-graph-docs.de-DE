---
title: Ressourcentyp locatedRiskEvent
description: 'Ein Risikoereignis von Azure Active Directory-Identität Protection, die auf Standortdaten basiert erkannt. Befindet sich Risikotypen werden unterstützt:'
localization_priority: Normal
ms.openlocfilehash: 256c7a980fb9540e7e80337a5b8aad29fe73f26a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867557"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="8ee1e-104">Ressourcentyp locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8ee1e-104">locatedRiskEvent resource type</span></span>

> <span data-ttu-id="8ee1e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ee1e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ee1e-107">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , das auf Standortdaten erkannt.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="8ee1e-108">Befindet sich Risikotypen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="8ee1e-108">Located risk event types include:</span></span>
* [<span data-ttu-id="8ee1e-109">Anmeldungen von anonymen IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="8ee1e-109">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="8ee1e-110">Anmeldungen von Geräten Malware infiziert</span><span class="sxs-lookup"><span data-stu-id="8ee1e-110">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="8ee1e-111">unmöglich Reisen zu untypischen Speicherorte</span><span class="sxs-lookup"><span data-stu-id="8ee1e-111">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="8ee1e-112">Anmeldungen von verdächtigen IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="8ee1e-112">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="8ee1e-113">[Anmeldungen von unbekannten Standorten](unfamiliarlocationriskevent.md) Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="8ee1e-113">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="8ee1e-114">Methoden</span><span class="sxs-lookup"><span data-stu-id="8ee1e-114">Methods</span></span>

| <span data-ttu-id="8ee1e-115">Methode</span><span class="sxs-lookup"><span data-stu-id="8ee1e-115">Method</span></span>           | <span data-ttu-id="8ee1e-116">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8ee1e-116">Return Type</span></span>    |<span data-ttu-id="8ee1e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ee1e-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ee1e-118">Abrufen von locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8ee1e-118">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="8ee1e-119">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="8ee1e-119">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="8ee1e-120">Lesen Sie Eigenschaften und Beziehungen des LocatedRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-120">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ee1e-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8ee1e-121">Properties</span></span>
| <span data-ttu-id="8ee1e-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8ee1e-122">Property</span></span>     | <span data-ttu-id="8ee1e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="8ee1e-123">Type</span></span>   |<span data-ttu-id="8ee1e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ee1e-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ee1e-125">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee1e-125">closedDateTime</span></span>|<span data-ttu-id="8ee1e-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee1e-126">dateTimeOffset</span></span>| <span data-ttu-id="8ee1e-127">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="8ee1e-127">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="8ee1e-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee1e-128">createdDateTime</span></span>|<span data-ttu-id="8ee1e-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee1e-129">dateTimeOffset</span></span>| <span data-ttu-id="8ee1e-130">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-130">The date and time that the risk event was created.</span></span> <span data-ttu-id="8ee1e-131">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-131">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="8ee1e-132">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-132">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="8ee1e-133">id</span><span class="sxs-lookup"><span data-stu-id="8ee1e-133">id</span></span>|<span data-ttu-id="8ee1e-134">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-134">string</span></span>| <span data-ttu-id="8ee1e-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-135">Read-only</span></span>|
|<span data-ttu-id="8ee1e-136">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8ee1e-136">ipAddress</span></span>|<span data-ttu-id="8ee1e-137">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-137">string</span></span>| <span data-ttu-id="8ee1e-138">Die IP-Adresse von der Anmeldung</span><span class="sxs-lookup"><span data-stu-id="8ee1e-138">The IP address of the sign-in</span></span>|
|<span data-ttu-id="8ee1e-139">location</span><span class="sxs-lookup"><span data-stu-id="8ee1e-139">location</span></span>|<span data-ttu-id="8ee1e-140">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-140">string</span></span>| <span data-ttu-id="8ee1e-141">Die Position, die IP-Adresse von der Anmeldung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="8ee1e-141">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="8ee1e-142">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="8ee1e-142">riskEventDateTime</span></span>|<span data-ttu-id="8ee1e-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee1e-143">dateTimeOffset</span></span>| <span data-ttu-id="8ee1e-144">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="8ee1e-144">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="8ee1e-145">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="8ee1e-145">riskEventStatus</span></span>|<span data-ttu-id="8ee1e-146">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-146">string</span></span>| <span data-ttu-id="8ee1e-147">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-147">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="8ee1e-148">riskLevel</span><span class="sxs-lookup"><span data-stu-id="8ee1e-148">riskLevel</span></span>|<span data-ttu-id="8ee1e-149">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-149">string</span></span>| <span data-ttu-id="8ee1e-150">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-150">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="8ee1e-151">riskEventType</span><span class="sxs-lookup"><span data-stu-id="8ee1e-151">riskEventType</span></span>|<span data-ttu-id="8ee1e-152">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-152">string</span></span>| <span data-ttu-id="8ee1e-153">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="8ee1e-153">The type of risk</span></span>|
|<span data-ttu-id="8ee1e-154">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8ee1e-154">userDisplayName</span></span>|<span data-ttu-id="8ee1e-155">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-155">string</span></span>| <span data-ttu-id="8ee1e-156">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="8ee1e-156">The name of the user at risk</span></span>|
|<span data-ttu-id="8ee1e-157">userId</span><span class="sxs-lookup"><span data-stu-id="8ee1e-157">userId</span></span>|<span data-ttu-id="8ee1e-158">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-158">string</span></span>| <span data-ttu-id="8ee1e-159">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="8ee1e-159">The id of the user at risk</span></span>|
|<span data-ttu-id="8ee1e-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8ee1e-160">userPrincipalName</span></span>|<span data-ttu-id="8ee1e-161">string</span><span class="sxs-lookup"><span data-stu-id="8ee1e-161">string</span></span>| <span data-ttu-id="8ee1e-162">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="8ee1e-162">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ee1e-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8ee1e-163">Relationships</span></span>
| <span data-ttu-id="8ee1e-164">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8ee1e-164">Relationship</span></span> | <span data-ttu-id="8ee1e-165">Typ</span><span class="sxs-lookup"><span data-stu-id="8ee1e-165">Type</span></span>   |<span data-ttu-id="8ee1e-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ee1e-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ee1e-167">impactedUser</span><span class="sxs-lookup"><span data-stu-id="8ee1e-167">impactedUser</span></span>|[<span data-ttu-id="8ee1e-168">Benutzer</span><span class="sxs-lookup"><span data-stu-id="8ee1e-168">user</span></span>](user.md)| <span data-ttu-id="8ee1e-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ee1e-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8ee1e-171">JSON representation</span></span>

<span data-ttu-id="8ee1e-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8ee1e-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locatedRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

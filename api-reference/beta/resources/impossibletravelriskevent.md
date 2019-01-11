---
title: Ressourcentyp impossibleTravelRiskEvent
description: Ein Risikoereignis von Azure Active Directory-Identität Protection, in dem zwei Konto Anmeldungen von Speicherorten für den Benutzer untypischen auftreten, und es ist nicht möglich, zwischen den Standorten in die Dauer zwischen den Anmelde-ins umfassende Informationen zum Reisen, erkannt Risikoereignisse finden Sie in der Dokumentation zu Azure AD-Schutz.
localization_priority: Normal
ms.openlocfilehash: e9ce064a5ea724b498f3290f630a4169b1aef897
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846452"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="693a2-103">Ressourcentyp impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="693a2-103">impossibleTravelRiskEvent resource type</span></span>

> <span data-ttu-id="693a2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="693a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="693a2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="693a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="693a2-106">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , in dem zwei Konto Anmeldungen von Speicherorten für den Benutzer untypischen auftreten, und es ist nicht möglich, zwischen den Standorten in die Dauer zwischen den Anmelde-Ins vollständig Reisen, erkannt Informationen zu Risiken-Ereignissen finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="693a2-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="693a2-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="693a2-107">Methods</span></span>

| <span data-ttu-id="693a2-108">Methode</span><span class="sxs-lookup"><span data-stu-id="693a2-108">Method</span></span>           | <span data-ttu-id="693a2-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="693a2-109">Return Type</span></span>    |<span data-ttu-id="693a2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693a2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="693a2-111">Abrufen von impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="693a2-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="693a2-112">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="693a2-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="693a2-113">Lesen Sie Eigenschaften und Beziehungen des ImpossibleTravelRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="693a2-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="693a2-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="693a2-114">Properties</span></span>
| <span data-ttu-id="693a2-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="693a2-115">Property</span></span>     | <span data-ttu-id="693a2-116">Typ</span><span class="sxs-lookup"><span data-stu-id="693a2-116">Type</span></span>   |<span data-ttu-id="693a2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693a2-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="693a2-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="693a2-118">closedDateTime</span></span>|<span data-ttu-id="693a2-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="693a2-119">dateTimeOffset</span></span>| <span data-ttu-id="693a2-120">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="693a2-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="693a2-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="693a2-121">createdDateTime</span></span>|<span data-ttu-id="693a2-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="693a2-122">dateTimeOffset</span></span>| <span data-ttu-id="693a2-123">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="693a2-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="693a2-124">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="693a2-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="693a2-125">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="693a2-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="693a2-126">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="693a2-126">deviceInformation</span></span>|<span data-ttu-id="693a2-127">string</span><span class="sxs-lookup"><span data-stu-id="693a2-127">string</span></span>| <span data-ttu-id="693a2-128">Informationen über das Gerät</span><span class="sxs-lookup"><span data-stu-id="693a2-128">Information about the device</span></span>|
|<span data-ttu-id="693a2-129">id</span><span class="sxs-lookup"><span data-stu-id="693a2-129">id</span></span>|<span data-ttu-id="693a2-130">string</span><span class="sxs-lookup"><span data-stu-id="693a2-130">string</span></span>| <span data-ttu-id="693a2-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="693a2-131">Read-only</span></span>|
|<span data-ttu-id="693a2-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="693a2-132">ipAddress</span></span>|<span data-ttu-id="693a2-133">string</span><span class="sxs-lookup"><span data-stu-id="693a2-133">string</span></span>| <span data-ttu-id="693a2-134">Die IP-Adresse des zweiten Anmeldung</span><span class="sxs-lookup"><span data-stu-id="693a2-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="693a2-135">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="693a2-135">isAtypicalLocation</span></span>|<span data-ttu-id="693a2-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="693a2-136">boolean</span></span>| <span data-ttu-id="693a2-137">Wenn eine der Speicherorte untypischen für den Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="693a2-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="693a2-138">location</span><span class="sxs-lookup"><span data-stu-id="693a2-138">location</span></span>|<span data-ttu-id="693a2-139">string</span><span class="sxs-lookup"><span data-stu-id="693a2-139">string</span></span>| <span data-ttu-id="693a2-140">Die Position, die IP-Adresse des zweiten Anmeldung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="693a2-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="693a2-141">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="693a2-141">previousIPAddress</span></span>|<span data-ttu-id="693a2-142">string</span><span class="sxs-lookup"><span data-stu-id="693a2-142">string</span></span>| <span data-ttu-id="693a2-143">Die IP-Adresse von der ersten Anmeldung</span><span class="sxs-lookup"><span data-stu-id="693a2-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="693a2-144">previousLocation</span><span class="sxs-lookup"><span data-stu-id="693a2-144">previousLocation</span></span>|<span data-ttu-id="693a2-145">string</span><span class="sxs-lookup"><span data-stu-id="693a2-145">string</span></span>| <span data-ttu-id="693a2-146">Die Position, die IP-Adresse von der ersten Anmeldung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="693a2-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="693a2-147">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="693a2-147">previousSigninDateTime</span></span>|<span data-ttu-id="693a2-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="693a2-148">dateTimeOffset</span></span>| <span data-ttu-id="693a2-149">Datum und Uhrzeit der ersten Anmeldung</span><span class="sxs-lookup"><span data-stu-id="693a2-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="693a2-150">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="693a2-150">riskEventDateTime</span></span>|<span data-ttu-id="693a2-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="693a2-151">dateTimeOffset</span></span>| <span data-ttu-id="693a2-152">Datum und Uhrzeit des zweiten Anmeldung</span><span class="sxs-lookup"><span data-stu-id="693a2-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="693a2-153">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="693a2-153">riskEventStatus</span></span>|<span data-ttu-id="693a2-154">string</span><span class="sxs-lookup"><span data-stu-id="693a2-154">string</span></span>| <span data-ttu-id="693a2-155">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="693a2-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="693a2-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="693a2-156">riskLevel</span></span>|<span data-ttu-id="693a2-157">string</span><span class="sxs-lookup"><span data-stu-id="693a2-157">string</span></span>| <span data-ttu-id="693a2-158">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="693a2-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="693a2-159">riskEventType</span><span class="sxs-lookup"><span data-stu-id="693a2-159">riskEventType</span></span>|<span data-ttu-id="693a2-160">string</span><span class="sxs-lookup"><span data-stu-id="693a2-160">string</span></span>| <span data-ttu-id="693a2-161">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="693a2-161">The type of risk</span></span>|
|<span data-ttu-id="693a2-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="693a2-162">userAgent</span></span>|<span data-ttu-id="693a2-163">string</span><span class="sxs-lookup"><span data-stu-id="693a2-163">string</span></span>| <span data-ttu-id="693a2-164">Benutzeragentzeichenfolge des Browsers</span><span class="sxs-lookup"><span data-stu-id="693a2-164">The browser's user agent string</span></span>|
|<span data-ttu-id="693a2-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="693a2-165">userDisplayName</span></span>|<span data-ttu-id="693a2-166">string</span><span class="sxs-lookup"><span data-stu-id="693a2-166">string</span></span>| <span data-ttu-id="693a2-167">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="693a2-167">The name of the user at risk</span></span>|
|<span data-ttu-id="693a2-168">userId</span><span class="sxs-lookup"><span data-stu-id="693a2-168">userId</span></span>|<span data-ttu-id="693a2-169">string</span><span class="sxs-lookup"><span data-stu-id="693a2-169">string</span></span>| <span data-ttu-id="693a2-170">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="693a2-170">The id of the user at risk</span></span>|
|<span data-ttu-id="693a2-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="693a2-171">userPrincipalName</span></span>|<span data-ttu-id="693a2-172">string</span><span class="sxs-lookup"><span data-stu-id="693a2-172">string</span></span>| <span data-ttu-id="693a2-173">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="693a2-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="693a2-174">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="693a2-174">Relationships</span></span>
| <span data-ttu-id="693a2-175">Beziehung</span><span class="sxs-lookup"><span data-stu-id="693a2-175">Relationship</span></span> | <span data-ttu-id="693a2-176">Typ</span><span class="sxs-lookup"><span data-stu-id="693a2-176">Type</span></span>   |<span data-ttu-id="693a2-177">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693a2-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="693a2-178">impactedUser</span><span class="sxs-lookup"><span data-stu-id="693a2-178">impactedUser</span></span>|[<span data-ttu-id="693a2-179">Benutzer</span><span class="sxs-lookup"><span data-stu-id="693a2-179">user</span></span>](user.md)| <span data-ttu-id="693a2-p103">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="693a2-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="693a2-182">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="693a2-182">JSON representation</span></span>

<span data-ttu-id="693a2-183">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="693a2-183">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

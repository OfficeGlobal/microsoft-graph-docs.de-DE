---
title: Ressourcentyp impossibleTravelRiskEvent
description: Ein Risikoereignis von Azure Active Directory-Identität Protection, in dem zwei Konto Anmeldungen von Speicherorten für den Benutzer untypischen auftreten, und es ist nicht möglich, zwischen den Standorten in die Dauer zwischen den Anmelde-ins umfassende Informationen zum Reisen, erkannt Risikoereignisse finden Sie in der Dokumentation zu Azure AD-Schutz.
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529383"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="cbba6-103">Ressourcentyp impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="cbba6-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbba6-104">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , in dem zwei Konto Anmeldungen von Speicherorten für den Benutzer untypischen auftreten, und es ist nicht möglich, zwischen den Standorten in die Dauer zwischen den Anmelde-Ins vollständig Reisen, erkannt Informationen zu Risiken-Ereignissen finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="cbba6-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="cbba6-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="cbba6-105">Methods</span></span>

| <span data-ttu-id="cbba6-106">Methode</span><span class="sxs-lookup"><span data-stu-id="cbba6-106">Method</span></span>           | <span data-ttu-id="cbba6-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cbba6-107">Return Type</span></span>    |<span data-ttu-id="cbba6-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbba6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbba6-109">Abrufen von impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="cbba6-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="cbba6-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="cbba6-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="cbba6-111">Lesen Sie Eigenschaften und Beziehungen des ImpossibleTravelRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cbba6-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbba6-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cbba6-112">Properties</span></span>
| <span data-ttu-id="cbba6-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cbba6-113">Property</span></span>     | <span data-ttu-id="cbba6-114">Typ</span><span class="sxs-lookup"><span data-stu-id="cbba6-114">Type</span></span>   |<span data-ttu-id="cbba6-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbba6-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbba6-116">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbba6-116">closedDateTime</span></span>|<span data-ttu-id="cbba6-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbba6-117">dateTimeOffset</span></span>| <span data-ttu-id="cbba6-118">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="cbba6-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="cbba6-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbba6-119">createdDateTime</span></span>|<span data-ttu-id="cbba6-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbba6-120">dateTimeOffset</span></span>| <span data-ttu-id="cbba6-121">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="cbba6-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="cbba6-122">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="cbba6-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="cbba6-123">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="cbba6-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="cbba6-124">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="cbba6-124">deviceInformation</span></span>|<span data-ttu-id="cbba6-125">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-125">string</span></span>| <span data-ttu-id="cbba6-126">Informationen über das Gerät</span><span class="sxs-lookup"><span data-stu-id="cbba6-126">Information about the device</span></span>|
|<span data-ttu-id="cbba6-127">id</span><span class="sxs-lookup"><span data-stu-id="cbba6-127">id</span></span>|<span data-ttu-id="cbba6-128">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-128">string</span></span>| <span data-ttu-id="cbba6-129">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="cbba6-129">Read-only</span></span>|
|<span data-ttu-id="cbba6-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="cbba6-130">ipAddress</span></span>|<span data-ttu-id="cbba6-131">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-131">string</span></span>| <span data-ttu-id="cbba6-132">Die IP-Adresse des zweiten Anmeldung</span><span class="sxs-lookup"><span data-stu-id="cbba6-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="cbba6-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="cbba6-133">isAtypicalLocation</span></span>|<span data-ttu-id="cbba6-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cbba6-134">boolean</span></span>| <span data-ttu-id="cbba6-135">Wenn eine der Speicherorte untypischen für den Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="cbba6-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="cbba6-136">location</span><span class="sxs-lookup"><span data-stu-id="cbba6-136">location</span></span>|<span data-ttu-id="cbba6-137">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-137">string</span></span>| <span data-ttu-id="cbba6-138">Die Position, die IP-Adresse des zweiten Anmeldung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="cbba6-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="cbba6-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="cbba6-139">previousIPAddress</span></span>|<span data-ttu-id="cbba6-140">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-140">string</span></span>| <span data-ttu-id="cbba6-141">Die IP-Adresse von der ersten Anmeldung</span><span class="sxs-lookup"><span data-stu-id="cbba6-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="cbba6-142">previousLocation</span><span class="sxs-lookup"><span data-stu-id="cbba6-142">previousLocation</span></span>|<span data-ttu-id="cbba6-143">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-143">string</span></span>| <span data-ttu-id="cbba6-144">Die Position, die IP-Adresse von der ersten Anmeldung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="cbba6-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="cbba6-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="cbba6-145">previousSigninDateTime</span></span>|<span data-ttu-id="cbba6-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbba6-146">dateTimeOffset</span></span>| <span data-ttu-id="cbba6-147">Datum und Uhrzeit der ersten Anmeldung</span><span class="sxs-lookup"><span data-stu-id="cbba6-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="cbba6-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="cbba6-148">riskEventDateTime</span></span>|<span data-ttu-id="cbba6-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbba6-149">dateTimeOffset</span></span>| <span data-ttu-id="cbba6-150">Datum und Uhrzeit des zweiten Anmeldung</span><span class="sxs-lookup"><span data-stu-id="cbba6-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="cbba6-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="cbba6-151">riskEventStatus</span></span>|<span data-ttu-id="cbba6-152">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-152">string</span></span>| <span data-ttu-id="cbba6-153">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="cbba6-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="cbba6-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="cbba6-154">riskLevel</span></span>|<span data-ttu-id="cbba6-155">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-155">string</span></span>| <span data-ttu-id="cbba6-156">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="cbba6-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="cbba6-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="cbba6-157">riskEventType</span></span>|<span data-ttu-id="cbba6-158">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-158">string</span></span>| <span data-ttu-id="cbba6-159">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="cbba6-159">The type of risk</span></span>|
|<span data-ttu-id="cbba6-160">UserAgent</span><span class="sxs-lookup"><span data-stu-id="cbba6-160">userAgent</span></span>|<span data-ttu-id="cbba6-161">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-161">string</span></span>| <span data-ttu-id="cbba6-162">Benutzeragentzeichenfolge des Browsers</span><span class="sxs-lookup"><span data-stu-id="cbba6-162">The browser's user agent string</span></span>|
|<span data-ttu-id="cbba6-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="cbba6-163">userDisplayName</span></span>|<span data-ttu-id="cbba6-164">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-164">string</span></span>| <span data-ttu-id="cbba6-165">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="cbba6-165">The name of the user at risk</span></span>|
|<span data-ttu-id="cbba6-166">userId</span><span class="sxs-lookup"><span data-stu-id="cbba6-166">userId</span></span>|<span data-ttu-id="cbba6-167">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-167">string</span></span>| <span data-ttu-id="cbba6-168">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="cbba6-168">The id of the user at risk</span></span>|
|<span data-ttu-id="cbba6-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cbba6-169">userPrincipalName</span></span>|<span data-ttu-id="cbba6-170">string</span><span class="sxs-lookup"><span data-stu-id="cbba6-170">string</span></span>| <span data-ttu-id="cbba6-171">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="cbba6-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbba6-172">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cbba6-172">Relationships</span></span>
| <span data-ttu-id="cbba6-173">Beziehung</span><span class="sxs-lookup"><span data-stu-id="cbba6-173">Relationship</span></span> | <span data-ttu-id="cbba6-174">Typ</span><span class="sxs-lookup"><span data-stu-id="cbba6-174">Type</span></span>   |<span data-ttu-id="cbba6-175">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbba6-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbba6-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="cbba6-176">impactedUser</span></span>|[<span data-ttu-id="cbba6-177">user</span><span class="sxs-lookup"><span data-stu-id="cbba6-177">user</span></span>](user.md)| <span data-ttu-id="cbba6-p102">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="cbba6-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbba6-180">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cbba6-180">JSON representation</span></span>

<span data-ttu-id="cbba6-181">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cbba6-181">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

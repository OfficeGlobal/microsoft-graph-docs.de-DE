---
title: Ressourcentyp anonymousIpRiskEvent
description: Ein Risikoereignis von Azure Active Directory-Identität Protection, wo ein Konto-Anmeldung aus einer IP-Adresse, die angezeigt wird versucht wird, einen anonymen, erkannt. Umfassende Informationen zum Risiko-Ereignissen finden Sie in der Dokumentation zu Azure AD-Schutz.
localization_priority: Normal
ms.openlocfilehash: 9c170e234116ca76e4dabe021c0aa7949d1a66ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848300"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="0e45f-104">Ressourcentyp anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0e45f-104">anonymousIpRiskEvent resource type</span></span>

> <span data-ttu-id="0e45f-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e45f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e45f-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e45f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e45f-107">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , wo ein Konto-Anmeldung aus einer IP-Adresse, die angezeigt wird versucht wird, einen anonymen, erkannt.</span><span class="sxs-lookup"><span data-stu-id="0e45f-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="0e45f-108">Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="0e45f-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="0e45f-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="0e45f-109">Methods</span></span>

| <span data-ttu-id="0e45f-110">Methode</span><span class="sxs-lookup"><span data-stu-id="0e45f-110">Method</span></span>           | <span data-ttu-id="0e45f-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0e45f-111">Return Type</span></span>    |<span data-ttu-id="0e45f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e45f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e45f-113">Abrufen von anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0e45f-113">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="0e45f-114">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0e45f-114">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="0e45f-115">Lesen Sie Eigenschaften und Beziehungen des AnonymousIpRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e45f-115">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e45f-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e45f-116">Properties</span></span>
| <span data-ttu-id="0e45f-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e45f-117">Property</span></span>     | <span data-ttu-id="0e45f-118">Typ</span><span class="sxs-lookup"><span data-stu-id="0e45f-118">Type</span></span>   |<span data-ttu-id="0e45f-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e45f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e45f-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e45f-120">closedDateTime</span></span>|<span data-ttu-id="0e45f-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e45f-121">dateTimeOffset</span></span>| <span data-ttu-id="0e45f-122">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="0e45f-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="0e45f-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e45f-123">createdDateTime</span></span>|<span data-ttu-id="0e45f-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e45f-124">dateTimeOffset</span></span>| <span data-ttu-id="0e45f-125">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="0e45f-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="0e45f-126">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="0e45f-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="0e45f-127">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="0e45f-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="0e45f-128">id</span><span class="sxs-lookup"><span data-stu-id="0e45f-128">id</span></span>|<span data-ttu-id="0e45f-129">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-129">string</span></span>| <span data-ttu-id="0e45f-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0e45f-130">Read-only</span></span>|
|<span data-ttu-id="0e45f-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0e45f-131">ipAddress</span></span>|<span data-ttu-id="0e45f-132">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-132">string</span></span>| <span data-ttu-id="0e45f-133">Die IP-Adresse von der Anmeldung</span><span class="sxs-lookup"><span data-stu-id="0e45f-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="0e45f-134">location</span><span class="sxs-lookup"><span data-stu-id="0e45f-134">location</span></span>|<span data-ttu-id="0e45f-135">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-135">string</span></span>| <span data-ttu-id="0e45f-136">Die Position, die IP-Adresse von der Anmeldung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="0e45f-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="0e45f-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="0e45f-137">riskEventDateTime</span></span>|<span data-ttu-id="0e45f-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e45f-138">dateTimeOffset</span></span>| <span data-ttu-id="0e45f-139">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="0e45f-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="0e45f-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="0e45f-140">riskEventStatus</span></span>|<span data-ttu-id="0e45f-141">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-141">string</span></span>| <span data-ttu-id="0e45f-142">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="0e45f-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="0e45f-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0e45f-143">riskLevel</span></span>|<span data-ttu-id="0e45f-144">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-144">string</span></span>| <span data-ttu-id="0e45f-145">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="0e45f-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="0e45f-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="0e45f-146">riskEventType</span></span>|<span data-ttu-id="0e45f-147">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-147">string</span></span>| <span data-ttu-id="0e45f-148">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="0e45f-148">The type of risk</span></span>|
|<span data-ttu-id="0e45f-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0e45f-149">userDisplayName</span></span>|<span data-ttu-id="0e45f-150">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-150">string</span></span>| <span data-ttu-id="0e45f-151">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="0e45f-151">The name of the user at risk</span></span>|
|<span data-ttu-id="0e45f-152">userId</span><span class="sxs-lookup"><span data-stu-id="0e45f-152">userId</span></span>|<span data-ttu-id="0e45f-153">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-153">string</span></span>| <span data-ttu-id="0e45f-154">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="0e45f-154">The id of the user at risk</span></span>|
|<span data-ttu-id="0e45f-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e45f-155">userPrincipalName</span></span>|<span data-ttu-id="0e45f-156">string</span><span class="sxs-lookup"><span data-stu-id="0e45f-156">string</span></span>| <span data-ttu-id="0e45f-157">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="0e45f-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e45f-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0e45f-158">Relationships</span></span>
| <span data-ttu-id="0e45f-159">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0e45f-159">Relationship</span></span> | <span data-ttu-id="0e45f-160">Typ</span><span class="sxs-lookup"><span data-stu-id="0e45f-160">Type</span></span>   |<span data-ttu-id="0e45f-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e45f-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e45f-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="0e45f-162">impactedUser</span></span>|[<span data-ttu-id="0e45f-163">Benutzer</span><span class="sxs-lookup"><span data-stu-id="0e45f-163">user</span></span>](user.md)| <span data-ttu-id="0e45f-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0e45f-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e45f-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0e45f-166">JSON representation</span></span>

<span data-ttu-id="0e45f-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0e45f-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

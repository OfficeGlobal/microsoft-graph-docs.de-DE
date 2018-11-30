---
title: Ressourcentyp leakedCredentialsRiskEvent
description: Ein Risikoereignis von Azure Active Directory-Identität Protection, in dem ein Konto Anmeldeinformationen in der Natur erkannt wurden, erkannt. Umfassende Informationen zum Risiko-Ereignissen finden Sie in der Dokumentation zu Azure AD-Schutz.
ms.openlocfilehash: 2404564726c3ca7ee1f577b3d81daaa339941406
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064482"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="54be5-104">Ressourcentyp leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="54be5-104">leakedCredentialsRiskEvent resource type</span></span>

> <span data-ttu-id="54be5-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54be5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54be5-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54be5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54be5-107">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , in dem ein Konto Anmeldeinformationen in der Natur erkannt wurden, erkannt.</span><span class="sxs-lookup"><span data-stu-id="54be5-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="54be5-108">Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="54be5-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="54be5-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="54be5-109">Methods</span></span>

| <span data-ttu-id="54be5-110">Methode</span><span class="sxs-lookup"><span data-stu-id="54be5-110">Method</span></span>           | <span data-ttu-id="54be5-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="54be5-111">Return Type</span></span>    |<span data-ttu-id="54be5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54be5-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54be5-113">Abrufen von leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="54be5-113">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="54be5-114">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="54be5-114">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="54be5-115">Lesen Sie Eigenschaften und Beziehungen des LeakedCredentialsRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="54be5-115">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="54be5-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54be5-116">Properties</span></span>
| <span data-ttu-id="54be5-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54be5-117">Property</span></span>     | <span data-ttu-id="54be5-118">Typ</span><span class="sxs-lookup"><span data-stu-id="54be5-118">Type</span></span>   |<span data-ttu-id="54be5-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54be5-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54be5-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="54be5-120">closedDateTime</span></span>|<span data-ttu-id="54be5-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54be5-121">dateTimeOffset</span></span>| <span data-ttu-id="54be5-122">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="54be5-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="54be5-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54be5-123">createdDateTime</span></span>|<span data-ttu-id="54be5-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54be5-124">dateTimeOffset</span></span>| <span data-ttu-id="54be5-125">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="54be5-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="54be5-126">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="54be5-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="54be5-127">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="54be5-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="54be5-128">id</span><span class="sxs-lookup"><span data-stu-id="54be5-128">id</span></span>|<span data-ttu-id="54be5-129">string</span><span class="sxs-lookup"><span data-stu-id="54be5-129">string</span></span>| <span data-ttu-id="54be5-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="54be5-130">Read-only</span></span>|
|<span data-ttu-id="54be5-131">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="54be5-131">riskEventDateTime</span></span>|<span data-ttu-id="54be5-132">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54be5-132">dateTimeOffset</span></span>| <span data-ttu-id="54be5-133">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="54be5-133">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="54be5-134">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="54be5-134">riskEventStatus</span></span>|<span data-ttu-id="54be5-135">string</span><span class="sxs-lookup"><span data-stu-id="54be5-135">string</span></span>| <span data-ttu-id="54be5-136">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="54be5-136">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="54be5-137">riskLevel</span><span class="sxs-lookup"><span data-stu-id="54be5-137">riskLevel</span></span>|<span data-ttu-id="54be5-138">string</span><span class="sxs-lookup"><span data-stu-id="54be5-138">string</span></span>| <span data-ttu-id="54be5-139">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="54be5-139">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="54be5-140">riskEventType</span><span class="sxs-lookup"><span data-stu-id="54be5-140">riskEventType</span></span>|<span data-ttu-id="54be5-141">string</span><span class="sxs-lookup"><span data-stu-id="54be5-141">string</span></span>| <span data-ttu-id="54be5-142">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="54be5-142">The type of risk</span></span>|
|<span data-ttu-id="54be5-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="54be5-143">userDisplayName</span></span>|<span data-ttu-id="54be5-144">string</span><span class="sxs-lookup"><span data-stu-id="54be5-144">string</span></span>| <span data-ttu-id="54be5-145">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="54be5-145">The name of the user at risk</span></span>|
|<span data-ttu-id="54be5-146">userId</span><span class="sxs-lookup"><span data-stu-id="54be5-146">userId</span></span>|<span data-ttu-id="54be5-147">string</span><span class="sxs-lookup"><span data-stu-id="54be5-147">string</span></span>| <span data-ttu-id="54be5-148">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="54be5-148">The id of the user at risk</span></span>|
|<span data-ttu-id="54be5-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="54be5-149">userPrincipalName</span></span>|<span data-ttu-id="54be5-150">string</span><span class="sxs-lookup"><span data-stu-id="54be5-150">string</span></span>| <span data-ttu-id="54be5-151">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="54be5-151">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="54be5-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="54be5-152">Relationships</span></span>
| <span data-ttu-id="54be5-153">Beziehung</span><span class="sxs-lookup"><span data-stu-id="54be5-153">Relationship</span></span> | <span data-ttu-id="54be5-154">Typ</span><span class="sxs-lookup"><span data-stu-id="54be5-154">Type</span></span>   |<span data-ttu-id="54be5-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54be5-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54be5-156">impactedUser</span><span class="sxs-lookup"><span data-stu-id="54be5-156">impactedUser</span></span>|[<span data-ttu-id="54be5-157">Benutzer</span><span class="sxs-lookup"><span data-stu-id="54be5-157">user</span></span>](user.md)| <span data-ttu-id="54be5-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="54be5-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54be5-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54be5-160">JSON representation</span></span>

<span data-ttu-id="54be5-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54be5-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
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
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: Ressourcentyp locatedRiskEvent
description: 'Ein Risikoereignis von Azure Active Directory-Identität Protection, die auf Standortdaten basiert erkannt. Befindet sich Risikotypen werden unterstützt:'
localization_priority: Normal
ms.openlocfilehash: 20fe76099c511483144b42e33fc260910debb5ed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510260"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="119b4-104">Ressourcentyp locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="119b4-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="119b4-105">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , das auf Standortdaten erkannt.</span><span class="sxs-lookup"><span data-stu-id="119b4-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="119b4-106">Befindet sich Risikotypen werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="119b4-106">Located risk event types include:</span></span>
* [<span data-ttu-id="119b4-107">Anmeldungen von anonymen IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="119b4-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="119b4-108">Anmeldungen von Geräten Malware infiziert</span><span class="sxs-lookup"><span data-stu-id="119b4-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="119b4-109">unmöglich Reisen zu untypischen Speicherorte</span><span class="sxs-lookup"><span data-stu-id="119b4-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="119b4-110">Anmeldungen von verdächtigen IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="119b4-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="119b4-111">[Anmeldungen von unbekannten Standorten](unfamiliarlocationriskevent.md) Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="119b4-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="119b4-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="119b4-112">Methods</span></span>

| <span data-ttu-id="119b4-113">Methode</span><span class="sxs-lookup"><span data-stu-id="119b4-113">Method</span></span>           | <span data-ttu-id="119b4-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="119b4-114">Return Type</span></span>    |<span data-ttu-id="119b4-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="119b4-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="119b4-116">Abrufen von locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="119b4-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="119b4-117">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="119b4-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="119b4-118">Lesen Sie Eigenschaften und Beziehungen des LocatedRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="119b4-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="119b4-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="119b4-119">Properties</span></span>
| <span data-ttu-id="119b4-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="119b4-120">Property</span></span>     | <span data-ttu-id="119b4-121">Typ</span><span class="sxs-lookup"><span data-stu-id="119b4-121">Type</span></span>   |<span data-ttu-id="119b4-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="119b4-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="119b4-123">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="119b4-123">closedDateTime</span></span>|<span data-ttu-id="119b4-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119b4-124">dateTimeOffset</span></span>| <span data-ttu-id="119b4-125">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="119b4-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="119b4-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="119b4-126">createdDateTime</span></span>|<span data-ttu-id="119b4-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119b4-127">dateTimeOffset</span></span>| <span data-ttu-id="119b4-128">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="119b4-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="119b4-129">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="119b4-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="119b4-130">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="119b4-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="119b4-131">id</span><span class="sxs-lookup"><span data-stu-id="119b4-131">id</span></span>|<span data-ttu-id="119b4-132">string</span><span class="sxs-lookup"><span data-stu-id="119b4-132">string</span></span>| <span data-ttu-id="119b4-133">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="119b4-133">Read-only</span></span>|
|<span data-ttu-id="119b4-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="119b4-134">ipAddress</span></span>|<span data-ttu-id="119b4-135">string</span><span class="sxs-lookup"><span data-stu-id="119b4-135">string</span></span>| <span data-ttu-id="119b4-136">Die IP-Adresse von der Anmeldung</span><span class="sxs-lookup"><span data-stu-id="119b4-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="119b4-137">location</span><span class="sxs-lookup"><span data-stu-id="119b4-137">location</span></span>|<span data-ttu-id="119b4-138">string</span><span class="sxs-lookup"><span data-stu-id="119b4-138">string</span></span>| <span data-ttu-id="119b4-139">Die Position, die IP-Adresse von der Anmeldung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="119b4-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="119b4-140">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="119b4-140">riskEventDateTime</span></span>|<span data-ttu-id="119b4-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="119b4-141">dateTimeOffset</span></span>| <span data-ttu-id="119b4-142">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="119b4-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="119b4-143">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="119b4-143">riskEventStatus</span></span>|<span data-ttu-id="119b4-144">string</span><span class="sxs-lookup"><span data-stu-id="119b4-144">string</span></span>| <span data-ttu-id="119b4-145">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="119b4-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="119b4-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="119b4-146">riskLevel</span></span>|<span data-ttu-id="119b4-147">string</span><span class="sxs-lookup"><span data-stu-id="119b4-147">string</span></span>| <span data-ttu-id="119b4-148">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="119b4-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="119b4-149">riskEventType</span><span class="sxs-lookup"><span data-stu-id="119b4-149">riskEventType</span></span>|<span data-ttu-id="119b4-150">string</span><span class="sxs-lookup"><span data-stu-id="119b4-150">string</span></span>| <span data-ttu-id="119b4-151">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="119b4-151">The type of risk</span></span>|
|<span data-ttu-id="119b4-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="119b4-152">userDisplayName</span></span>|<span data-ttu-id="119b4-153">string</span><span class="sxs-lookup"><span data-stu-id="119b4-153">string</span></span>| <span data-ttu-id="119b4-154">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="119b4-154">The name of the user at risk</span></span>|
|<span data-ttu-id="119b4-155">userId</span><span class="sxs-lookup"><span data-stu-id="119b4-155">userId</span></span>|<span data-ttu-id="119b4-156">string</span><span class="sxs-lookup"><span data-stu-id="119b4-156">string</span></span>| <span data-ttu-id="119b4-157">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="119b4-157">The id of the user at risk</span></span>|
|<span data-ttu-id="119b4-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="119b4-158">userPrincipalName</span></span>|<span data-ttu-id="119b4-159">string</span><span class="sxs-lookup"><span data-stu-id="119b4-159">string</span></span>| <span data-ttu-id="119b4-160">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="119b4-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="119b4-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="119b4-161">Relationships</span></span>
| <span data-ttu-id="119b4-162">Beziehung</span><span class="sxs-lookup"><span data-stu-id="119b4-162">Relationship</span></span> | <span data-ttu-id="119b4-163">Typ</span><span class="sxs-lookup"><span data-stu-id="119b4-163">Type</span></span>   |<span data-ttu-id="119b4-164">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="119b4-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="119b4-165">impactedUser</span><span class="sxs-lookup"><span data-stu-id="119b4-165">impactedUser</span></span>|[<span data-ttu-id="119b4-166">user</span><span class="sxs-lookup"><span data-stu-id="119b4-166">user</span></span>](user.md)| <span data-ttu-id="119b4-p104">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="119b4-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="119b4-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="119b4-169">JSON representation</span></span>

<span data-ttu-id="119b4-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="119b4-170">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locatedriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: Ressourcentyp unfamiliarLocationRiskEvent
description: Ein Risikoereignis von Azure Active Directory-Identität Protection ein Konto anmelden, in dem versucht wird, von einem neuen Speicherort für diesen Benutzer erkannt. Umfassende Informationen zum Risiko-Ereignissen finden Sie in der Dokumentation zu Azure AD-Schutz.
localization_priority: Normal
ms.openlocfilehash: adad214c0ac58540f1115b836c2c5f26faa6c031
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507978"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="662dc-104">Ressourcentyp unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="662dc-104">unfamiliarLocationRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="662dc-105">Ein Risikoereignis von [Azure Active Directory-Identität Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) ein Konto anmelden, in dem versucht wird, von einem neuen Speicherort für diesen Benutzer erkannt.</span><span class="sxs-lookup"><span data-stu-id="662dc-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="662dc-106">Umfassende Informationen zum Risikoereignisse finden Sie in der [Dokumentation von Azure AD-Schutz](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="662dc-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="662dc-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="662dc-107">Methods</span></span>

| <span data-ttu-id="662dc-108">Methode</span><span class="sxs-lookup"><span data-stu-id="662dc-108">Method</span></span>           | <span data-ttu-id="662dc-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="662dc-109">Return Type</span></span>    |<span data-ttu-id="662dc-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="662dc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="662dc-111">Abrufen von unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="662dc-111">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="662dc-112">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="662dc-112">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="662dc-113">Lesen Sie Eigenschaften und Beziehungen des UnfamiliarLocationRiskEvent-Objekts.</span><span class="sxs-lookup"><span data-stu-id="662dc-113">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="662dc-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="662dc-114">Properties</span></span>
| <span data-ttu-id="662dc-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="662dc-115">Property</span></span>     | <span data-ttu-id="662dc-116">Typ</span><span class="sxs-lookup"><span data-stu-id="662dc-116">Type</span></span>   |<span data-ttu-id="662dc-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="662dc-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="662dc-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="662dc-118">closedDateTime</span></span>|<span data-ttu-id="662dc-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="662dc-119">dateTimeOffset</span></span>| <span data-ttu-id="662dc-120">Datum und Uhrzeit, die das Risikoereignis geschlossen wurde</span><span class="sxs-lookup"><span data-stu-id="662dc-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="662dc-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="662dc-121">createdDateTime</span></span>|<span data-ttu-id="662dc-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="662dc-122">dateTimeOffset</span></span>| <span data-ttu-id="662dc-123">Das Datum und die Uhrzeit, die das Risikoereignis erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="662dc-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="662dc-124">Dies ist immer größer als oder gleich dem Datetime des Ereignisses Risiko selbst.</span><span class="sxs-lookup"><span data-stu-id="662dc-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="662dc-125">Dies ist die entsprechende Eigenschaft eines Filters beim Risikoereignisse Abfragen verwendet.</span><span class="sxs-lookup"><span data-stu-id="662dc-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="662dc-126">id</span><span class="sxs-lookup"><span data-stu-id="662dc-126">id</span></span>|<span data-ttu-id="662dc-127">string</span><span class="sxs-lookup"><span data-stu-id="662dc-127">string</span></span>| <span data-ttu-id="662dc-128">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="662dc-128">Read-only</span></span>|
|<span data-ttu-id="662dc-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="662dc-129">ipAddress</span></span>|<span data-ttu-id="662dc-130">string</span><span class="sxs-lookup"><span data-stu-id="662dc-130">string</span></span>| <span data-ttu-id="662dc-131">Die IP-Adresse von der Anmeldung</span><span class="sxs-lookup"><span data-stu-id="662dc-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="662dc-132">location</span><span class="sxs-lookup"><span data-stu-id="662dc-132">location</span></span>|<span data-ttu-id="662dc-133">string</span><span class="sxs-lookup"><span data-stu-id="662dc-133">string</span></span>| <span data-ttu-id="662dc-134">Die Position, die IP-Adresse von der Anmeldung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="662dc-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="662dc-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="662dc-135">riskEventDateTime</span></span>|<span data-ttu-id="662dc-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="662dc-136">dateTimeOffset</span></span>| <span data-ttu-id="662dc-137">Datum und Uhrzeit, wann das Risikoereignis aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="662dc-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="662dc-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="662dc-138">riskEventStatus</span></span>|<span data-ttu-id="662dc-139">string</span><span class="sxs-lookup"><span data-stu-id="662dc-139">string</span></span>| <span data-ttu-id="662dc-140">Mögliche Werte sind: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto` und `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="662dc-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="662dc-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="662dc-141">riskLevel</span></span>|<span data-ttu-id="662dc-142">string</span><span class="sxs-lookup"><span data-stu-id="662dc-142">string</span></span>| <span data-ttu-id="662dc-143">Mögliche Werte sind: `low`, `medium` und `high`.</span><span class="sxs-lookup"><span data-stu-id="662dc-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="662dc-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="662dc-144">riskEventType</span></span>|<span data-ttu-id="662dc-145">string</span><span class="sxs-lookup"><span data-stu-id="662dc-145">string</span></span>| <span data-ttu-id="662dc-146">Der Typ des Risikos</span><span class="sxs-lookup"><span data-stu-id="662dc-146">The type of risk</span></span>|
|<span data-ttu-id="662dc-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="662dc-147">userDisplayName</span></span>|<span data-ttu-id="662dc-148">string</span><span class="sxs-lookup"><span data-stu-id="662dc-148">string</span></span>| <span data-ttu-id="662dc-149">Der Name des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="662dc-149">The name of the user at risk</span></span>|
|<span data-ttu-id="662dc-150">userId</span><span class="sxs-lookup"><span data-stu-id="662dc-150">userId</span></span>|<span data-ttu-id="662dc-151">string</span><span class="sxs-lookup"><span data-stu-id="662dc-151">string</span></span>| <span data-ttu-id="662dc-152">Die Id des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="662dc-152">The id of the user at risk</span></span>|
|<span data-ttu-id="662dc-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="662dc-153">userPrincipalName</span></span>|<span data-ttu-id="662dc-154">string</span><span class="sxs-lookup"><span data-stu-id="662dc-154">string</span></span>| <span data-ttu-id="662dc-155">Der Benutzerprinzipalname des Benutzers gefährdet</span><span class="sxs-lookup"><span data-stu-id="662dc-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="662dc-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="662dc-156">Relationships</span></span>
| <span data-ttu-id="662dc-157">Beziehung</span><span class="sxs-lookup"><span data-stu-id="662dc-157">Relationship</span></span> | <span data-ttu-id="662dc-158">Typ</span><span class="sxs-lookup"><span data-stu-id="662dc-158">Type</span></span>   |<span data-ttu-id="662dc-159">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="662dc-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="662dc-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="662dc-160">impactedUser</span></span>|[<span data-ttu-id="662dc-161">user</span><span class="sxs-lookup"><span data-stu-id="662dc-161">user</span></span>](user.md)| <span data-ttu-id="662dc-p104">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="662dc-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="662dc-164">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="662dc-164">JSON representation</span></span>

<span data-ttu-id="662dc-165">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="662dc-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
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
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/unfamiliarlocationriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

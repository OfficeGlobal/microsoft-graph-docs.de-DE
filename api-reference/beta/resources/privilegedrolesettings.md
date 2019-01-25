---
title: Ressourcentyp privilegedRoleSettings
description: Stellt die Einstellungen für eine privilegierten Rolle.
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525696"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="76f76-103">Ressourcentyp privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="76f76-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76f76-104">Stellt die Einstellungen für eine privilegierten Rolle.</span><span class="sxs-lookup"><span data-stu-id="76f76-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="76f76-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="76f76-105">Methods</span></span>

| <span data-ttu-id="76f76-106">Methode</span><span class="sxs-lookup"><span data-stu-id="76f76-106">Method</span></span>           | <span data-ttu-id="76f76-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="76f76-107">Return Type</span></span>    |<span data-ttu-id="76f76-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76f76-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="76f76-109">Abrufen von privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="76f76-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="76f76-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="76f76-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="76f76-111">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSettings-Objekts.</span><span class="sxs-lookup"><span data-stu-id="76f76-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="76f76-112">PrivilegedRoleSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="76f76-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="76f76-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="76f76-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="76f76-114">PrivilegedRoleSettings-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="76f76-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="76f76-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="76f76-115">Properties</span></span>
| <span data-ttu-id="76f76-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76f76-116">Property</span></span>     | <span data-ttu-id="76f76-117">Typ</span><span class="sxs-lookup"><span data-stu-id="76f76-117">Type</span></span>   |<span data-ttu-id="76f76-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76f76-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76f76-119">ElevationDuration</span><span class="sxs-lookup"><span data-stu-id="76f76-119">elevationDuration</span></span>|<span data-ttu-id="76f76-120">duration</span><span class="sxs-lookup"><span data-stu-id="76f76-120">duration</span></span>|<span data-ttu-id="76f76-121">Die Dauer, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="76f76-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="76f76-122">id</span><span class="sxs-lookup"><span data-stu-id="76f76-122">id</span></span>|<span data-ttu-id="76f76-123">string</span><span class="sxs-lookup"><span data-stu-id="76f76-123">string</span></span>| <span data-ttu-id="76f76-124">Der eindeutige Bezeichner für die rolleneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="76f76-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="76f76-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="76f76-125">Read-only.</span></span>|
|<span data-ttu-id="76f76-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="76f76-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="76f76-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="76f76-127">boolean</span></span>|<span data-ttu-id="76f76-128">**true,** Wenn MfaOnElevation konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="76f76-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="76f76-129">**false,** Wenn MfaOnElevation nicht konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="76f76-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="76f76-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="76f76-130">lastGlobalAdmin</span></span>|<span data-ttu-id="76f76-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="76f76-131">boolean</span></span>|<span data-ttu-id="76f76-132">Verwendet nur intern.</span><span class="sxs-lookup"><span data-stu-id="76f76-132">Internal used only.</span></span>|
|<span data-ttu-id="76f76-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="76f76-133">maxElavationDuration</span></span>|<span data-ttu-id="76f76-134">duration</span><span class="sxs-lookup"><span data-stu-id="76f76-134">duration</span></span>|<span data-ttu-id="76f76-135">Maximale Dauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="76f76-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="76f76-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="76f76-136">mfaOnElevation</span></span>|<span data-ttu-id="76f76-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="76f76-137">boolean</span></span>|<span data-ttu-id="76f76-138">**true,** Wenn mehrstufiger Authentifizierung das erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76f76-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="76f76-139">**false,** Wenn mehrstufiger Authentifizierung das nicht erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76f76-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="76f76-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="76f76-140">minElevationDuration</span></span>|<span data-ttu-id="76f76-141">duration</span><span class="sxs-lookup"><span data-stu-id="76f76-141">duration</span></span>|<span data-ttu-id="76f76-142">Minimale Dauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="76f76-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="76f76-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="76f76-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="76f76-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="76f76-144">boolean</span></span>|<span data-ttu-id="76f76-145">**true,** Wenn für den Endbenutzer Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="76f76-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="76f76-146">**false,** Wenn keine Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="76f76-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="76f76-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="76f76-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="76f76-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="76f76-148">boolean</span></span>|<span data-ttu-id="76f76-149">**true,** Wenn die Informationen zur erforderlichen wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76f76-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="76f76-150">**false,** Wenn die Informationen zur nicht erforderlich bei ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76f76-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="76f76-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="76f76-151">approvalOnElevation</span></span>|<span data-ttu-id="76f76-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="76f76-152">boolean</span></span>|<span data-ttu-id="76f76-153">**true,** Wenn die Genehmigung erforderlich wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76f76-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="76f76-154">**false,** Wenn die Genehmigung ist nicht erforderlich bei die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="76f76-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="76f76-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="76f76-155">approverIds</span></span>|<span data-ttu-id="76f76-156">Array</span><span class="sxs-lookup"><span data-stu-id="76f76-156">array</span></span>|<span data-ttu-id="76f76-157">Liste der Genehmigung-Ids, wenn die Genehmigung für die Aktivierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="76f76-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76f76-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="76f76-158">Relationships</span></span>
<span data-ttu-id="76f76-159">Keine</span><span class="sxs-lookup"><span data-stu-id="76f76-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="76f76-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="76f76-160">JSON representation</span></span>

<span data-ttu-id="76f76-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="76f76-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

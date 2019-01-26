---
title: Ressourcentyp privilegedRoleSettings
description: Stellt die Einstellungen für eine privilegierten Rolle.
localization_priority: Normal
ms.openlocfilehash: 673327e3c83a4111eb469ca48550836433dbdf0a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577151"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="786ed-103">Ressourcentyp privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="786ed-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="786ed-104">Stellt die Einstellungen für eine privilegierten Rolle.</span><span class="sxs-lookup"><span data-stu-id="786ed-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="786ed-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="786ed-105">Methods</span></span>

| <span data-ttu-id="786ed-106">Methode</span><span class="sxs-lookup"><span data-stu-id="786ed-106">Method</span></span>           | <span data-ttu-id="786ed-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="786ed-107">Return Type</span></span>    |<span data-ttu-id="786ed-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="786ed-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="786ed-109">Abrufen von privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="786ed-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="786ed-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="786ed-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="786ed-111">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSettings-Objekts.</span><span class="sxs-lookup"><span data-stu-id="786ed-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="786ed-112">PrivilegedRoleSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="786ed-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="786ed-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="786ed-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="786ed-114">PrivilegedRoleSettings-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="786ed-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="786ed-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="786ed-115">Properties</span></span>
| <span data-ttu-id="786ed-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="786ed-116">Property</span></span>     | <span data-ttu-id="786ed-117">Typ</span><span class="sxs-lookup"><span data-stu-id="786ed-117">Type</span></span>   |<span data-ttu-id="786ed-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="786ed-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="786ed-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="786ed-119">elevationDuration</span></span>| <span data-ttu-id="786ed-120">Zeichenfolge (Zeitstempel)</span><span class="sxs-lookup"><span data-stu-id="786ed-120">String (timestamp)</span></span> |<span data-ttu-id="786ed-121">Die Dauer, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="786ed-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="786ed-122">id</span><span class="sxs-lookup"><span data-stu-id="786ed-122">id</span></span>| <span data-ttu-id="786ed-123">Zeichenfolge (ID)</span><span class="sxs-lookup"><span data-stu-id="786ed-123">string (identifier)</span></span>| <span data-ttu-id="786ed-124">Der eindeutige Bezeichner für die rolleneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="786ed-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="786ed-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="786ed-125">Read-only.</span></span>|
|<span data-ttu-id="786ed-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="786ed-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="786ed-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="786ed-127">boolean</span></span>|<span data-ttu-id="786ed-128">**true,** Wenn MfaOnElevation konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="786ed-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="786ed-129">**false,** Wenn MfaOnElevation nicht konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="786ed-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="786ed-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="786ed-130">lastGlobalAdmin</span></span>|<span data-ttu-id="786ed-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="786ed-131">boolean</span></span>|<span data-ttu-id="786ed-132">Verwendet nur intern.</span><span class="sxs-lookup"><span data-stu-id="786ed-132">Internal used only.</span></span>|
|<span data-ttu-id="786ed-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="786ed-133">maxElavationDuration</span></span>| <span data-ttu-id="786ed-134">Zeichenfolge (ID)</span><span class="sxs-lookup"><span data-stu-id="786ed-134">string (identifier)</span></span>| |<span data-ttu-id="786ed-135">Maximale Dauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="786ed-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="786ed-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="786ed-136">mfaOnElevation</span></span>|<span data-ttu-id="786ed-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="786ed-137">boolean</span></span>|<span data-ttu-id="786ed-138">**true,** Wenn mehrstufiger Authentifizierung das erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="786ed-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="786ed-139">**false,** Wenn mehrstufiger Authentifizierung das nicht erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="786ed-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="786ed-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="786ed-140">minElevationDuration</span></span>|<span data-ttu-id="786ed-141">Zeichenfolge (ID)</span><span class="sxs-lookup"><span data-stu-id="786ed-141">string (identifier)</span></span>||<span data-ttu-id="786ed-142">Minimale Dauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="786ed-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="786ed-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="786ed-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="786ed-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="786ed-144">boolean</span></span>|<span data-ttu-id="786ed-145">**true,** Wenn für den Endbenutzer Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="786ed-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="786ed-146">**false,** Wenn keine Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="786ed-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="786ed-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="786ed-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="786ed-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="786ed-148">boolean</span></span>|<span data-ttu-id="786ed-149">**true,** Wenn die Informationen zur erforderlichen wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="786ed-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="786ed-150">**false,** Wenn die Informationen zur nicht erforderlich bei ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="786ed-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="786ed-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="786ed-151">approvalOnElevation</span></span>|<span data-ttu-id="786ed-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="786ed-152">boolean</span></span>|<span data-ttu-id="786ed-153">**true,** Wenn die Genehmigung erforderlich wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="786ed-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="786ed-154">**false,** Wenn die Genehmigung ist nicht erforderlich bei die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="786ed-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="786ed-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="786ed-155">approverIds</span></span>| <span data-ttu-id="786ed-156">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="786ed-156">String collection</span></span> |<span data-ttu-id="786ed-157">Liste der Genehmigung-Ids, wenn die Genehmigung für die Aktivierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="786ed-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="786ed-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="786ed-158">Relationships</span></span>
<span data-ttu-id="786ed-159">Keine</span><span class="sxs-lookup"><span data-stu-id="786ed-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="786ed-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="786ed-160">JSON representation</span></span>

<span data-ttu-id="786ed-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="786ed-161">Here is a JSON representation of the resource.</span></span>

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
  "approverIds": [ "String (identifier)" ]
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

---
title: Ressourcentyp privilegedRoleSettings
description: Stellt die Einstellungen für eine privilegierten Rolle.
localization_priority: Normal
ms.openlocfilehash: 971c48ce3ecdd2a219a111f3a11884377e20430c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842742"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="8f192-103">Ressourcentyp privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8f192-103">privilegedRoleSettings resource type</span></span>

> <span data-ttu-id="8f192-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8f192-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f192-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f192-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f192-106">Stellt die Einstellungen für eine privilegierten Rolle.</span><span class="sxs-lookup"><span data-stu-id="8f192-106">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="8f192-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8f192-107">Methods</span></span>

| <span data-ttu-id="8f192-108">Methode</span><span class="sxs-lookup"><span data-stu-id="8f192-108">Method</span></span>           | <span data-ttu-id="8f192-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8f192-109">Return Type</span></span>    |<span data-ttu-id="8f192-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f192-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f192-111">Abrufen von privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8f192-111">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="8f192-112">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8f192-112">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="8f192-113">Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSettings-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f192-113">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="8f192-114">PrivilegedRoleSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8f192-114">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="8f192-115">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8f192-115">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="8f192-116">PrivilegedRoleSettings-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="8f192-116">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="8f192-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f192-117">Properties</span></span>
| <span data-ttu-id="8f192-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f192-118">Property</span></span>     | <span data-ttu-id="8f192-119">Typ</span><span class="sxs-lookup"><span data-stu-id="8f192-119">Type</span></span>   |<span data-ttu-id="8f192-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f192-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f192-121">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="8f192-121">elevationDuration</span></span>|<span data-ttu-id="8f192-122">duration</span><span class="sxs-lookup"><span data-stu-id="8f192-122">duration</span></span>|<span data-ttu-id="8f192-123">Die Dauer, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="8f192-123">The duration when the role is activated.</span></span>|
|<span data-ttu-id="8f192-124">id</span><span class="sxs-lookup"><span data-stu-id="8f192-124">id</span></span>|<span data-ttu-id="8f192-125">string</span><span class="sxs-lookup"><span data-stu-id="8f192-125">string</span></span>| <span data-ttu-id="8f192-126">Der eindeutige Bezeichner für die rolleneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="8f192-126">The unique identifier for the role settings.</span></span> <span data-ttu-id="8f192-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8f192-127">Read-only.</span></span>|
|<span data-ttu-id="8f192-128">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="8f192-128">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="8f192-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f192-129">boolean</span></span>|<span data-ttu-id="8f192-130">**true,** Wenn MfaOnElevation konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="8f192-130">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="8f192-131">**false,** Wenn MfaOnElevation nicht konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="8f192-131">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="8f192-132">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="8f192-132">lastGlobalAdmin</span></span>|<span data-ttu-id="8f192-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f192-133">boolean</span></span>|<span data-ttu-id="8f192-134">Verwendet nur intern.</span><span class="sxs-lookup"><span data-stu-id="8f192-134">Internal used only.</span></span>|
|<span data-ttu-id="8f192-135">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="8f192-135">maxElavationDuration</span></span>|<span data-ttu-id="8f192-136">duration</span><span class="sxs-lookup"><span data-stu-id="8f192-136">duration</span></span>|<span data-ttu-id="8f192-137">Maximale Dauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="8f192-137">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="8f192-138">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="8f192-138">mfaOnElevation</span></span>|<span data-ttu-id="8f192-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f192-139">boolean</span></span>|<span data-ttu-id="8f192-140">**true,** Wenn mehrstufiger Authentifizierung das erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="8f192-140">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="8f192-141">**false,** Wenn mehrstufiger Authentifizierung das nicht erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="8f192-141">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="8f192-142">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="8f192-142">minElevationDuration</span></span>|<span data-ttu-id="8f192-143">duration</span><span class="sxs-lookup"><span data-stu-id="8f192-143">duration</span></span>|<span data-ttu-id="8f192-144">Minimale Dauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="8f192-144">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="8f192-145">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="8f192-145">notificationToUserOnElevation</span></span>|<span data-ttu-id="8f192-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f192-146">boolean</span></span>|<span data-ttu-id="8f192-147">**true,** Wenn für den Endbenutzer Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="8f192-147">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="8f192-148">**false,** Wenn keine Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="8f192-148">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="8f192-149">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="8f192-149">ticketingInfoOnElevation</span></span>|<span data-ttu-id="8f192-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f192-150">boolean</span></span>|<span data-ttu-id="8f192-151">**true,** Wenn die Informationen zur erforderlichen wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="8f192-151">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="8f192-152">**false,** Wenn die Informationen zur nicht erforderlich bei ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="8f192-152">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="8f192-153">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="8f192-153">approvalOnElevation</span></span>|<span data-ttu-id="8f192-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f192-154">boolean</span></span>|<span data-ttu-id="8f192-155">**true,** Wenn die Genehmigung erforderlich wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="8f192-155">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="8f192-156">**false,** Wenn die Genehmigung ist nicht erforderlich bei die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="8f192-156">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="8f192-157">approverIds</span><span class="sxs-lookup"><span data-stu-id="8f192-157">approverIds</span></span>|<span data-ttu-id="8f192-158">Array</span><span class="sxs-lookup"><span data-stu-id="8f192-158">array</span></span>|<span data-ttu-id="8f192-159">Liste der Genehmigung-Ids, wenn die Genehmigung für die Aktivierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8f192-159">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f192-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f192-160">Relationships</span></span>
<span data-ttu-id="8f192-161">Keine</span><span class="sxs-lookup"><span data-stu-id="8f192-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f192-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f192-162">JSON representation</span></span>

<span data-ttu-id="8f192-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f192-163">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

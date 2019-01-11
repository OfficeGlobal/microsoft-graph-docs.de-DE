---
title: groupLifecyclePolicy-Ressourcentyp
description: Steht für eine Lebenszyklusrichtlinie für eine Office 365-Gruppe. Eine Lebenszyklusrichtlinie für eine Gruppe ermöglicht Administratoren das Festlegen eines Ablaufzeitraums für Gruppen. Zum Beispiel nach 180 Tagen läuft eine Gruppe ab. Wenn eine Gruppe den Ablaufzeitpunkt erreicht, müssen Besitzer der Gruppe die Gruppe in einem vom Administrator definierten Zeitintervall verlängern. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind. Der neue Ablaufzeitraum für die Gruppe lautet dann beispielsweise 180 Tage ab Verlängerung. Wenn die Gruppe nicht verlängert wird, läuft sie ab und wird gelöscht. Die Gruppe kann innerhalb von 30 Tagen nach Löschung wiederhergestellt werden.
localization_priority: Normal
ms.openlocfilehash: 271a3421599eaa58487cc7917c8dfaf4c382050d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861684"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="aab69-110">groupLifecyclePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aab69-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="aab69-111">Steht für eine Lebenszyklusrichtlinie für eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="aab69-111">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="aab69-112">Eine Lebenszyklusrichtlinie für eine Gruppe ermöglicht Administratoren das Festlegen eines Ablaufzeitraums für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="aab69-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="aab69-113">Zum Beispiel nach 180 Tagen läuft eine Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="aab69-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="aab69-114">Wenn eine Gruppe den Ablaufzeitpunkt erreicht, müssen Besitzer der Gruppe die Gruppe in einem vom Administrator definierten Zeitintervall verlängern.</span><span class="sxs-lookup"><span data-stu-id="aab69-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="aab69-115">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.</span><span class="sxs-lookup"><span data-stu-id="aab69-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="aab69-116">Der neue Ablaufzeitraum für die Gruppe lautet dann beispielsweise 180 Tage ab Verlängerung.</span><span class="sxs-lookup"><span data-stu-id="aab69-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="aab69-117">Wenn die Gruppe nicht verlängert wird, läuft sie ab und wird gelöscht.</span><span class="sxs-lookup"><span data-stu-id="aab69-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="aab69-118">Die Gruppe kann innerhalb von 30 Tagen nach Löschung wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="aab69-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="aab69-119">Methoden</span><span class="sxs-lookup"><span data-stu-id="aab69-119">Methods</span></span>

| <span data-ttu-id="aab69-120">Methode</span><span class="sxs-lookup"><span data-stu-id="aab69-120">Method</span></span> | <span data-ttu-id="aab69-121">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aab69-121">Return Type</span></span> | <span data-ttu-id="aab69-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aab69-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="aab69-123">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="aab69-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="aab69-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="aab69-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="aab69-125">Dient zum Lesen der Eigenschaften und der Beziehungen eines groupLifecyclePolicy-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aab69-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="aab69-126">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="aab69-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="aab69-127">[groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aab69-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="aab69-128">Listet alle groupLifecyclePolicies auf.</span><span class="sxs-lookup"><span data-stu-id="aab69-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="aab69-129">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="aab69-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="aab69-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="aab69-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="aab69-131">Aktualisiert ein groupLifecyclePolicy-Objekt.</span><span class="sxs-lookup"><span data-stu-id="aab69-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="aab69-132">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="aab69-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="aab69-133">Keine</span><span class="sxs-lookup"><span data-stu-id="aab69-133">None</span></span> | <span data-ttu-id="aab69-134">Löscht ein groupLifecyclePolicy-Objekt.</span><span class="sxs-lookup"><span data-stu-id="aab69-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="aab69-135">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="aab69-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="aab69-136">Keine</span><span class="sxs-lookup"><span data-stu-id="aab69-136">None</span></span>| <span data-ttu-id="aab69-137">Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.</span><span class="sxs-lookup"><span data-stu-id="aab69-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="aab69-138">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="aab69-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="aab69-139">Keine</span><span class="sxs-lookup"><span data-stu-id="aab69-139">None</span></span>| <span data-ttu-id="aab69-140">Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="aab69-140">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="aab69-141">Erneuern einer Gruppe</span><span class="sxs-lookup"><span data-stu-id="aab69-141">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="aab69-142">Keine</span><span class="sxs-lookup"><span data-stu-id="aab69-142">None</span></span>| <span data-ttu-id="aab69-143">Erneuern einer Gruppe Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="aab69-143">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="aab69-144">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aab69-144">Properties</span></span>

| <span data-ttu-id="aab69-145">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aab69-145">Property</span></span> | <span data-ttu-id="aab69-146">Typ</span><span class="sxs-lookup"><span data-stu-id="aab69-146">Type</span></span> | <span data-ttu-id="aab69-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aab69-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aab69-148">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="aab69-148">alternateNotificationEmails</span></span>|<span data-ttu-id="aab69-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aab69-149">String</span></span>| <span data-ttu-id="aab69-150">Liste der E-Mail-Adressen, an die Benachrichtigungen für Gruppen ohne Besitzer gesendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="aab69-150">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="aab69-151">Mehrere E-Mail-Adressen können durch ein Semikolon voneinander getrennt definiert werden.</span><span class="sxs-lookup"><span data-stu-id="aab69-151">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="aab69-152">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="aab69-152">groupLifetimeInDays</span></span>|<span data-ttu-id="aab69-153">Int32</span><span class="sxs-lookup"><span data-stu-id="aab69-153">Int32</span></span>| <span data-ttu-id="aab69-154">Anzahl von Tagen, bis eine Gruppe abläuft und verlängert werden muss.</span><span class="sxs-lookup"><span data-stu-id="aab69-154">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="aab69-155">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der definierten Tage verlängert.</span><span class="sxs-lookup"><span data-stu-id="aab69-155">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="aab69-156">id</span><span class="sxs-lookup"><span data-stu-id="aab69-156">id</span></span>|<span data-ttu-id="aab69-157">Guid</span><span class="sxs-lookup"><span data-stu-id="aab69-157">Guid</span></span>| <span data-ttu-id="aab69-158">Ein eindeutiger Bezeichner für eine Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="aab69-158">A unique identifier for a policy.</span></span> <span data-ttu-id="aab69-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="aab69-159">Read-only.</span></span>|
|<span data-ttu-id="aab69-160">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="aab69-160">managedGroupTypes</span></span>|<span data-ttu-id="aab69-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aab69-161">String</span></span>| <span data-ttu-id="aab69-162">Der Gruppentyp, für den die Ablaufrichtlinie gilt.</span><span class="sxs-lookup"><span data-stu-id="aab69-162">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="aab69-163">Mögliche Werte sind **Alle**, **Ausgewählte** oder **Keine**.</span><span class="sxs-lookup"><span data-stu-id="aab69-163">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="aab69-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aab69-164">Relationships</span></span>

<span data-ttu-id="aab69-165">Keine.</span><span class="sxs-lookup"><span data-stu-id="aab69-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aab69-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aab69-166">JSON representation</span></span>

<span data-ttu-id="aab69-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aab69-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

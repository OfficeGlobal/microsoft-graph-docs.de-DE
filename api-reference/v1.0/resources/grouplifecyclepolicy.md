# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="289a2-101">groupLifecyclePolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="289a2-101">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="289a2-102">Steht für eine Lebenszyklusrichtlinie für eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="289a2-102">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="289a2-103">Eine Lebenszyklusrichtlinie für eine Gruppe ermöglicht Administratoren das Festlegen eines Ablaufzeitraums für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="289a2-103">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="289a2-104">Zum Beispiel nach 180 Tagen läuft eine Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="289a2-104">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="289a2-105">Wenn eine Gruppe den Ablaufzeitpunkt erreicht, müssen Besitzer der Gruppe die Gruppe in einem vom Administrator definierten Zeitintervall verlängern.</span><span class="sxs-lookup"><span data-stu-id="289a2-105">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="289a2-106">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind.</span><span class="sxs-lookup"><span data-stu-id="289a2-106">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="289a2-107">Der neue Ablaufzeitraum für die Gruppe lautet dann beispielsweise 180 Tage ab Verlängerung.</span><span class="sxs-lookup"><span data-stu-id="289a2-107">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="289a2-108">Wenn die Gruppe nicht verlängert wird, läuft sie ab und wird gelöscht.</span><span class="sxs-lookup"><span data-stu-id="289a2-108">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="289a2-109">Die Gruppe kann innerhalb von 30 Tagen nach Löschung wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="289a2-109">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="289a2-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="289a2-110">Methods</span></span>

| <span data-ttu-id="289a2-111">Methode</span><span class="sxs-lookup"><span data-stu-id="289a2-111">Method</span></span> | <span data-ttu-id="289a2-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="289a2-112">Return Type</span></span> | <span data-ttu-id="289a2-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="289a2-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="289a2-114">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="289a2-114">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_get.md) | [<span data-ttu-id="289a2-115">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="289a2-115">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="289a2-116">Dient zum Lesen der Eigenschaften und der Beziehungen eines groupLifecyclePolicy-Objekts.</span><span class="sxs-lookup"><span data-stu-id="289a2-116">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="289a2-117">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="289a2-117">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy_list.md) | <span data-ttu-id="289a2-118">[groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="289a2-118">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="289a2-119">Listet alle groupLifecyclePolicies auf.</span><span class="sxs-lookup"><span data-stu-id="289a2-119">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="289a2-120">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="289a2-120">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_update.md) | [<span data-ttu-id="289a2-121">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="289a2-121">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="289a2-122">Aktualisiert ein groupLifecyclePolicy-Objekt.</span><span class="sxs-lookup"><span data-stu-id="289a2-122">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="289a2-123">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="289a2-123">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_delete.md) | <span data-ttu-id="289a2-124">Keine</span><span class="sxs-lookup"><span data-stu-id="289a2-124">None</span></span> | <span data-ttu-id="289a2-125">Löscht ein groupLifecyclePolicy-Objekt.</span><span class="sxs-lookup"><span data-stu-id="289a2-125">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="289a2-126">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="289a2-126">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_addgroup.md)|<span data-ttu-id="289a2-127">Keine</span><span class="sxs-lookup"><span data-stu-id="289a2-127">None</span></span>| <span data-ttu-id="289a2-128">Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.</span><span class="sxs-lookup"><span data-stu-id="289a2-128">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="289a2-129">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="289a2-129">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_removegroup.md)|<span data-ttu-id="289a2-130">Keine</span><span class="sxs-lookup"><span data-stu-id="289a2-130">None</span></span>| <span data-ttu-id="289a2-131">Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="289a2-131">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="289a2-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="289a2-132">Properties</span></span>

| <span data-ttu-id="289a2-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="289a2-133">Property</span></span> | <span data-ttu-id="289a2-134">Typ</span><span class="sxs-lookup"><span data-stu-id="289a2-134">Type</span></span> | <span data-ttu-id="289a2-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="289a2-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="289a2-136">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="289a2-136">alternateNotificationEmails</span></span>|<span data-ttu-id="289a2-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="289a2-137">String</span></span>| <span data-ttu-id="289a2-138">Liste der E-Mail-Adressen, an die Benachrichtigungen für Gruppen ohne Besitzer gesendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="289a2-138">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="289a2-139">Mehrere E-Mail-Adressen können durch ein Semikolon voneinander getrennt definiert werden.</span><span class="sxs-lookup"><span data-stu-id="289a2-139">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="289a2-140">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="289a2-140">groupLifetimeInDays</span></span>|<span data-ttu-id="289a2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="289a2-141">Int32</span></span>| <span data-ttu-id="289a2-142">Anzahl von Tagen, bis eine Gruppe abläuft und verlängert werden muss.</span><span class="sxs-lookup"><span data-stu-id="289a2-142">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="289a2-143">Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der definierten Tage verlängert.</span><span class="sxs-lookup"><span data-stu-id="289a2-143">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="289a2-144">id</span><span class="sxs-lookup"><span data-stu-id="289a2-144">id</span></span>|<span data-ttu-id="289a2-145">Guid</span><span class="sxs-lookup"><span data-stu-id="289a2-145">Guid</span></span>| <span data-ttu-id="289a2-146">Ein eindeutiger Bezeichner für eine Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="289a2-146">A unique identifier for a policy.</span></span> <span data-ttu-id="289a2-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="289a2-147">Read-only.</span></span>|
|<span data-ttu-id="289a2-148">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="289a2-148">managedGroupTypes</span></span>|<span data-ttu-id="289a2-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="289a2-149">String</span></span>| <span data-ttu-id="289a2-150">Der Gruppentyp, für den die Ablaufrichtlinie gilt.</span><span class="sxs-lookup"><span data-stu-id="289a2-150">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="289a2-151">Mögliche Werte sind **Alle**, **Ausgewählte** oder **Keine**.</span><span class="sxs-lookup"><span data-stu-id="289a2-151">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="289a2-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="289a2-152">Relationships</span></span>

<span data-ttu-id="289a2-153">Keine.</span><span class="sxs-lookup"><span data-stu-id="289a2-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="289a2-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="289a2-154">JSON representation</span></span>

<span data-ttu-id="289a2-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="289a2-155">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
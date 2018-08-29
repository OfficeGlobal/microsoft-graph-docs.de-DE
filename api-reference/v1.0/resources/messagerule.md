# <a name="messagerule-resource-type"></a><span data-ttu-id="f69da-101">messageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f69da-101">messageRule resource type</span></span>


<span data-ttu-id="f69da-102">Eine Regel, die auf Nachrichten im Posteingang eines Benutzers angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="f69da-102">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="f69da-103">In Outlook können Sie Regeln für eingehende Nachrichten im Posteingang festlegen, um bestimmte Aktionen bei bestimmten Bedingungen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="f69da-103">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="f69da-104">Programmgesteuert können Sie über die **messageRules**-Navigationseigenschaft des [Posteingangsordners](mailfolder.md) auf Regeln zugreifen.</span><span class="sxs-lookup"><span data-stu-id="f69da-104">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="f69da-105">Jede Regel wird von dieser **messageRule**-Ressource dargestellt, verfügbare Regelaktionen werden von dem komplexen Typ [messageRuleActions](messageruleactions.md) dargestellt, und verfügbare Regelbedingungen und -ausnahmen werden von dem komplexen Typ [messageRulePredicates](messagerulepredicates.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="f69da-105">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="f69da-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f69da-106">Properties</span></span>
| <span data-ttu-id="f69da-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f69da-107">Property</span></span>     | <span data-ttu-id="f69da-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f69da-108">Type</span></span>   |<span data-ttu-id="f69da-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f69da-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f69da-110">Aktionen</span><span class="sxs-lookup"><span data-stu-id="f69da-110">actions</span></span> | [<span data-ttu-id="f69da-111">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="f69da-111">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="f69da-112">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="f69da-112">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="f69da-113">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="f69da-113">conditions</span></span> | [<span data-ttu-id="f69da-114">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="f69da-114">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="f69da-115">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="f69da-115">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="f69da-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f69da-116">displayName</span></span> | <span data-ttu-id="f69da-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f69da-117">String</span></span> | <span data-ttu-id="f69da-118">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="f69da-118">The display name of the rule.</span></span> |
| <span data-ttu-id="f69da-119">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="f69da-119">exceptions</span></span> | [<span data-ttu-id="f69da-120">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="f69da-120">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="f69da-121">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="f69da-121">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="f69da-122">hasError</span><span class="sxs-lookup"><span data-stu-id="f69da-122">hasError</span></span> | <span data-ttu-id="f69da-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f69da-123">Boolean</span></span> | <span data-ttu-id="f69da-124">Gibt an, ob sich die Regel in einem Fehlerzustand befindet.</span><span class="sxs-lookup"><span data-stu-id="f69da-124">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="f69da-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f69da-125">Read-only.</span></span> |
| <span data-ttu-id="f69da-126">id</span><span class="sxs-lookup"><span data-stu-id="f69da-126">id</span></span> |<span data-ttu-id="f69da-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f69da-127">String</span></span>|<span data-ttu-id="f69da-128">Der eindeutige Bezeichner der Regel.</span><span class="sxs-lookup"><span data-stu-id="f69da-128">The unique identifier of the rule.</span></span> <span data-ttu-id="f69da-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f69da-129">Read-only.</span></span>|
| <span data-ttu-id="f69da-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f69da-130">isEnabled</span></span> | <span data-ttu-id="f69da-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f69da-131">Boolean</span></span> | <span data-ttu-id="f69da-132">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="f69da-132">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="f69da-133">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="f69da-133">isReadOnly</span></span> | <span data-ttu-id="f69da-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f69da-134">Boolean</span></span> | <span data-ttu-id="f69da-135">Gibt an, ob die Regel schreibgeschützt ist und von der Regel-REST-API nicht geändert oder gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="f69da-135">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="f69da-136">sequence</span><span class="sxs-lookup"><span data-stu-id="f69da-136">sequence</span></span> | <span data-ttu-id="f69da-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f69da-137">Int32</span></span> | <span data-ttu-id="f69da-138">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f69da-138">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f69da-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f69da-139">JSON representation</span></span>
<span data-ttu-id="f69da-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f69da-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
   "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a><span data-ttu-id="f69da-141">Methoden</span><span class="sxs-lookup"><span data-stu-id="f69da-141">Methods</span></span>
| <span data-ttu-id="f69da-142">Methode</span><span class="sxs-lookup"><span data-stu-id="f69da-142">Method</span></span>           | <span data-ttu-id="f69da-143">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f69da-143">Return Type</span></span>    |<span data-ttu-id="f69da-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f69da-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f69da-145">Auflisten von Regeln</span><span class="sxs-lookup"><span data-stu-id="f69da-145">List rules</span></span>](../api/mailfolder_list_messagerules.md) | <span data-ttu-id="f69da-146">[messageRule](messagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f69da-146">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="f69da-147">Ruft alle **messageRule**-Objekte ab, die für das Postfach des Benutzers definiert sind.</span><span class="sxs-lookup"><span data-stu-id="f69da-147">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="f69da-148">Regel abrufen</span><span class="sxs-lookup"><span data-stu-id="f69da-148">Get rule</span></span>](../api/messagerule_get.md) | [<span data-ttu-id="f69da-149">messageRule</span><span class="sxs-lookup"><span data-stu-id="f69da-149">messageRule</span></span>](messagerule.md) |<span data-ttu-id="f69da-150">Lesen der Eigenschaften und Beziehungen eines **messageRule**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f69da-150">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="f69da-151">Erstellen</span><span class="sxs-lookup"><span data-stu-id="f69da-151">Create</span></span>](../api/mailfolder_post_messagerules.md) | [<span data-ttu-id="f69da-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="f69da-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="f69da-153">Erstellen Sie ein  **messageRule**-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.</span><span class="sxs-lookup"><span data-stu-id="f69da-153">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="f69da-154">Update</span><span class="sxs-lookup"><span data-stu-id="f69da-154">Update</span></span>](../api/messagerule_update.md) | [<span data-ttu-id="f69da-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="f69da-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="f69da-156">Ändern Sie die schreibbaren Eigenschaften in einem **messageRule**-Objekt, und speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="f69da-156">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="f69da-157">Delete</span><span class="sxs-lookup"><span data-stu-id="f69da-157">Delete</span></span>](../api/messagerule_delete.md) | <span data-ttu-id="f69da-158">Keine</span><span class="sxs-lookup"><span data-stu-id="f69da-158">None</span></span> |<span data-ttu-id="f69da-159">Löschen des angegebenen **messageRule**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f69da-159">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
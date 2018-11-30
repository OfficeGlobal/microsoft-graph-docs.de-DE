---
title: messageRule-Ressourcentyp
description: Eine Regel, die auf Nachrichten im Posteingang eines Benutzers angewendet wird.
ms.openlocfilehash: 3189ca11f00d5f298e4de29531f20e9da52c8c6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065219"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="d220f-103">messageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d220f-103">messageRule resource type</span></span>

> <span data-ttu-id="d220f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d220f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d220f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d220f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d220f-106">Eine Regel, die auf Nachrichten im Posteingang eines Benutzers angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="d220f-106">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="d220f-107">In Outlook können Sie Regeln für eingehende Nachrichten im Posteingang festlegen, um bestimmte Aktionen bei bestimmten Bedingungen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="d220f-107">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="d220f-108">Programmgesteuert können Sie über die **messageRules**-Navigationseigenschaft des [Posteingangsordners](mailfolder.md) auf Regeln zugreifen.</span><span class="sxs-lookup"><span data-stu-id="d220f-108">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="d220f-109">Jede Regel wird von dieser **messageRule**-Ressource dargestellt, verfügbare Regelaktionen werden von dem komplexen Typ [messageRuleActions](messageruleactions.md) dargestellt, und verfügbare Regelbedingungen und -ausnahmen werden von dem komplexen Typ [messageRulePredicates](messagerulepredicates.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="d220f-109">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="d220f-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d220f-110">Properties</span></span>
| <span data-ttu-id="d220f-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d220f-111">Property</span></span>     | <span data-ttu-id="d220f-112">Typ</span><span class="sxs-lookup"><span data-stu-id="d220f-112">Type</span></span>   |<span data-ttu-id="d220f-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d220f-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d220f-114">Aktionen</span><span class="sxs-lookup"><span data-stu-id="d220f-114">actions</span></span> | [<span data-ttu-id="d220f-115">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="d220f-115">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="d220f-116">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="d220f-116">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="d220f-117">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="d220f-117">conditions</span></span> | [<span data-ttu-id="d220f-118">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="d220f-118">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="d220f-119">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="d220f-119">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="d220f-120">displayName</span><span class="sxs-lookup"><span data-stu-id="d220f-120">displayName</span></span> | <span data-ttu-id="d220f-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d220f-121">String</span></span> | <span data-ttu-id="d220f-122">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="d220f-122">The display name of the rule.</span></span> |
| <span data-ttu-id="d220f-123">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="d220f-123">exceptions</span></span> | [<span data-ttu-id="d220f-124">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="d220f-124">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="d220f-125">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="d220f-125">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="d220f-126">hasError</span><span class="sxs-lookup"><span data-stu-id="d220f-126">hasError</span></span> | <span data-ttu-id="d220f-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d220f-127">Boolean</span></span> | <span data-ttu-id="d220f-128">Gibt an, ob sich die Regel in einem Fehlerzustand befindet.</span><span class="sxs-lookup"><span data-stu-id="d220f-128">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="d220f-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d220f-129">Read-only.</span></span> |
| <span data-ttu-id="d220f-130">id</span><span class="sxs-lookup"><span data-stu-id="d220f-130">id</span></span> |<span data-ttu-id="d220f-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d220f-131">String</span></span>|<span data-ttu-id="d220f-132">Der eindeutige Bezeichner der Regel.</span><span class="sxs-lookup"><span data-stu-id="d220f-132">The unique identifier of the rule.</span></span> <span data-ttu-id="d220f-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d220f-133">Read-only.</span></span>|
| <span data-ttu-id="d220f-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d220f-134">isEnabled</span></span> | <span data-ttu-id="d220f-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d220f-135">Boolean</span></span> | <span data-ttu-id="d220f-136">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d220f-136">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="d220f-137">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="d220f-137">isReadOnly</span></span> | <span data-ttu-id="d220f-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d220f-138">Boolean</span></span> | <span data-ttu-id="d220f-139">Gibt an, ob die Regel schreibgeschützt ist und von der Regel-REST-API nicht geändert oder gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="d220f-139">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="d220f-140">sequence</span><span class="sxs-lookup"><span data-stu-id="d220f-140">sequence</span></span> | <span data-ttu-id="d220f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d220f-141">Int32</span></span> | <span data-ttu-id="d220f-142">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d220f-142">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d220f-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d220f-143">JSON representation</span></span>
<span data-ttu-id="d220f-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d220f-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
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

## <a name="methods"></a><span data-ttu-id="d220f-145">Methoden</span><span class="sxs-lookup"><span data-stu-id="d220f-145">Methods</span></span>
| <span data-ttu-id="d220f-146">Methode</span><span class="sxs-lookup"><span data-stu-id="d220f-146">Method</span></span>           | <span data-ttu-id="d220f-147">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d220f-147">Return Type</span></span>    |<span data-ttu-id="d220f-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d220f-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d220f-149">Auflisten von Regeln</span><span class="sxs-lookup"><span data-stu-id="d220f-149">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="d220f-150">[messageRule](messagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d220f-150">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="d220f-151">Ruft alle **messageRule**-Objekte ab, die für das Postfach des Benutzers definiert sind.</span><span class="sxs-lookup"><span data-stu-id="d220f-151">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="d220f-152">Regel abrufen</span><span class="sxs-lookup"><span data-stu-id="d220f-152">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="d220f-153">messageRule</span><span class="sxs-lookup"><span data-stu-id="d220f-153">messageRule</span></span>](messagerule.md) |<span data-ttu-id="d220f-154">Lesen der Eigenschaften und Beziehungen eines **messageRule**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d220f-154">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="d220f-155">Erstellen</span><span class="sxs-lookup"><span data-stu-id="d220f-155">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="d220f-156">messageRule</span><span class="sxs-lookup"><span data-stu-id="d220f-156">messageRule</span></span>](messagerule.md) |<span data-ttu-id="d220f-157">Erstellen Sie ein  **messageRule**-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.</span><span class="sxs-lookup"><span data-stu-id="d220f-157">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="d220f-158">Update</span><span class="sxs-lookup"><span data-stu-id="d220f-158">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="d220f-159">messageRule</span><span class="sxs-lookup"><span data-stu-id="d220f-159">messageRule</span></span>](messagerule.md) |<span data-ttu-id="d220f-160">Ändern Sie die schreibbaren Eigenschaften in einem **messageRule**-Objekt, und speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="d220f-160">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="d220f-161">Delete</span><span class="sxs-lookup"><span data-stu-id="d220f-161">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="d220f-162">Keine</span><span class="sxs-lookup"><span data-stu-id="d220f-162">None</span></span> |<span data-ttu-id="d220f-163">Löschen des angegebenen **messageRule**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d220f-163">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
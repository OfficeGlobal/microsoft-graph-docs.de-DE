---
title: messageRule-Ressourcentyp
description: Eine Regel, die auf Nachrichten im Posteingang eines Benutzers angewendet wird.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9336f2e35d6c68d86c3e92b5f94c024eff1e49a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862125"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="a1b14-103">messageRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a1b14-103">messageRule resource type</span></span>


<span data-ttu-id="a1b14-104">Eine Regel, die auf Nachrichten im Posteingang eines Benutzers angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="a1b14-104">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="a1b14-105">In Outlook können Sie Regeln für eingehende Nachrichten im Posteingang festlegen, um bestimmte Aktionen bei bestimmten Bedingungen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="a1b14-105">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="a1b14-106">Programmgesteuert können Sie über die **messageRules**-Navigationseigenschaft des [Posteingangsordners](mailfolder.md) auf Regeln zugreifen.</span><span class="sxs-lookup"><span data-stu-id="a1b14-106">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="a1b14-107">Jede Regel wird von dieser **messageRule**-Ressource dargestellt, verfügbare Regelaktionen werden von dem komplexen Typ [messageRuleActions](messageruleactions.md) dargestellt, und verfügbare Regelbedingungen und -ausnahmen werden von dem komplexen Typ [messageRulePredicates](messagerulepredicates.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="a1b14-107">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="a1b14-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1b14-108">Properties</span></span>
| <span data-ttu-id="a1b14-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1b14-109">Property</span></span>     | <span data-ttu-id="a1b14-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a1b14-110">Type</span></span>   |<span data-ttu-id="a1b14-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1b14-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1b14-112">Aktionen</span><span class="sxs-lookup"><span data-stu-id="a1b14-112">actions</span></span> | [<span data-ttu-id="a1b14-113">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="a1b14-113">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="a1b14-114">Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="a1b14-114">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="a1b14-115">Bedingungen</span><span class="sxs-lookup"><span data-stu-id="a1b14-115">conditions</span></span> | [<span data-ttu-id="a1b14-116">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="a1b14-116">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="a1b14-117">Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen.</span><span class="sxs-lookup"><span data-stu-id="a1b14-117">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="a1b14-118">displayName</span><span class="sxs-lookup"><span data-stu-id="a1b14-118">displayName</span></span> | <span data-ttu-id="a1b14-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1b14-119">String</span></span> | <span data-ttu-id="a1b14-120">Der Anzeigename der Regel.</span><span class="sxs-lookup"><span data-stu-id="a1b14-120">The display name of the rule.</span></span> |
| <span data-ttu-id="a1b14-121">Ausnahmen</span><span class="sxs-lookup"><span data-stu-id="a1b14-121">exceptions</span></span> | [<span data-ttu-id="a1b14-122">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="a1b14-122">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="a1b14-123">Ausnahmebedingungen für die Regel.</span><span class="sxs-lookup"><span data-stu-id="a1b14-123">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="a1b14-124">hasError</span><span class="sxs-lookup"><span data-stu-id="a1b14-124">hasError</span></span> | <span data-ttu-id="a1b14-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1b14-125">Boolean</span></span> | <span data-ttu-id="a1b14-126">Gibt an, ob sich die Regel in einem Fehlerzustand befindet.</span><span class="sxs-lookup"><span data-stu-id="a1b14-126">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="a1b14-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b14-127">Read-only.</span></span> |
| <span data-ttu-id="a1b14-128">id</span><span class="sxs-lookup"><span data-stu-id="a1b14-128">id</span></span> |<span data-ttu-id="a1b14-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1b14-129">String</span></span>|<span data-ttu-id="a1b14-130">Der eindeutige Bezeichner der Regel.</span><span class="sxs-lookup"><span data-stu-id="a1b14-130">The unique identifier of the rule.</span></span> <span data-ttu-id="a1b14-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a1b14-131">Read-only.</span></span>|
| <span data-ttu-id="a1b14-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a1b14-132">isEnabled</span></span> | <span data-ttu-id="a1b14-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1b14-133">Boolean</span></span> | <span data-ttu-id="a1b14-134">Gibt an, ob die Regel auf Nachrichten angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="a1b14-134">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="a1b14-135">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="a1b14-135">isReadOnly</span></span> | <span data-ttu-id="a1b14-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1b14-136">Boolean</span></span> | <span data-ttu-id="a1b14-137">Gibt an, ob die Regel schreibgeschützt ist und von der Regel-REST-API nicht geändert oder gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="a1b14-137">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="a1b14-138">sequence</span><span class="sxs-lookup"><span data-stu-id="a1b14-138">sequence</span></span> | <span data-ttu-id="a1b14-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b14-139">Int32</span></span> | <span data-ttu-id="a1b14-140">Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="a1b14-140">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a1b14-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1b14-141">JSON representation</span></span>
<span data-ttu-id="a1b14-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1b14-142">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="a1b14-143">Methoden</span><span class="sxs-lookup"><span data-stu-id="a1b14-143">Methods</span></span>
| <span data-ttu-id="a1b14-144">Methode</span><span class="sxs-lookup"><span data-stu-id="a1b14-144">Method</span></span>           | <span data-ttu-id="a1b14-145">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a1b14-145">Return Type</span></span>    |<span data-ttu-id="a1b14-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1b14-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1b14-147">Auflisten von Regeln</span><span class="sxs-lookup"><span data-stu-id="a1b14-147">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="a1b14-148">[messageRule](messagerule.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a1b14-148">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="a1b14-149">Ruft alle **messageRule**-Objekte ab, die für das Postfach des Benutzers definiert sind.</span><span class="sxs-lookup"><span data-stu-id="a1b14-149">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="a1b14-150">Regel abrufen</span><span class="sxs-lookup"><span data-stu-id="a1b14-150">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="a1b14-151">messageRule</span><span class="sxs-lookup"><span data-stu-id="a1b14-151">messageRule</span></span>](messagerule.md) |<span data-ttu-id="a1b14-152">Lesen der Eigenschaften und Beziehungen eines **messageRule**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1b14-152">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="a1b14-153">Erstellen</span><span class="sxs-lookup"><span data-stu-id="a1b14-153">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="a1b14-154">messageRule</span><span class="sxs-lookup"><span data-stu-id="a1b14-154">messageRule</span></span>](messagerule.md) |<span data-ttu-id="a1b14-155">Erstellen Sie ein  **messageRule**-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.</span><span class="sxs-lookup"><span data-stu-id="a1b14-155">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="a1b14-156">Update</span><span class="sxs-lookup"><span data-stu-id="a1b14-156">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="a1b14-157">messageRule</span><span class="sxs-lookup"><span data-stu-id="a1b14-157">messageRule</span></span>](messagerule.md) |<span data-ttu-id="a1b14-158">Ändern Sie die schreibbaren Eigenschaften in einem **messageRule**-Objekt, und speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="a1b14-158">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="a1b14-159">Delete</span><span class="sxs-lookup"><span data-stu-id="a1b14-159">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="a1b14-160">Keine</span><span class="sxs-lookup"><span data-stu-id="a1b14-160">None</span></span> |<span data-ttu-id="a1b14-161">Löschen des angegebenen **messageRule**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1b14-161">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

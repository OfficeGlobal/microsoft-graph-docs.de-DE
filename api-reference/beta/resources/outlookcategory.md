---
title: outlookCategory-Ressourcentyp
description: Stellt eine Kategorie dar, anhand der ein Benutzer Outlook-Elemente, z. B. Nachrichten und Ereignisse, gruppieren kann. In Outlook der Benutzer Kategorien in einer Masterliste definiert und kann eine oder mehrere der folgenden benutzerdefinierten anwenden
localization_priority: Normal
ms.openlocfilehash: b9c1a3a1813195a36dd1f1cf587cf69d2ddb5f1b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816758"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="90720-104">outlookCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="90720-104">outlookCategory resource type</span></span>

> <span data-ttu-id="90720-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="90720-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90720-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90720-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90720-107">Stellt eine Kategorie dar, anhand der ein Benutzer Outlook-Elemente, z. B. Nachrichten und Ereignisse, gruppieren kann.</span><span class="sxs-lookup"><span data-stu-id="90720-107">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="90720-108">In Outlook wird der Benutzer Kategorien in einer Masterliste definiert und kann eine oder mehrere dieser benutzerdefinierten Kategorien einem Element anwenden.</span><span class="sxs-lookup"><span data-stu-id="90720-108">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="90720-109">Mithilfe der REST-API können Sie Kategorien für einen Benutzer in der Masterliste [erstellen](../api/outlookuser-post-mastercategories.md) und definieren.</span><span class="sxs-lookup"><span data-stu-id="90720-109">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="90720-110">Sie können auch [dieser Masterliste mit Kategorien erhalten](../api/outlookuser-list-mastercategories.md), [eine bestimmte Kategorie abrufen](../api/outlookcategory-get.md), [aktualisieren](../api/outlookcategory-update.md) die Farbe einer Kategorie, oder [Löschen](../api/outlookcategory-delete.md)eine Kategorie.</span><span class="sxs-lookup"><span data-stu-id="90720-110">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="90720-111">Sie können eine Kategorie auf ein Element anwenden, indem Sie die **displayName**-Eigenschaft der Kategorie der **categories**-Sammlung des Elements zuweisen.</span><span class="sxs-lookup"><span data-stu-id="90720-111">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="90720-112">Ressourcen, die Kategorien zugewiesen werden können gehören, [wenden Sie sich an](contact.md), [Ereignis](event.md), [Nachricht](message.md), [OutlookTask](outlooktask.md)und [Buchen](post.md).</span><span class="sxs-lookup"><span data-stu-id="90720-112">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="90720-113">Jede Kategorie weist zwei Eigenschaften auf: **displayName** und **color**.</span><span class="sxs-lookup"><span data-stu-id="90720-113">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="90720-114">Der Wert **displayName** muss in der Masterliste eines Benutzers eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="90720-114">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="90720-115">Die **color**-Eigenschaft muss jedoch nicht eindeutig sein; mehrere Kategorien in der Masterliste können derselben Farbe zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="90720-115">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="90720-116">Sie können bis zu 25 verschiedene Farben Kategorien in der Masterliste eines Benutzers zuordnen.</span><span class="sxs-lookup"><span data-stu-id="90720-116">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="90720-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="90720-117">Properties</span></span>
| <span data-ttu-id="90720-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90720-118">Property</span></span>     | <span data-ttu-id="90720-119">Typ</span><span class="sxs-lookup"><span data-stu-id="90720-119">Type</span></span>   |<span data-ttu-id="90720-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90720-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90720-121">displayName</span><span class="sxs-lookup"><span data-stu-id="90720-121">displayName</span></span>|<span data-ttu-id="90720-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90720-122">String</span></span>|<span data-ttu-id="90720-123">Ein eindeutiger Name, der eine Kategorie im Postfach des Benutzers identifiziert.</span><span class="sxs-lookup"><span data-stu-id="90720-123">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="90720-124">Nach der Erstellung einer Kategorie kann der Namen nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="90720-124">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="90720-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="90720-125">Read-only.</span></span>|
|<span data-ttu-id="90720-126">color</span><span class="sxs-lookup"><span data-stu-id="90720-126">color</span></span>|<span data-ttu-id="90720-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90720-127">String</span></span>|<span data-ttu-id="90720-128">Eine voreingestellte Konstante, die eine Kategorie charakterisiert und einer von 25 vordefinierten Farben zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="90720-128">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="90720-129">Siehe folgenden Hinweis.</span><span class="sxs-lookup"><span data-stu-id="90720-129">See the note below.</span></span> |

> <span data-ttu-id="90720-130">**Hinweis** Die möglichen Werte für **color** sind vordefinierte Konstanten wie `None`, `preset0` und `preset1`.</span><span class="sxs-lookup"><span data-stu-id="90720-130">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="90720-131">Jede voreingestellte Konstante ist weiter einer Farbe zugeordnet. Die tatsächliche Farbe ist von dem Outlook-Client abhängig, auf dem die Kategorien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="90720-131">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="90720-132">In der folgenden Tabelle sind die Farben dargestellt, die den einzelnen vordefinierten Konstanten für Outlook (Desktopclient) zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="90720-132">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="90720-133">Voreingestellte Konstante</span><span class="sxs-lookup"><span data-stu-id="90720-133">Pre-set constant</span></span>  | <span data-ttu-id="90720-134">In Outlook zugeordnete Farbe</span><span class="sxs-lookup"><span data-stu-id="90720-134">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90720-135">Keine</span><span class="sxs-lookup"><span data-stu-id="90720-135">None</span></span> | <span data-ttu-id="90720-136">Keine Farbe zugeordnet</span><span class="sxs-lookup"><span data-stu-id="90720-136">No color mapped</span></span> |
| <span data-ttu-id="90720-137">Preset0</span><span class="sxs-lookup"><span data-stu-id="90720-137">Preset0</span></span> | <span data-ttu-id="90720-138">Red</span><span class="sxs-lookup"><span data-stu-id="90720-138">Red</span></span> |
| <span data-ttu-id="90720-139">Preset1</span><span class="sxs-lookup"><span data-stu-id="90720-139">Preset1</span></span> | <span data-ttu-id="90720-140">Orange</span><span class="sxs-lookup"><span data-stu-id="90720-140">Orange</span></span> |
| <span data-ttu-id="90720-141">Preset2</span><span class="sxs-lookup"><span data-stu-id="90720-141">Preset2</span></span> | <span data-ttu-id="90720-142">Brown</span><span class="sxs-lookup"><span data-stu-id="90720-142">Brown</span></span> |
| <span data-ttu-id="90720-143">Preset3</span><span class="sxs-lookup"><span data-stu-id="90720-143">Preset3</span></span> | <span data-ttu-id="90720-144">Yellow</span><span class="sxs-lookup"><span data-stu-id="90720-144">Yellow</span></span> |
| <span data-ttu-id="90720-145">Preset4</span><span class="sxs-lookup"><span data-stu-id="90720-145">Preset4</span></span> | <span data-ttu-id="90720-146">Green</span><span class="sxs-lookup"><span data-stu-id="90720-146">Green</span></span> |
| <span data-ttu-id="90720-147">Preset5</span><span class="sxs-lookup"><span data-stu-id="90720-147">Preset5</span></span> | <span data-ttu-id="90720-148">Teal</span><span class="sxs-lookup"><span data-stu-id="90720-148">Teal</span></span> |
| <span data-ttu-id="90720-149">Preset6</span><span class="sxs-lookup"><span data-stu-id="90720-149">Preset6</span></span> | <span data-ttu-id="90720-150">Olive</span><span class="sxs-lookup"><span data-stu-id="90720-150">Olive</span></span> |
| <span data-ttu-id="90720-151">Preset7</span><span class="sxs-lookup"><span data-stu-id="90720-151">Preset7</span></span> | <span data-ttu-id="90720-152">Blau</span><span class="sxs-lookup"><span data-stu-id="90720-152">Blue</span></span> |
| <span data-ttu-id="90720-153">Preset8</span><span class="sxs-lookup"><span data-stu-id="90720-153">Preset8</span></span> | <span data-ttu-id="90720-154">Purple</span><span class="sxs-lookup"><span data-stu-id="90720-154">Purple</span></span> |
| <span data-ttu-id="90720-155">Preset9</span><span class="sxs-lookup"><span data-stu-id="90720-155">Preset9</span></span> | <span data-ttu-id="90720-156">Cranberry</span><span class="sxs-lookup"><span data-stu-id="90720-156">Cranberry</span></span> |
| <span data-ttu-id="90720-157">Preset10</span><span class="sxs-lookup"><span data-stu-id="90720-157">Preset10</span></span> | <span data-ttu-id="90720-158">Steel</span><span class="sxs-lookup"><span data-stu-id="90720-158">Steel</span></span> |
| <span data-ttu-id="90720-159">Preset11</span><span class="sxs-lookup"><span data-stu-id="90720-159">Preset11</span></span> | <span data-ttu-id="90720-160">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="90720-160">DarkSteel</span></span> |
| <span data-ttu-id="90720-161">Preset12</span><span class="sxs-lookup"><span data-stu-id="90720-161">Preset12</span></span> | <span data-ttu-id="90720-162">Gray</span><span class="sxs-lookup"><span data-stu-id="90720-162">Gray</span></span> |
| <span data-ttu-id="90720-163">Preset13</span><span class="sxs-lookup"><span data-stu-id="90720-163">Preset13</span></span> | <span data-ttu-id="90720-164">DarkGray</span><span class="sxs-lookup"><span data-stu-id="90720-164">DarkGray</span></span> |
| <span data-ttu-id="90720-165">Preset14</span><span class="sxs-lookup"><span data-stu-id="90720-165">Preset14</span></span> | <span data-ttu-id="90720-166">Black</span><span class="sxs-lookup"><span data-stu-id="90720-166">Black</span></span> |
| <span data-ttu-id="90720-167">Preset15</span><span class="sxs-lookup"><span data-stu-id="90720-167">Preset15</span></span> | <span data-ttu-id="90720-168">DarkRed</span><span class="sxs-lookup"><span data-stu-id="90720-168">DarkRed</span></span> |
| <span data-ttu-id="90720-169">Preset16</span><span class="sxs-lookup"><span data-stu-id="90720-169">Preset16</span></span> | <span data-ttu-id="90720-170">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="90720-170">DarkOrange</span></span> |
| <span data-ttu-id="90720-171">Preset17</span><span class="sxs-lookup"><span data-stu-id="90720-171">Preset17</span></span> | <span data-ttu-id="90720-172">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="90720-172">DarkBrown</span></span> |
| <span data-ttu-id="90720-173">Preset18</span><span class="sxs-lookup"><span data-stu-id="90720-173">Preset18</span></span> | <span data-ttu-id="90720-174">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="90720-174">DarkYellow</span></span> |
| <span data-ttu-id="90720-175">Preset19</span><span class="sxs-lookup"><span data-stu-id="90720-175">Preset19</span></span> | <span data-ttu-id="90720-176">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="90720-176">DarkGreen</span></span> |
| <span data-ttu-id="90720-177">Preset20</span><span class="sxs-lookup"><span data-stu-id="90720-177">Preset20</span></span> | <span data-ttu-id="90720-178">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="90720-178">DarkTeal</span></span> |
| <span data-ttu-id="90720-179">Preset21</span><span class="sxs-lookup"><span data-stu-id="90720-179">Preset21</span></span> | <span data-ttu-id="90720-180">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="90720-180">DarkOlive</span></span> |
| <span data-ttu-id="90720-181">Preset22</span><span class="sxs-lookup"><span data-stu-id="90720-181">Preset22</span></span> | <span data-ttu-id="90720-182">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="90720-182">DarkBlue</span></span> |
| <span data-ttu-id="90720-183">Preset23</span><span class="sxs-lookup"><span data-stu-id="90720-183">Preset23</span></span> | <span data-ttu-id="90720-184">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="90720-184">DarkPurple</span></span> |
| <span data-ttu-id="90720-185">Preset24</span><span class="sxs-lookup"><span data-stu-id="90720-185">Preset24</span></span> | <span data-ttu-id="90720-186">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="90720-186">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="90720-187">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="90720-187">JSON representation</span></span>
<span data-ttu-id="90720-188">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="90720-188">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="90720-189">Methoden</span><span class="sxs-lookup"><span data-stu-id="90720-189">Methods</span></span>
| <span data-ttu-id="90720-190">Methode</span><span class="sxs-lookup"><span data-stu-id="90720-190">Method</span></span>           | <span data-ttu-id="90720-191">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="90720-191">Return Type</span></span>    |<span data-ttu-id="90720-192">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90720-192">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90720-193">Kategorien auflisten</span><span class="sxs-lookup"><span data-stu-id="90720-193">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="90720-194">[outlookCategory](../resources/outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="90720-194">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="90720-195">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="90720-195">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="90720-196">Kategorie abrufen</span><span class="sxs-lookup"><span data-stu-id="90720-196">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="90720-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="90720-197">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="90720-198">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen **outlookCategory**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="90720-198">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="90720-199">Erstellen</span><span class="sxs-lookup"><span data-stu-id="90720-199">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="90720-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="90720-200">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="90720-201">Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="90720-201">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="90720-202">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="90720-202">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="90720-203">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="90720-203">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="90720-204">Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen **outlookCategory**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="90720-204">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="90720-205">Löschen</span><span class="sxs-lookup"><span data-stu-id="90720-205">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="90720-206">Keine</span><span class="sxs-lookup"><span data-stu-id="90720-206">None</span></span> |<span data-ttu-id="90720-207">Löscht das angegebene **outlookCategory**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="90720-207">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/beta/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 

---
title: outlookCategory-Ressourcentyp
description: Stellt eine Kategorie dar, anhand der ein Benutzer Outlook-Elemente, z. B. Nachrichten und Ereignisse, gruppieren kann. Der Benutzer Kategorien in einer Masterliste definiert und kann eine oder mehrere der folgenden benutzerdefinierten anwenden
localization_priority: Normal
ms.openlocfilehash: 08188480bc2b95ded0d1cb9ac033939a17fc92b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832767"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="13ca6-104">outlookCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="13ca6-104">outlookCategory resource type</span></span>


<span data-ttu-id="13ca6-105">Stellt eine Kategorie dar, anhand der ein Benutzer Outlook-Elemente, z. B. Nachrichten und Ereignisse, gruppieren kann.</span><span class="sxs-lookup"><span data-stu-id="13ca6-105">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="13ca6-106">Der Benutzer definiert Kategorien in einer Masterliste und kann eine oder mehrere dieser benutzerdefinierten Kategorien auf ein Element anwenden.</span><span class="sxs-lookup"><span data-stu-id="13ca6-106">The user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="13ca6-107">Mithilfe der REST-API können Sie Kategorien für einen Benutzer in der Masterliste [erstellen](../api/outlookuser-post-mastercategories.md) und definieren.</span><span class="sxs-lookup"><span data-stu-id="13ca6-107">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="13ca6-108">Sie können auch [dieser Masterliste mit Kategorien erhalten](../api/outlookuser-list-mastercategories.md), [eine bestimmte Kategorie abrufen](../api/outlookcategory-get.md), [aktualisieren](../api/outlookcategory-update.md) die Farbe einer Kategorie, oder [Löschen](../api/outlookcategory-delete.md)eine Kategorie.</span><span class="sxs-lookup"><span data-stu-id="13ca6-108">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="13ca6-109">Sie können eine Kategorie auf ein Element anwenden, indem Sie die **displayName**-Eigenschaft der Kategorie der **categories**-Sammlung des Elements zuweisen.</span><span class="sxs-lookup"><span data-stu-id="13ca6-109">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="13ca6-110">Ressourcen, die Kategorien zugewiesen werden können, sind [contact](contact.md), [event](event.md), [message](message.md) und [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="13ca6-110">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), and [post](post.md).</span></span>   

<span data-ttu-id="13ca6-111">Jede Kategorie weist zwei Eigenschaften auf: **displayName** und **color**.</span><span class="sxs-lookup"><span data-stu-id="13ca6-111">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="13ca6-112">Der Wert **displayName** muss in der Masterliste eines Benutzers eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="13ca6-112">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="13ca6-113">Die **color**-Eigenschaft muss jedoch nicht eindeutig sein; mehrere Kategorien in der Masterliste können derselben Farbe zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="13ca6-113">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="13ca6-114">Sie können bis zu 25 verschiedene Farben Kategorien in der Masterliste eines Benutzers zuordnen.</span><span class="sxs-lookup"><span data-stu-id="13ca6-114">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="13ca6-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13ca6-115">Properties</span></span>
| <span data-ttu-id="13ca6-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13ca6-116">Property</span></span>     | <span data-ttu-id="13ca6-117">Typ</span><span class="sxs-lookup"><span data-stu-id="13ca6-117">Type</span></span>   |<span data-ttu-id="13ca6-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13ca6-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13ca6-119">displayName</span><span class="sxs-lookup"><span data-stu-id="13ca6-119">displayName</span></span>|<span data-ttu-id="13ca6-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13ca6-120">String</span></span>|<span data-ttu-id="13ca6-121">Ein eindeutiger Name, der eine Kategorie im Postfach des Benutzers identifiziert.</span><span class="sxs-lookup"><span data-stu-id="13ca6-121">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="13ca6-122">Nach der Erstellung einer Kategorie kann der Namen nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="13ca6-122">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="13ca6-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13ca6-123">Read-only.</span></span>|
|<span data-ttu-id="13ca6-124">color</span><span class="sxs-lookup"><span data-stu-id="13ca6-124">color</span></span>|<span data-ttu-id="13ca6-125">categoryColor</span><span class="sxs-lookup"><span data-stu-id="13ca6-125">categoryColor</span></span>|<span data-ttu-id="13ca6-126">Eine voreingestellte Konstante, die eine Kategorie charakterisiert und einer von 25 vordefinierten Farben zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="13ca6-126">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="13ca6-127">Siehe folgenden Hinweis.</span><span class="sxs-lookup"><span data-stu-id="13ca6-127">See the note below.</span></span> |

> <span data-ttu-id="13ca6-128">**Hinweis** Die möglichen Werte für **color** sind vordefinierte Konstanten wie `None`, `preset0` und `preset1`.</span><span class="sxs-lookup"><span data-stu-id="13ca6-128">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="13ca6-129">Jede voreingestellte Konstante ist weiter einer Farbe zugeordnet. Die tatsächliche Farbe ist von dem Outlook-Client abhängig, auf dem die Kategorien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="13ca6-129">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="13ca6-130">In der folgenden Tabelle sind die Farben dargestellt, die den einzelnen vordefinierten Konstanten für Outlook (Desktopclient) zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="13ca6-130">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 

| <span data-ttu-id="13ca6-131">Voreingestellte Konstante</span><span class="sxs-lookup"><span data-stu-id="13ca6-131">Pre-set constant</span></span>  | <span data-ttu-id="13ca6-132">In Outlook zugeordnete Farbe</span><span class="sxs-lookup"><span data-stu-id="13ca6-132">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13ca6-133">Keine</span><span class="sxs-lookup"><span data-stu-id="13ca6-133">None</span></span> | <span data-ttu-id="13ca6-134">Keine Farbe zugeordnet</span><span class="sxs-lookup"><span data-stu-id="13ca6-134">No color mapped</span></span> |
| <span data-ttu-id="13ca6-135">Preset0</span><span class="sxs-lookup"><span data-stu-id="13ca6-135">Preset0</span></span> | <span data-ttu-id="13ca6-136">Red</span><span class="sxs-lookup"><span data-stu-id="13ca6-136">Red</span></span> |
| <span data-ttu-id="13ca6-137">Preset1</span><span class="sxs-lookup"><span data-stu-id="13ca6-137">Preset1</span></span> | <span data-ttu-id="13ca6-138">Orange</span><span class="sxs-lookup"><span data-stu-id="13ca6-138">Orange</span></span> |
| <span data-ttu-id="13ca6-139">Preset2</span><span class="sxs-lookup"><span data-stu-id="13ca6-139">Preset2</span></span> | <span data-ttu-id="13ca6-140">Brown</span><span class="sxs-lookup"><span data-stu-id="13ca6-140">Brown</span></span> |
| <span data-ttu-id="13ca6-141">Preset3</span><span class="sxs-lookup"><span data-stu-id="13ca6-141">Preset3</span></span> | <span data-ttu-id="13ca6-142">Yellow</span><span class="sxs-lookup"><span data-stu-id="13ca6-142">Yellow</span></span> |
| <span data-ttu-id="13ca6-143">Preset4</span><span class="sxs-lookup"><span data-stu-id="13ca6-143">Preset4</span></span> | <span data-ttu-id="13ca6-144">Green</span><span class="sxs-lookup"><span data-stu-id="13ca6-144">Green</span></span> |
| <span data-ttu-id="13ca6-145">Preset5</span><span class="sxs-lookup"><span data-stu-id="13ca6-145">Preset5</span></span> | <span data-ttu-id="13ca6-146">Teal</span><span class="sxs-lookup"><span data-stu-id="13ca6-146">Teal</span></span> |
| <span data-ttu-id="13ca6-147">Preset6</span><span class="sxs-lookup"><span data-stu-id="13ca6-147">Preset6</span></span> | <span data-ttu-id="13ca6-148">Olive</span><span class="sxs-lookup"><span data-stu-id="13ca6-148">Olive</span></span> |
| <span data-ttu-id="13ca6-149">Preset7</span><span class="sxs-lookup"><span data-stu-id="13ca6-149">Preset7</span></span> | <span data-ttu-id="13ca6-150">Blau</span><span class="sxs-lookup"><span data-stu-id="13ca6-150">Blue</span></span> |
| <span data-ttu-id="13ca6-151">Preset8</span><span class="sxs-lookup"><span data-stu-id="13ca6-151">Preset8</span></span> | <span data-ttu-id="13ca6-152">Purple</span><span class="sxs-lookup"><span data-stu-id="13ca6-152">Purple</span></span> |
| <span data-ttu-id="13ca6-153">Preset9</span><span class="sxs-lookup"><span data-stu-id="13ca6-153">Preset9</span></span> | <span data-ttu-id="13ca6-154">Cranberry</span><span class="sxs-lookup"><span data-stu-id="13ca6-154">Cranberry</span></span> |
| <span data-ttu-id="13ca6-155">Preset10</span><span class="sxs-lookup"><span data-stu-id="13ca6-155">Preset10</span></span> | <span data-ttu-id="13ca6-156">Steel</span><span class="sxs-lookup"><span data-stu-id="13ca6-156">Steel</span></span> |
| <span data-ttu-id="13ca6-157">Preset11</span><span class="sxs-lookup"><span data-stu-id="13ca6-157">Preset11</span></span> | <span data-ttu-id="13ca6-158">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="13ca6-158">DarkSteel</span></span> |
| <span data-ttu-id="13ca6-159">Preset12</span><span class="sxs-lookup"><span data-stu-id="13ca6-159">Preset12</span></span> | <span data-ttu-id="13ca6-160">Gray</span><span class="sxs-lookup"><span data-stu-id="13ca6-160">Gray</span></span> |
| <span data-ttu-id="13ca6-161">Preset13</span><span class="sxs-lookup"><span data-stu-id="13ca6-161">Preset13</span></span> | <span data-ttu-id="13ca6-162">DarkGray</span><span class="sxs-lookup"><span data-stu-id="13ca6-162">DarkGray</span></span> |
| <span data-ttu-id="13ca6-163">Preset14</span><span class="sxs-lookup"><span data-stu-id="13ca6-163">Preset14</span></span> | <span data-ttu-id="13ca6-164">Black</span><span class="sxs-lookup"><span data-stu-id="13ca6-164">Black</span></span> |
| <span data-ttu-id="13ca6-165">Preset15</span><span class="sxs-lookup"><span data-stu-id="13ca6-165">Preset15</span></span> | <span data-ttu-id="13ca6-166">DarkRed</span><span class="sxs-lookup"><span data-stu-id="13ca6-166">DarkRed</span></span> |
| <span data-ttu-id="13ca6-167">Preset16</span><span class="sxs-lookup"><span data-stu-id="13ca6-167">Preset16</span></span> | <span data-ttu-id="13ca6-168">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="13ca6-168">DarkOrange</span></span> |
| <span data-ttu-id="13ca6-169">Preset17</span><span class="sxs-lookup"><span data-stu-id="13ca6-169">Preset17</span></span> | <span data-ttu-id="13ca6-170">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="13ca6-170">DarkBrown</span></span> |
| <span data-ttu-id="13ca6-171">Preset18</span><span class="sxs-lookup"><span data-stu-id="13ca6-171">Preset18</span></span> | <span data-ttu-id="13ca6-172">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="13ca6-172">DarkYellow</span></span> |
| <span data-ttu-id="13ca6-173">Preset19</span><span class="sxs-lookup"><span data-stu-id="13ca6-173">Preset19</span></span> | <span data-ttu-id="13ca6-174">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="13ca6-174">DarkGreen</span></span> |
| <span data-ttu-id="13ca6-175">Preset20</span><span class="sxs-lookup"><span data-stu-id="13ca6-175">Preset20</span></span> | <span data-ttu-id="13ca6-176">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="13ca6-176">DarkTeal</span></span> |
| <span data-ttu-id="13ca6-177">Preset21</span><span class="sxs-lookup"><span data-stu-id="13ca6-177">Preset21</span></span> | <span data-ttu-id="13ca6-178">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="13ca6-178">DarkOlive</span></span> |
| <span data-ttu-id="13ca6-179">Preset22</span><span class="sxs-lookup"><span data-stu-id="13ca6-179">Preset22</span></span> | <span data-ttu-id="13ca6-180">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="13ca6-180">DarkBlue</span></span> |
| <span data-ttu-id="13ca6-181">Preset23</span><span class="sxs-lookup"><span data-stu-id="13ca6-181">Preset23</span></span> | <span data-ttu-id="13ca6-182">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="13ca6-182">DarkPurple</span></span> |
| <span data-ttu-id="13ca6-183">Preset24</span><span class="sxs-lookup"><span data-stu-id="13ca6-183">Preset24</span></span> | <span data-ttu-id="13ca6-184">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="13ca6-184">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13ca6-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13ca6-185">JSON representation</span></span>
<span data-ttu-id="13ca6-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13ca6-186">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="13ca6-187">Methoden</span><span class="sxs-lookup"><span data-stu-id="13ca6-187">Methods</span></span>
| <span data-ttu-id="13ca6-188">Methode</span><span class="sxs-lookup"><span data-stu-id="13ca6-188">Method</span></span>           | <span data-ttu-id="13ca6-189">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="13ca6-189">Return Type</span></span>    |<span data-ttu-id="13ca6-190">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13ca6-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13ca6-191">Kategorien auflisten</span><span class="sxs-lookup"><span data-stu-id="13ca6-191">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="13ca6-192">[outlookCategory](../resources/outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="13ca6-192">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="13ca6-193">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="13ca6-193">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="13ca6-194">Kategorie abrufen</span><span class="sxs-lookup"><span data-stu-id="13ca6-194">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="13ca6-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="13ca6-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="13ca6-196">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen **outlookCategory**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="13ca6-196">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="13ca6-197">Erstellen</span><span class="sxs-lookup"><span data-stu-id="13ca6-197">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="13ca6-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="13ca6-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="13ca6-199">Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="13ca6-199">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="13ca6-200">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="13ca6-200">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="13ca6-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="13ca6-201">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="13ca6-202">Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen **outlookCategory**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="13ca6-202">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="13ca6-203">Löschen</span><span class="sxs-lookup"><span data-stu-id="13ca6-203">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="13ca6-204">Keine</span><span class="sxs-lookup"><span data-stu-id="13ca6-204">None</span></span> |<span data-ttu-id="13ca6-205">Löscht das angegebene **outlookCategory**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="13ca6-205">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 

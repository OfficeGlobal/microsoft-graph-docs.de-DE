---
title: outlookCategory-Ressourcentyp
description: Stellt eine Kategorie dar, anhand der ein Benutzer Outlook-Elemente, z. B. Nachrichten und Ereignisse, gruppieren kann. In Outlook der Benutzer Kategorien in einer Masterliste definiert und kann eine oder mehrere der folgenden benutzerdefinierten anwenden
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5124a681cd4dd1f37ef1ecfea250eb6eb2d228a3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524765"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="4e9e3-104">outlookCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4e9e3-104">outlookCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e9e3-105">Stellt eine Kategorie dar, anhand der ein Benutzer Outlook-Elemente, z. B. Nachrichten und Ereignisse, gruppieren kann.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-105">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="4e9e3-106">In Outlook wird der Benutzer Kategorien in einer Masterliste definiert und kann eine oder mehrere dieser benutzerdefinierten Kategorien einem Element anwenden.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-106">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="4e9e3-107">Mithilfe der REST-API können Sie Kategorien für einen Benutzer in der Masterliste [erstellen](../api/outlookuser-post-mastercategories.md) und definieren.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-107">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="4e9e3-108">Sie können auch [dieser Masterliste mit Kategorien erhalten](../api/outlookuser-list-mastercategories.md), [eine bestimmte Kategorie abrufen](../api/outlookcategory-get.md), [aktualisieren](../api/outlookcategory-update.md) die Farbe einer Kategorie, oder [Löschen](../api/outlookcategory-delete.md)eine Kategorie.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-108">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="4e9e3-109">Sie können eine Kategorie auf ein Element anwenden, indem Sie die **displayName**-Eigenschaft der Kategorie der **categories**-Sammlung des Elements zuweisen.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-109">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="4e9e3-110">Ressourcen, die Kategorien zugewiesen werden können gehören, [wenden Sie sich an](contact.md), [Ereignis](event.md), [Nachricht](message.md), [OutlookTask](outlooktask.md)und [Buchen](post.md).</span><span class="sxs-lookup"><span data-stu-id="4e9e3-110">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="4e9e3-111">Jede Kategorie weist zwei Eigenschaften auf: **displayName** und **color**.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-111">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="4e9e3-112">Der Wert **displayName** muss in der Masterliste eines Benutzers eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-112">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="4e9e3-113">Die **color**-Eigenschaft muss jedoch nicht eindeutig sein; mehrere Kategorien in der Masterliste können derselben Farbe zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-113">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="4e9e3-114">Sie können bis zu 25 verschiedene Farben Kategorien in der Masterliste eines Benutzers zuordnen.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-114">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="4e9e3-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e9e3-115">Properties</span></span>
| <span data-ttu-id="4e9e3-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e9e3-116">Property</span></span>     | <span data-ttu-id="4e9e3-117">Typ</span><span class="sxs-lookup"><span data-stu-id="4e9e3-117">Type</span></span>   |<span data-ttu-id="4e9e3-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e9e3-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e9e3-119">displayName</span><span class="sxs-lookup"><span data-stu-id="4e9e3-119">displayName</span></span>|<span data-ttu-id="4e9e3-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4e9e3-120">String</span></span>|<span data-ttu-id="4e9e3-121">Ein eindeutiger Name, der eine Kategorie im Postfach des Benutzers identifiziert.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-121">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="4e9e3-122">Nach der Erstellung einer Kategorie kann der Namen nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-122">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="4e9e3-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-123">Read-only.</span></span>|
|<span data-ttu-id="4e9e3-124">color</span><span class="sxs-lookup"><span data-stu-id="4e9e3-124">color</span></span>|<span data-ttu-id="4e9e3-125">String</span><span class="sxs-lookup"><span data-stu-id="4e9e3-125">String</span></span>|<span data-ttu-id="4e9e3-126">Eine voreingestellte Konstante, die eine Kategorie charakterisiert und einer von 25 vordefinierten Farben zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-126">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="4e9e3-127">Siehe folgenden Hinweis.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-127">See the note below.</span></span> |

> <span data-ttu-id="4e9e3-128">**Hinweis** Die möglichen Werte für **color** sind vordefinierte Konstanten wie `None`, `preset0` und `preset1`.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-128">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="4e9e3-129">Jede voreingestellte Konstante ist weiter einer Farbe zugeordnet. Die tatsächliche Farbe ist von dem Outlook-Client abhängig, auf dem die Kategorien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-129">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="4e9e3-130">In der folgenden Tabelle sind die Farben dargestellt, die den einzelnen vordefinierten Konstanten für Outlook (Desktopclient) zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-130">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="4e9e3-131">Voreingestellte Konstante</span><span class="sxs-lookup"><span data-stu-id="4e9e3-131">Pre-set constant</span></span>  | <span data-ttu-id="4e9e3-132">In Outlook zugeordnete Farbe</span><span class="sxs-lookup"><span data-stu-id="4e9e3-132">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e9e3-133">Keine</span><span class="sxs-lookup"><span data-stu-id="4e9e3-133">None</span></span> | <span data-ttu-id="4e9e3-134">Keine Farbe zugeordnet</span><span class="sxs-lookup"><span data-stu-id="4e9e3-134">No color mapped</span></span> |
| <span data-ttu-id="4e9e3-135">Preset0</span><span class="sxs-lookup"><span data-stu-id="4e9e3-135">Preset0</span></span> | <span data-ttu-id="4e9e3-136">Red</span><span class="sxs-lookup"><span data-stu-id="4e9e3-136">Red</span></span> |
| <span data-ttu-id="4e9e3-137">Preset1</span><span class="sxs-lookup"><span data-stu-id="4e9e3-137">Preset1</span></span> | <span data-ttu-id="4e9e3-138">Orange</span><span class="sxs-lookup"><span data-stu-id="4e9e3-138">Orange</span></span> |
| <span data-ttu-id="4e9e3-139">Preset2</span><span class="sxs-lookup"><span data-stu-id="4e9e3-139">Preset2</span></span> | <span data-ttu-id="4e9e3-140">Brown</span><span class="sxs-lookup"><span data-stu-id="4e9e3-140">Brown</span></span> |
| <span data-ttu-id="4e9e3-141">Preset3</span><span class="sxs-lookup"><span data-stu-id="4e9e3-141">Preset3</span></span> | <span data-ttu-id="4e9e3-142">Yellow</span><span class="sxs-lookup"><span data-stu-id="4e9e3-142">Yellow</span></span> |
| <span data-ttu-id="4e9e3-143">Preset4</span><span class="sxs-lookup"><span data-stu-id="4e9e3-143">Preset4</span></span> | <span data-ttu-id="4e9e3-144">Green</span><span class="sxs-lookup"><span data-stu-id="4e9e3-144">Green</span></span> |
| <span data-ttu-id="4e9e3-145">Preset5</span><span class="sxs-lookup"><span data-stu-id="4e9e3-145">Preset5</span></span> | <span data-ttu-id="4e9e3-146">Teal</span><span class="sxs-lookup"><span data-stu-id="4e9e3-146">Teal</span></span> |
| <span data-ttu-id="4e9e3-147">Preset6</span><span class="sxs-lookup"><span data-stu-id="4e9e3-147">Preset6</span></span> | <span data-ttu-id="4e9e3-148">Olive</span><span class="sxs-lookup"><span data-stu-id="4e9e3-148">Olive</span></span> |
| <span data-ttu-id="4e9e3-149">Preset7</span><span class="sxs-lookup"><span data-stu-id="4e9e3-149">Preset7</span></span> | <span data-ttu-id="4e9e3-150">Blau</span><span class="sxs-lookup"><span data-stu-id="4e9e3-150">Blue</span></span> |
| <span data-ttu-id="4e9e3-151">Preset8</span><span class="sxs-lookup"><span data-stu-id="4e9e3-151">Preset8</span></span> | <span data-ttu-id="4e9e3-152">Purple</span><span class="sxs-lookup"><span data-stu-id="4e9e3-152">Purple</span></span> |
| <span data-ttu-id="4e9e3-153">Preset9</span><span class="sxs-lookup"><span data-stu-id="4e9e3-153">Preset9</span></span> | <span data-ttu-id="4e9e3-154">Cranberry</span><span class="sxs-lookup"><span data-stu-id="4e9e3-154">Cranberry</span></span> |
| <span data-ttu-id="4e9e3-155">Preset10</span><span class="sxs-lookup"><span data-stu-id="4e9e3-155">Preset10</span></span> | <span data-ttu-id="4e9e3-156">Steel</span><span class="sxs-lookup"><span data-stu-id="4e9e3-156">Steel</span></span> |
| <span data-ttu-id="4e9e3-157">Preset11</span><span class="sxs-lookup"><span data-stu-id="4e9e3-157">Preset11</span></span> | <span data-ttu-id="4e9e3-158">DarkSteel</span><span class="sxs-lookup"><span data-stu-id="4e9e3-158">DarkSteel</span></span> |
| <span data-ttu-id="4e9e3-159">Preset12</span><span class="sxs-lookup"><span data-stu-id="4e9e3-159">Preset12</span></span> | <span data-ttu-id="4e9e3-160">Gray</span><span class="sxs-lookup"><span data-stu-id="4e9e3-160">Gray</span></span> |
| <span data-ttu-id="4e9e3-161">Preset13</span><span class="sxs-lookup"><span data-stu-id="4e9e3-161">Preset13</span></span> | <span data-ttu-id="4e9e3-162">DarkGray</span><span class="sxs-lookup"><span data-stu-id="4e9e3-162">DarkGray</span></span> |
| <span data-ttu-id="4e9e3-163">Preset14</span><span class="sxs-lookup"><span data-stu-id="4e9e3-163">Preset14</span></span> | <span data-ttu-id="4e9e3-164">Black</span><span class="sxs-lookup"><span data-stu-id="4e9e3-164">Black</span></span> |
| <span data-ttu-id="4e9e3-165">Preset15</span><span class="sxs-lookup"><span data-stu-id="4e9e3-165">Preset15</span></span> | <span data-ttu-id="4e9e3-166">DarkRed</span><span class="sxs-lookup"><span data-stu-id="4e9e3-166">DarkRed</span></span> |
| <span data-ttu-id="4e9e3-167">Preset16</span><span class="sxs-lookup"><span data-stu-id="4e9e3-167">Preset16</span></span> | <span data-ttu-id="4e9e3-168">DarkOrange</span><span class="sxs-lookup"><span data-stu-id="4e9e3-168">DarkOrange</span></span> |
| <span data-ttu-id="4e9e3-169">Preset17</span><span class="sxs-lookup"><span data-stu-id="4e9e3-169">Preset17</span></span> | <span data-ttu-id="4e9e3-170">DarkBrown</span><span class="sxs-lookup"><span data-stu-id="4e9e3-170">DarkBrown</span></span> |
| <span data-ttu-id="4e9e3-171">Preset18</span><span class="sxs-lookup"><span data-stu-id="4e9e3-171">Preset18</span></span> | <span data-ttu-id="4e9e3-172">DarkYellow</span><span class="sxs-lookup"><span data-stu-id="4e9e3-172">DarkYellow</span></span> |
| <span data-ttu-id="4e9e3-173">Preset19</span><span class="sxs-lookup"><span data-stu-id="4e9e3-173">Preset19</span></span> | <span data-ttu-id="4e9e3-174">DarkGreen</span><span class="sxs-lookup"><span data-stu-id="4e9e3-174">DarkGreen</span></span> |
| <span data-ttu-id="4e9e3-175">Preset20</span><span class="sxs-lookup"><span data-stu-id="4e9e3-175">Preset20</span></span> | <span data-ttu-id="4e9e3-176">DarkTeal</span><span class="sxs-lookup"><span data-stu-id="4e9e3-176">DarkTeal</span></span> |
| <span data-ttu-id="4e9e3-177">Preset21</span><span class="sxs-lookup"><span data-stu-id="4e9e3-177">Preset21</span></span> | <span data-ttu-id="4e9e3-178">DarkOlive</span><span class="sxs-lookup"><span data-stu-id="4e9e3-178">DarkOlive</span></span> |
| <span data-ttu-id="4e9e3-179">Preset22</span><span class="sxs-lookup"><span data-stu-id="4e9e3-179">Preset22</span></span> | <span data-ttu-id="4e9e3-180">DarkBlue</span><span class="sxs-lookup"><span data-stu-id="4e9e3-180">DarkBlue</span></span> |
| <span data-ttu-id="4e9e3-181">Preset23</span><span class="sxs-lookup"><span data-stu-id="4e9e3-181">Preset23</span></span> | <span data-ttu-id="4e9e3-182">DarkPurple</span><span class="sxs-lookup"><span data-stu-id="4e9e3-182">DarkPurple</span></span> |
| <span data-ttu-id="4e9e3-183">Preset24</span><span class="sxs-lookup"><span data-stu-id="4e9e3-183">Preset24</span></span> | <span data-ttu-id="4e9e3-184">DarkCranberry</span><span class="sxs-lookup"><span data-stu-id="4e9e3-184">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e9e3-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e9e3-185">JSON representation</span></span>
<span data-ttu-id="4e9e3-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-186">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="4e9e3-187">Methoden</span><span class="sxs-lookup"><span data-stu-id="4e9e3-187">Methods</span></span>
| <span data-ttu-id="4e9e3-188">Methode</span><span class="sxs-lookup"><span data-stu-id="4e9e3-188">Method</span></span>           | <span data-ttu-id="4e9e3-189">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4e9e3-189">Return Type</span></span>    |<span data-ttu-id="4e9e3-190">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e9e3-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e9e3-191">Kategorien auflisten</span><span class="sxs-lookup"><span data-stu-id="4e9e3-191">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="4e9e3-192">[outlookCategory](../resources/outlookcategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e9e3-192">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="4e9e3-193">Ruft alle Kategorien ab, die für den Benutzer definiert wurden.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-193">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="4e9e3-194">Kategorie abrufen</span><span class="sxs-lookup"><span data-stu-id="4e9e3-194">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="4e9e3-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="4e9e3-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="4e9e3-196">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen **outlookCategory**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-196">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="4e9e3-197">Erstellen</span><span class="sxs-lookup"><span data-stu-id="4e9e3-197">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="4e9e3-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="4e9e3-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="4e9e3-199">Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-199">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="4e9e3-200">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4e9e3-200">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="4e9e3-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="4e9e3-201">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="4e9e3-202">Aktualisieren Sie die schreibbare Eigenschaft, **color**, des angegebenen **outlookCategory**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-202">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="4e9e3-203">Löschen</span><span class="sxs-lookup"><span data-stu-id="4e9e3-203">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="4e9e3-204">Keine</span><span class="sxs-lookup"><span data-stu-id="4e9e3-204">None</span></span> |<span data-ttu-id="4e9e3-205">Löscht das angegebene **outlookCategory**-Objekt.</span><span class="sxs-lookup"><span data-stu-id="4e9e3-205">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/outlookcategory.md:\r\n      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|",
    "Error: /api-reference/beta/resources/outlookcategory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
 

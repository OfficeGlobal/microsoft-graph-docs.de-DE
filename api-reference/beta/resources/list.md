---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Auflisten
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 419f35226c09c1bde500994b6e023f764c54b3cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953616"
---
# <a name="list-resource"></a><span data-ttu-id="32531-102">List-Ressource</span><span class="sxs-lookup"><span data-stu-id="32531-102">List resource</span></span>

> <span data-ttu-id="32531-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="32531-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32531-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32531-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32531-105">The **list**-Ressource stellt eine Liste auf einer [Website][] dar.</span><span class="sxs-lookup"><span data-stu-id="32531-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="32531-106">Diese Ressource enthält die Eigenschaften der Liste auf oberster Ebene, einschließlich der Vorlage- und Feld-Definitionen.</span><span class="sxs-lookup"><span data-stu-id="32531-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="32531-107">Aufgaben in einer Liste</span><span class="sxs-lookup"><span data-stu-id="32531-107">Tasks on a list</span></span>

<span data-ttu-id="32531-108">Die folgenden Aufgaben stehen für list-Ressourcen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="32531-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="32531-109">**Hinweis:** Mit dieser Beta können Sie nur durch Listen navigieren, keine Listen erstellen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="32531-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="32531-110">Sie können jedoch [Listenelemente][listItem] erstellen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="32531-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="32531-111">Alle Beispiele unten beziehen sich auf  eine Website, z. B.: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="32531-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="32531-112">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="32531-112">Common task</span></span>               | <span data-ttu-id="32531-113">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="32531-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="32531-114">[Liste abrufen][]</span><span class="sxs-lookup"><span data-stu-id="32531-114">[Get list][]</span></span>              | <span data-ttu-id="32531-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="32531-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="32531-116">[Listenelemente auflisten][]</span><span class="sxs-lookup"><span data-stu-id="32531-116">[Enumerate list items][]</span></span>  | <span data-ttu-id="32531-117">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="32531-117">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="32531-118">[Listenelement aktualisieren][]</span><span class="sxs-lookup"><span data-stu-id="32531-118">[Update list item][]</span></span>      | <span data-ttu-id="32531-119">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="32531-119">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="32531-120">[Listenelement löschen][]</span><span class="sxs-lookup"><span data-stu-id="32531-120">[Delete list item][]</span></span>      | <span data-ttu-id="32531-121">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="32531-121">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="32531-122">[Listenelement erstellen][]</span><span class="sxs-lookup"><span data-stu-id="32531-122">[Create list item][]</span></span>      | <span data-ttu-id="32531-123">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="32531-123">POST /lists/{list-id}</span></span>
| <span data-ttu-id="32531-124">[Aktuelle Aktivitäten abrufen][]</span><span class="sxs-lookup"><span data-stu-id="32531-124">[Get recent activities][]</span></span> | <span data-ttu-id="32531-125">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="32531-125">GET /lists/{list-id}/activities</span></span>

[Liste abrufen]: ../api/list-get.md
[Get list]: ../api/list-get.md
[Listenelemente auflisten]: ../api/listitem-list.md
[Enumerate list items]: ../api/listitem-list.md
[Listenelement aktualisieren]: ../api/listitem-update.md
[Update list item]: ../api/listitem-update.md
[Listenelement löschen]: ../api/listitem-delete.md
[Delete list item]: ../api/listitem-delete.md
[Listenelement erstellen]: ../api/listitem-create.md
[Create list item]: ../api/listitem-create.md
[Aktuelle Aktivitäten abrufen]: ../api/activities-list.md
[Get recent activities]: ../api/activities-list.md

## <a name="json-representation"></a><span data-ttu-id="32531-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="32531-132">JSON representation</span></span>

<span data-ttu-id="32531-133">Es folgt eine JSON-Darstellung einer **list**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="32531-133">Here is a JSON representation of a **list** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
  },
  "system": false,

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="32531-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="32531-134">Properties</span></span>

<span data-ttu-id="32531-135">Die **list**-Ressource besitzt folgende Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="32531-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="32531-136">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="32531-136">Property name</span></span>    | <span data-ttu-id="32531-137">Typ</span><span class="sxs-lookup"><span data-stu-id="32531-137">Type</span></span>                             | <span data-ttu-id="32531-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32531-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="32531-139">**columns**</span><span class="sxs-lookup"><span data-stu-id="32531-139">**columns**</span></span>      | <span data-ttu-id="32531-140">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="32531-140">Collection([columnDefinition][])</span></span> | <span data-ttu-id="32531-141">Die Sammlung von Felddefinitionen für diese Liste.</span><span class="sxs-lookup"><span data-stu-id="32531-141">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="32531-142">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="32531-142">**contentTypes**</span></span> | <span data-ttu-id="32531-143">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="32531-143">Collection([contentType][])</span></span>      | <span data-ttu-id="32531-144">Die Sammlung von in dieser Liste enthaltenen content-Typen.</span><span class="sxs-lookup"><span data-stu-id="32531-144">The collection of content types present in this list.</span></span>
| <span data-ttu-id="32531-145">**displayName**</span><span class="sxs-lookup"><span data-stu-id="32531-145">**displayName**</span></span>  | <span data-ttu-id="32531-146">string</span><span class="sxs-lookup"><span data-stu-id="32531-146">string</span></span>                           | <span data-ttu-id="32531-147">Der anzeigbare Titel der Liste.</span><span class="sxs-lookup"><span data-stu-id="32531-147">The displayable title of the list.</span></span>
| <span data-ttu-id="32531-148">**list**</span><span class="sxs-lookup"><span data-stu-id="32531-148">**list**</span></span>         | <span data-ttu-id="32531-149">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="32531-149">[listInfo][]</span></span>                     | <span data-ttu-id="32531-150">Weitere Details über die Liste.</span><span class="sxs-lookup"><span data-stu-id="32531-150">Provides additional details about the list.</span></span>
| <span data-ttu-id="32531-151">**system**</span><span class="sxs-lookup"><span data-stu-id="32531-151">**system**</span></span>       | <span data-ttu-id="32531-152">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="32531-152">[systemFacet][]</span></span>                  | <span data-ttu-id="32531-153">Falls vorhanden, gibt an, dass es sich um eine vom System verwaltete Liste handelt.</span><span class="sxs-lookup"><span data-stu-id="32531-153">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="32531-154">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32531-154">Read-only.</span></span>

<span data-ttu-id="32531-155">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="32531-155">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="32531-156">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="32531-156">Property name</span></span>            | <span data-ttu-id="32531-157">Typ</span><span class="sxs-lookup"><span data-stu-id="32531-157">Type</span></span>             | <span data-ttu-id="32531-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32531-158">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="32531-159">**id**</span><span class="sxs-lookup"><span data-stu-id="32531-159">**id**</span></span>                   | <span data-ttu-id="32531-160">string</span><span class="sxs-lookup"><span data-stu-id="32531-160">string</span></span>           | <span data-ttu-id="32531-p105">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32531-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="32531-163">**name**</span><span class="sxs-lookup"><span data-stu-id="32531-163">**name**</span></span>                 | <span data-ttu-id="32531-164">string</span><span class="sxs-lookup"><span data-stu-id="32531-164">string</span></span>           | <span data-ttu-id="32531-165">Der Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="32531-165">The name of the item.</span></span>
| <span data-ttu-id="32531-166">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="32531-166">**createdBy**</span></span>            | <span data-ttu-id="32531-167">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="32531-167">[identitySet][]</span></span>  | <span data-ttu-id="32531-168">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="32531-168">Identity of the creator of this item.</span></span> <span data-ttu-id="32531-169">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32531-169">Read-only.</span></span>
| <span data-ttu-id="32531-170">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="32531-170">**createdDateTime**</span></span>      | <span data-ttu-id="32531-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32531-171">DateTimeOffset</span></span>   | <span data-ttu-id="32531-p107">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32531-p107">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="32531-174">**description**</span><span class="sxs-lookup"><span data-stu-id="32531-174">**description**</span></span>          | <span data-ttu-id="32531-175">string</span><span class="sxs-lookup"><span data-stu-id="32531-175">string</span></span>           | <span data-ttu-id="32531-176">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="32531-176">The descriptive text for the item.</span></span>
| <span data-ttu-id="32531-177">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="32531-177">**lastModifiedBy**</span></span>       | <span data-ttu-id="32531-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="32531-178">[identitySet][]</span></span>  | <span data-ttu-id="32531-179">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="32531-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="32531-180">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32531-180">Read-only.</span></span>
| <span data-ttu-id="32531-181">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="32531-181">**lastModifiedDateTime**</span></span> | <span data-ttu-id="32531-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32531-182">DateTimeOffset</span></span>   | <span data-ttu-id="32531-p109">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32531-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="32531-185">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="32531-185">**webUrl**</span></span>               | <span data-ttu-id="32531-186">String (URL)</span><span class="sxs-lookup"><span data-stu-id="32531-186">string (url)</span></span>     | <span data-ttu-id="32531-p110">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32531-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="32531-189">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="32531-189">Relationships</span></span>

<span data-ttu-id="32531-190">Die **list**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="32531-190">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="32531-191">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="32531-191">Relationship name</span></span> | <span data-ttu-id="32531-192">Typ</span><span class="sxs-lookup"><span data-stu-id="32531-192">Type</span></span>                        | <span data-ttu-id="32531-193">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32531-193">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="32531-194">**activities**</span><span class="sxs-lookup"><span data-stu-id="32531-194">**activities**</span></span>    | <span data-ttu-id="32531-195">[itemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="32531-195">[itemActivity][] collection</span></span> | <span data-ttu-id="32531-196">Die letzten Aktivitäten, die innerhalb dieser Liste stattfanden.</span><span class="sxs-lookup"><span data-stu-id="32531-196">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="32531-197">**drive**</span><span class="sxs-lookup"><span data-stu-id="32531-197">**drive**</span></span>         | <span data-ttu-id="32531-198">[drive][]</span><span class="sxs-lookup"><span data-stu-id="32531-198">[drive][]</span></span>                   | <span data-ttu-id="32531-199">Nur in Dokumentbibliotheken vorhanden.</span><span class="sxs-lookup"><span data-stu-id="32531-199">Only present on document libraries.</span></span> <span data-ttu-id="32531-200">Ermöglicht den Zugriff auf die Liste als [drive][]-Ressource mit [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="32531-200">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="32531-201">**items**</span><span class="sxs-lookup"><span data-stu-id="32531-201">**items**</span></span>         | <span data-ttu-id="32531-202">Sammlung ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="32531-202">Collection([listItem][])</span></span>    | <span data-ttu-id="32531-203">Alle in der Liste enthaltenen Elemente.</span><span class="sxs-lookup"><span data-stu-id="32531-203">All items contained in the list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[Website]: site.md
[site]: site.md
[systemFacet]: systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  }
} -->

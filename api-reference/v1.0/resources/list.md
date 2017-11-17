---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Auflisten
ms.openlocfilehash: ba0c01ce1887a32bd8b671cf511104e9128b5efb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="list-resource"></a><span data-ttu-id="d53ed-102">List-Ressource</span><span class="sxs-lookup"><span data-stu-id="d53ed-102">List resource</span></span>

<span data-ttu-id="d53ed-103">The **list**-Ressource stellt eine Liste auf einer [Website][] dar.</span><span class="sxs-lookup"><span data-stu-id="d53ed-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="d53ed-104">Diese Ressource enthält die Eigenschaften der Liste auf oberster Ebene, einschließlich der Vorlage- und Feld-Definitionen.</span><span class="sxs-lookup"><span data-stu-id="d53ed-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="d53ed-105">Aufgaben in einer Liste</span><span class="sxs-lookup"><span data-stu-id="d53ed-105">Tasks on a list</span></span>

<span data-ttu-id="d53ed-106">Die folgenden Aufgaben stehen für list-Ressourcen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="d53ed-106">The following tasks are available for {type} resources.</span></span>
<span data-ttu-id="d53ed-107">**Hinweis:** Mit dieser Beta können Sie nur durch Listen navigieren, keine Listen erstellen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d53ed-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="d53ed-108">Sie können jedoch [Listenelemente][listItem] erstellen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d53ed-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="d53ed-109">Alle Beispiele unten beziehen sich auf  eine Website, z. B.: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="d53ed-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="d53ed-110">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="d53ed-110">Common task</span></span>               | <span data-ttu-id="d53ed-111">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="d53ed-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="d53ed-112">[Liste abrufen][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-112">[Get list][]</span></span>              | <span data-ttu-id="d53ed-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="d53ed-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="d53ed-114">[Listenelemente auflisten][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="d53ed-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="d53ed-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="d53ed-116">[Listenelement aktualisieren][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-116">[Update list item][]</span></span>      | <span data-ttu-id="d53ed-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="d53ed-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="d53ed-118">[Listenelement löschen][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-118">[Delete list item][]</span></span>      | <span data-ttu-id="d53ed-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="d53ed-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="d53ed-120">[Listenelement erstellen][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-120">[Create list item][]</span></span>      | <span data-ttu-id="d53ed-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="d53ed-121">POST /lists/{list-id}</span></span>

[Liste abrufen]: ../api/list_get.md
[Listenelemente auflisten]: ../api/listitem_list.md
[Listenelement aktualisieren]: ../api/listItem_update.md
[Listenelement löschen]: ../api/listItem_delete.md
[Listenelement erstellen]: ../api/listItem_create.md

## <a name="json-representation"></a><span data-ttu-id="d53ed-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d53ed-127">JSON representation</span></span>

<span data-ttu-id="d53ed-128">Es folgt eine JSON-Darstellung einer **list**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="d53ed-128">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
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

## <a name="properties"></a><span data-ttu-id="d53ed-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d53ed-129">Properties</span></span>

<span data-ttu-id="d53ed-130">Die **list**-Ressource besitzt folgende Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="d53ed-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="d53ed-131">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="d53ed-131">Property name</span></span>    | <span data-ttu-id="d53ed-132">Typ</span><span class="sxs-lookup"><span data-stu-id="d53ed-132">Type</span></span>                             | <span data-ttu-id="d53ed-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d53ed-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="d53ed-134">**columns**</span><span class="sxs-lookup"><span data-stu-id="d53ed-134">**columns**</span></span>      | <span data-ttu-id="d53ed-135">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="d53ed-135">Collection([columnDefinition][])</span></span> | <span data-ttu-id="d53ed-136">Die Sammlung von Felddefinitionen für diese Liste.</span><span class="sxs-lookup"><span data-stu-id="d53ed-136">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="d53ed-137">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="d53ed-137">**contentTypes**</span></span> | <span data-ttu-id="d53ed-138">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="d53ed-138">Collection([contentType][])</span></span>      | <span data-ttu-id="d53ed-139">Die Sammlung von in dieser Liste enthaltenen content-Typen.</span><span class="sxs-lookup"><span data-stu-id="d53ed-139">The collection of content types present in this list.</span></span>
| <span data-ttu-id="d53ed-140">**displayName**</span><span class="sxs-lookup"><span data-stu-id="d53ed-140">**displayName**</span></span>  | <span data-ttu-id="d53ed-141">string</span><span class="sxs-lookup"><span data-stu-id="d53ed-141">string</span></span>                           | <span data-ttu-id="d53ed-142">Der anzeigbare Titel der Liste.</span><span class="sxs-lookup"><span data-stu-id="d53ed-142">The new title of the list.</span></span>
| <span data-ttu-id="d53ed-143">**list**</span><span class="sxs-lookup"><span data-stu-id="d53ed-143">**list**</span></span>         | <span data-ttu-id="d53ed-144">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-144">[listInfo][]</span></span>                     | <span data-ttu-id="d53ed-145">Weitere Details über die Liste.</span><span class="sxs-lookup"><span data-stu-id="d53ed-145">Provides additional details about the list.</span></span>
| <span data-ttu-id="d53ed-146">**system**</span><span class="sxs-lookup"><span data-stu-id="d53ed-146">**System**</span></span>       | <span data-ttu-id="d53ed-147">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-147">[systemFacet][]</span></span>                  | <span data-ttu-id="d53ed-148">Falls vorhanden, gibt an, dass es sich um eine vom System verwaltete Liste handelt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-148">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="d53ed-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-149">Read-only.</span></span>

<span data-ttu-id="d53ed-150">Die folgenden Eigenschaften werden von  ** [baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-150">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="d53ed-151">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="d53ed-151">Property name</span></span>            | <span data-ttu-id="d53ed-152">Typ</span><span class="sxs-lookup"><span data-stu-id="d53ed-152">Type</span></span>             | <span data-ttu-id="d53ed-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d53ed-153">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="d53ed-154">**id**</span><span class="sxs-lookup"><span data-stu-id="d53ed-154">**id**</span></span>                   | <span data-ttu-id="d53ed-155">string</span><span class="sxs-lookup"><span data-stu-id="d53ed-155">string</span></span>           | <span data-ttu-id="d53ed-p104">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="d53ed-158">**name**</span><span class="sxs-lookup"><span data-stu-id="d53ed-158">**name**</span></span>                 | <span data-ttu-id="d53ed-159">string</span><span class="sxs-lookup"><span data-stu-id="d53ed-159">string</span></span>           | <span data-ttu-id="d53ed-160">Der Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="d53ed-160">The name of the item.</span></span>
| <span data-ttu-id="d53ed-161">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="d53ed-161">**createdBy**</span></span>            | <span data-ttu-id="d53ed-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-162">[identitySet][]</span></span>  | <span data-ttu-id="d53ed-163">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="d53ed-163">Identity of the creator of this item.</span></span> <span data-ttu-id="d53ed-164">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-164">Read-only.</span></span>
| <span data-ttu-id="d53ed-165">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="d53ed-165">**createdDateTime**</span></span>      | <span data-ttu-id="d53ed-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d53ed-166">DateTimeOffset</span></span>   | <span data-ttu-id="d53ed-p106">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="d53ed-169">**description**</span><span class="sxs-lookup"><span data-stu-id="d53ed-169">**description**</span></span>          | <span data-ttu-id="d53ed-170">string</span><span class="sxs-lookup"><span data-stu-id="d53ed-170">string</span></span>           | <span data-ttu-id="d53ed-171">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="d53ed-171">The descriptive text for the site.</span></span>
| <span data-ttu-id="d53ed-172">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="d53ed-172">**lastModifiedBy**</span></span>       | <span data-ttu-id="d53ed-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-173">[identitySet][]</span></span>  | <span data-ttu-id="d53ed-174">Die Identität der Person, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="d53ed-174">Identity of the last modifier of this item.</span></span> <span data-ttu-id="d53ed-175">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-175">Read-only.</span></span>
| <span data-ttu-id="d53ed-176">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d53ed-176">**lastModifiedDateTime**</span></span> | <span data-ttu-id="d53ed-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d53ed-177">DateTimeOffset</span></span>   | <span data-ttu-id="d53ed-p108">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="d53ed-180">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="d53ed-180">**webUrl**</span></span>               | <span data-ttu-id="d53ed-181">String (URL)</span><span class="sxs-lookup"><span data-stu-id="d53ed-181">string (url)</span></span>     | <span data-ttu-id="d53ed-p109">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d53ed-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="d53ed-184">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d53ed-184">Relationships</span></span>

<span data-ttu-id="d53ed-185">Die **list**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="d53ed-185">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="d53ed-186">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="d53ed-186">Relationship name</span></span> | <span data-ttu-id="d53ed-187">Typ</span><span class="sxs-lookup"><span data-stu-id="d53ed-187">Type</span></span>                        | <span data-ttu-id="d53ed-188">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d53ed-188">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="d53ed-189">**drive**</span><span class="sxs-lookup"><span data-stu-id="d53ed-189">**drive**</span></span>         | <span data-ttu-id="d53ed-190">[drive][]</span><span class="sxs-lookup"><span data-stu-id="d53ed-190">[drive][]</span></span>                   | <span data-ttu-id="d53ed-191">Nur in Dokumentbibliotheken vorhanden.</span><span class="sxs-lookup"><span data-stu-id="d53ed-191">Only present on document libraries.</span></span> <span data-ttu-id="d53ed-192">Ermöglicht den Zugriff auf die Liste als [drive][]-Ressource mit [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="d53ed-192">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="d53ed-193">**items**</span><span class="sxs-lookup"><span data-stu-id="d53ed-193">**items**</span></span>         | <span data-ttu-id="d53ed-194">Sammlung ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="d53ed-194">Collection([listItem][])</span></span>    | <span data-ttu-id="d53ed-195">Alle in der Liste enthaltenen Elemente.</span><span class="sxs-lookup"><span data-stu-id="d53ed-195">All items contained in the drive.</span></span>

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[listInfo]: listInfo.md
[listItem]: listItem.md
[site]: site.md
[systemFacet]: systemFacet.md

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

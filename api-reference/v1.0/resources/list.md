---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Auflisten
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 7946346c5b872cad80eb3b8dc50109862ac15b8e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481405"
---
# <a name="list-resource"></a><span data-ttu-id="62373-102">List-Ressource</span><span class="sxs-lookup"><span data-stu-id="62373-102">List resource</span></span>

<span data-ttu-id="62373-103">The **list**-Ressource stellt eine Liste auf einer [Website][] dar.</span><span class="sxs-lookup"><span data-stu-id="62373-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="62373-104">Diese Ressource enthält die Eigenschaften der Liste auf oberster Ebene, einschließlich der Vorlage- und Feld-Definitionen.</span><span class="sxs-lookup"><span data-stu-id="62373-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="62373-105">Aufgaben in einer Liste</span><span class="sxs-lookup"><span data-stu-id="62373-105">Tasks on a list</span></span>

<span data-ttu-id="62373-106">Die folgenden Aufgaben stehen für list-Ressourcen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="62373-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="62373-107">**Hinweis:** Mit dieser Beta können Sie nur durch Listen navigieren, keine Listen erstellen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="62373-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="62373-108">Sie können jedoch [Listenelemente][listItem] erstellen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="62373-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="62373-109">Alle Beispiele unten beziehen sich auf  eine Website, z. B.: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="62373-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="62373-110">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="62373-110">Common task</span></span>               | <span data-ttu-id="62373-111">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="62373-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="62373-112">[Liste abrufen][]</span><span class="sxs-lookup"><span data-stu-id="62373-112">[Get list][]</span></span>              | <span data-ttu-id="62373-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="62373-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="62373-114">[Listenelemente auflisten][]</span><span class="sxs-lookup"><span data-stu-id="62373-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="62373-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="62373-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="62373-116">[Listenelement aktualisieren][]</span><span class="sxs-lookup"><span data-stu-id="62373-116">[Update list item][]</span></span>      | <span data-ttu-id="62373-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="62373-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="62373-118">[Listenelement löschen][]</span><span class="sxs-lookup"><span data-stu-id="62373-118">[Delete list item][]</span></span>      | <span data-ttu-id="62373-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="62373-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="62373-120">[Listenelement erstellen][]</span><span class="sxs-lookup"><span data-stu-id="62373-120">[Create list item][]</span></span>      | <span data-ttu-id="62373-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="62373-121">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="62373-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="62373-127">JSON representation</span></span>

<span data-ttu-id="62373-128">Es folgt eine JSON-Darstellung einer **list**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="62373-128">Here is a JSON representation of a **list** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.list"
}-->

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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
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
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="62373-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="62373-129">Properties</span></span>

<span data-ttu-id="62373-130">Die **list**-Ressource besitzt folgende Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="62373-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="62373-131">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="62373-131">Property name</span></span>    | <span data-ttu-id="62373-132">Typ</span><span class="sxs-lookup"><span data-stu-id="62373-132">Type</span></span>                             | <span data-ttu-id="62373-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62373-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="62373-134">**displayName**</span><span class="sxs-lookup"><span data-stu-id="62373-134">**displayName**</span></span>  | <span data-ttu-id="62373-135">string</span><span class="sxs-lookup"><span data-stu-id="62373-135">string</span></span>                           | <span data-ttu-id="62373-136">Der anzeigbare Titel der Liste.</span><span class="sxs-lookup"><span data-stu-id="62373-136">The displayable title of the list.</span></span>
| <span data-ttu-id="62373-137">**list**</span><span class="sxs-lookup"><span data-stu-id="62373-137">**list**</span></span>         | <span data-ttu-id="62373-138">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="62373-138">[listInfo][]</span></span>                     | <span data-ttu-id="62373-139">Weitere Details über die Liste.</span><span class="sxs-lookup"><span data-stu-id="62373-139">Provides additional details about the list.</span></span>
| <span data-ttu-id="62373-140">**system**</span><span class="sxs-lookup"><span data-stu-id="62373-140">**system**</span></span>       | <span data-ttu-id="62373-141">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="62373-141">[systemFacet][]</span></span>                  | <span data-ttu-id="62373-142">Falls vorhanden, gibt an, dass es sich um eine vom System verwaltete Liste handelt.</span><span class="sxs-lookup"><span data-stu-id="62373-142">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="62373-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-143">Read-only.</span></span>

<span data-ttu-id="62373-144">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="62373-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="62373-145">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="62373-145">Property name</span></span>            | <span data-ttu-id="62373-146">Typ</span><span class="sxs-lookup"><span data-stu-id="62373-146">Type</span></span>              | <span data-ttu-id="62373-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62373-147">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="62373-148">**id**</span><span class="sxs-lookup"><span data-stu-id="62373-148">**id**</span></span>                   | <span data-ttu-id="62373-149">string</span><span class="sxs-lookup"><span data-stu-id="62373-149">string</span></span>            | <span data-ttu-id="62373-p104">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="62373-152">**name**</span><span class="sxs-lookup"><span data-stu-id="62373-152">**name**</span></span>                 | <span data-ttu-id="62373-153">string</span><span class="sxs-lookup"><span data-stu-id="62373-153">string</span></span>            | <span data-ttu-id="62373-154">Der Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="62373-154">The name of the item.</span></span>
| <span data-ttu-id="62373-155">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="62373-155">**createdBy**</span></span>            | <span data-ttu-id="62373-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="62373-156">[identitySet][]</span></span>   | <span data-ttu-id="62373-157">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="62373-157">Identity of the creator of this item.</span></span> <span data-ttu-id="62373-158">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-158">Read-only.</span></span>
| <span data-ttu-id="62373-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="62373-159">**createdDateTime**</span></span>      | <span data-ttu-id="62373-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62373-160">DateTimeOffset</span></span>    | <span data-ttu-id="62373-p106">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="62373-163">**description**</span><span class="sxs-lookup"><span data-stu-id="62373-163">**description**</span></span>          | <span data-ttu-id="62373-164">string</span><span class="sxs-lookup"><span data-stu-id="62373-164">string</span></span>            | <span data-ttu-id="62373-165">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="62373-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="62373-166">**eTag**</span><span class="sxs-lookup"><span data-stu-id="62373-166">**eTag**</span></span>                 | <span data-ttu-id="62373-167">string</span><span class="sxs-lookup"><span data-stu-id="62373-167">string</span></span>            | <span data-ttu-id="62373-p107">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="62373-170">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="62373-170">**lastModifiedBy**</span></span>       | <span data-ttu-id="62373-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="62373-171">[identitySet][]</span></span>   | <span data-ttu-id="62373-172">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="62373-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="62373-173">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-173">Read-only.</span></span>
| <span data-ttu-id="62373-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="62373-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="62373-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62373-175">DateTimeOffset</span></span>    | <span data-ttu-id="62373-p109">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="62373-178">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="62373-178">**parentReference**</span></span>      | <span data-ttu-id="62373-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="62373-179">[itemReference][]</span></span> | <span data-ttu-id="62373-p110">Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="62373-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="62373-182">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="62373-182">**sharepointIds**</span></span>        | <span data-ttu-id="62373-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="62373-183">[sharepointIds][]</span></span> | <span data-ttu-id="62373-p111">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="62373-186">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="62373-186">**webUrl**</span></span>               | <span data-ttu-id="62373-187">String (URL)</span><span class="sxs-lookup"><span data-stu-id="62373-187">string (url)</span></span>      | <span data-ttu-id="62373-p112">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="62373-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="62373-190">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="62373-190">Relationships</span></span>

<span data-ttu-id="62373-191">Die **list**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="62373-191">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="62373-192">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="62373-192">Relationship name</span></span> | <span data-ttu-id="62373-193">Typ</span><span class="sxs-lookup"><span data-stu-id="62373-193">Type</span></span>                             | <span data-ttu-id="62373-194">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62373-194">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="62373-195">**drive**</span><span class="sxs-lookup"><span data-stu-id="62373-195">**drive**</span></span>         | <span data-ttu-id="62373-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="62373-196">[drive][]</span></span>                        | <span data-ttu-id="62373-197">Nur in Dokumentbibliotheken vorhanden.</span><span class="sxs-lookup"><span data-stu-id="62373-197">Only present on document libraries.</span></span> <span data-ttu-id="62373-198">Ermöglicht den Zugriff auf die Liste als [drive][]-Ressource mit [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="62373-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="62373-199">**items**</span><span class="sxs-lookup"><span data-stu-id="62373-199">**items**</span></span>         | <span data-ttu-id="62373-200">Sammlung ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="62373-200">Collection([listItem][])</span></span>         | <span data-ttu-id="62373-201">Alle in der Liste enthaltenen Elemente.</span><span class="sxs-lookup"><span data-stu-id="62373-201">All items contained in the list.</span></span>
| <span data-ttu-id="62373-202">**columns**</span><span class="sxs-lookup"><span data-stu-id="62373-202">**columns**</span></span>       | <span data-ttu-id="62373-203">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="62373-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="62373-204">Die Sammlung von Felddefinitionen für diese Liste.</span><span class="sxs-lookup"><span data-stu-id="62373-204">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="62373-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="62373-205">**contentTypes**</span></span>  | <span data-ttu-id="62373-206">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="62373-206">Collection([contentType][])</span></span>      | <span data-ttu-id="62373-207">Die Sammlung von in dieser Liste enthaltenen content-Typen.</span><span class="sxs-lookup"><span data-stu-id="62373-207">The collection of content types present in this list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[sharepointIds]: sharepointids.md
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

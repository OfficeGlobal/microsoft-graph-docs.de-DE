---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Auflisten
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: aafae9e9214f98ade129d46b63f0e7f930ac4a9c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481517"
---
# <a name="list-resource"></a><span data-ttu-id="69e0e-102">List-Ressource</span><span class="sxs-lookup"><span data-stu-id="69e0e-102">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69e0e-103">The **list**-Ressource stellt eine Liste auf einer [Website][] dar.</span><span class="sxs-lookup"><span data-stu-id="69e0e-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="69e0e-104">Diese Ressource enthält die Eigenschaften der Liste auf oberster Ebene, einschließlich der Vorlage- und Feld-Definitionen.</span><span class="sxs-lookup"><span data-stu-id="69e0e-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="69e0e-105">Aufgaben in einer Liste</span><span class="sxs-lookup"><span data-stu-id="69e0e-105">Tasks on a list</span></span>

<span data-ttu-id="69e0e-106">Die folgenden Aufgaben stehen für list-Ressourcen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="69e0e-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="69e0e-107">**Hinweis:** Mit dieser Beta können Sie nur durch Listen navigieren, keine Listen erstellen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="69e0e-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="69e0e-108">Sie können jedoch [Listenelemente][listItem] erstellen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="69e0e-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="69e0e-109">Alle Beispiele unten beziehen sich auf  eine Website, z. B.: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="69e0e-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="69e0e-110">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="69e0e-110">Common task</span></span>               | <span data-ttu-id="69e0e-111">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="69e0e-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="69e0e-112">[Liste abrufen][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-112">[Get list][]</span></span>              | <span data-ttu-id="69e0e-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="69e0e-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="69e0e-114">[Listenelemente auflisten][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="69e0e-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="69e0e-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="69e0e-116">[Listenelement aktualisieren][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-116">[Update list item][]</span></span>      | <span data-ttu-id="69e0e-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="69e0e-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="69e0e-118">[Listenelement löschen][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-118">[Delete list item][]</span></span>      | <span data-ttu-id="69e0e-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="69e0e-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="69e0e-120">[Listenelement erstellen][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-120">[Create list item][]</span></span>      | <span data-ttu-id="69e0e-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="69e0e-121">POST /lists/{list-id}</span></span>
| <span data-ttu-id="69e0e-122">[Aktuelle Aktivitäten abrufen][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-122">[Get recent activities][]</span></span> | <span data-ttu-id="69e0e-123">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="69e0e-123">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="69e0e-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69e0e-130">JSON representation</span></span>

<span data-ttu-id="69e0e-131">Es folgt eine JSON-Darstellung einer **list**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="69e0e-131">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="69e0e-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69e0e-132">Properties</span></span>

<span data-ttu-id="69e0e-133">Die **list**-Ressource besitzt folgende Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="69e0e-133">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="69e0e-134">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="69e0e-134">Property name</span></span>    | <span data-ttu-id="69e0e-135">Typ</span><span class="sxs-lookup"><span data-stu-id="69e0e-135">Type</span></span>                             | <span data-ttu-id="69e0e-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69e0e-136">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="69e0e-137">**columns**</span><span class="sxs-lookup"><span data-stu-id="69e0e-137">**columns**</span></span>      | <span data-ttu-id="69e0e-138">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="69e0e-138">Collection([columnDefinition][])</span></span> | <span data-ttu-id="69e0e-139">Die Sammlung von Felddefinitionen für diese Liste.</span><span class="sxs-lookup"><span data-stu-id="69e0e-139">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="69e0e-140">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="69e0e-140">**contentTypes**</span></span> | <span data-ttu-id="69e0e-141">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="69e0e-141">Collection([contentType][])</span></span>      | <span data-ttu-id="69e0e-142">Die Sammlung von in dieser Liste enthaltenen content-Typen.</span><span class="sxs-lookup"><span data-stu-id="69e0e-142">The collection of content types present in this list.</span></span>
| <span data-ttu-id="69e0e-143">**displayName**</span><span class="sxs-lookup"><span data-stu-id="69e0e-143">**displayName**</span></span>  | <span data-ttu-id="69e0e-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69e0e-144">string</span></span>                           | <span data-ttu-id="69e0e-145">Der anzeigbare Titel der Liste.</span><span class="sxs-lookup"><span data-stu-id="69e0e-145">The displayable title of the list.</span></span>
| <span data-ttu-id="69e0e-146">**list**</span><span class="sxs-lookup"><span data-stu-id="69e0e-146">**list**</span></span>         | <span data-ttu-id="69e0e-147">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-147">[listInfo][]</span></span>                     | <span data-ttu-id="69e0e-148">Weitere Details über die Liste.</span><span class="sxs-lookup"><span data-stu-id="69e0e-148">Provides additional details about the list.</span></span>
| <span data-ttu-id="69e0e-149">**system**</span><span class="sxs-lookup"><span data-stu-id="69e0e-149">**system**</span></span>       | <span data-ttu-id="69e0e-150">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-150">[systemFacet][]</span></span>                  | <span data-ttu-id="69e0e-151">Falls vorhanden, gibt an, dass es sich um eine vom System verwaltete Liste handelt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-151">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="69e0e-152">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-152">Read-only.</span></span>

<span data-ttu-id="69e0e-153">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="69e0e-154">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="69e0e-154">Property name</span></span>            | <span data-ttu-id="69e0e-155">Typ</span><span class="sxs-lookup"><span data-stu-id="69e0e-155">Type</span></span>             | <span data-ttu-id="69e0e-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69e0e-156">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="69e0e-157">**id**</span><span class="sxs-lookup"><span data-stu-id="69e0e-157">**id**</span></span>                   | <span data-ttu-id="69e0e-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69e0e-158">string</span></span>           | <span data-ttu-id="69e0e-p104">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="69e0e-161">**name**</span><span class="sxs-lookup"><span data-stu-id="69e0e-161">**name**</span></span>                 | <span data-ttu-id="69e0e-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69e0e-162">string</span></span>           | <span data-ttu-id="69e0e-163">Der Name des Elements.</span><span class="sxs-lookup"><span data-stu-id="69e0e-163">The name of the item.</span></span>
| <span data-ttu-id="69e0e-164">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="69e0e-164">**createdBy**</span></span>            | <span data-ttu-id="69e0e-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-165">[identitySet][]</span></span>  | <span data-ttu-id="69e0e-166">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="69e0e-166">Identity of the creator of this item.</span></span> <span data-ttu-id="69e0e-167">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-167">Read-only.</span></span>
| <span data-ttu-id="69e0e-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="69e0e-168">**createdDateTime**</span></span>      | <span data-ttu-id="69e0e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e0e-169">DateTimeOffset</span></span>   | <span data-ttu-id="69e0e-p106">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="69e0e-172">**description**</span><span class="sxs-lookup"><span data-stu-id="69e0e-172">**description**</span></span>          | <span data-ttu-id="69e0e-173">string</span><span class="sxs-lookup"><span data-stu-id="69e0e-173">string</span></span>           | <span data-ttu-id="69e0e-174">Der beschreibende Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="69e0e-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="69e0e-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="69e0e-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="69e0e-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-176">[identitySet][]</span></span>  | <span data-ttu-id="69e0e-177">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="69e0e-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="69e0e-178">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-178">Read-only.</span></span>
| <span data-ttu-id="69e0e-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="69e0e-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="69e0e-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69e0e-180">DateTimeOffset</span></span>   | <span data-ttu-id="69e0e-p108">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="69e0e-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="69e0e-183">**webUrl**</span></span>               | <span data-ttu-id="69e0e-184">String (URL)</span><span class="sxs-lookup"><span data-stu-id="69e0e-184">string (url)</span></span>     | <span data-ttu-id="69e0e-p109">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69e0e-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="69e0e-187">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69e0e-187">Relationships</span></span>

<span data-ttu-id="69e0e-188">Die **list**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.</span><span class="sxs-lookup"><span data-stu-id="69e0e-188">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="69e0e-189">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="69e0e-189">Relationship name</span></span> | <span data-ttu-id="69e0e-190">Typ</span><span class="sxs-lookup"><span data-stu-id="69e0e-190">Type</span></span>                        | <span data-ttu-id="69e0e-191">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69e0e-191">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="69e0e-192">**activities**</span><span class="sxs-lookup"><span data-stu-id="69e0e-192">**activities**</span></span>    | <span data-ttu-id="69e0e-193">[itemActivity][]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="69e0e-193">[itemActivity][] collection</span></span> | <span data-ttu-id="69e0e-194">Die letzten Aktivitäten, die innerhalb dieser Liste stattfanden.</span><span class="sxs-lookup"><span data-stu-id="69e0e-194">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="69e0e-195">**drive**</span><span class="sxs-lookup"><span data-stu-id="69e0e-195">**drive**</span></span>         | <span data-ttu-id="69e0e-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="69e0e-196">[drive][]</span></span>                   | <span data-ttu-id="69e0e-197">Nur in Dokumentbibliotheken vorhanden.</span><span class="sxs-lookup"><span data-stu-id="69e0e-197">Only present on document libraries.</span></span> <span data-ttu-id="69e0e-198">Ermöglicht den Zugriff auf die Liste als [drive][]-Ressource mit [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="69e0e-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="69e0e-199">**items**</span><span class="sxs-lookup"><span data-stu-id="69e0e-199">**items**</span></span>         | <span data-ttu-id="69e0e-200">Sammlung ([listItem][])</span><span class="sxs-lookup"><span data-stu-id="69e0e-200">Collection([listItem][])</span></span>    | <span data-ttu-id="69e0e-201">Alle in der Liste enthaltenen Elemente.</span><span class="sxs-lookup"><span data-stu-id="69e0e-201">All items contained in the list.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

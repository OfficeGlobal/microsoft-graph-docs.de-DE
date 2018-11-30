---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Website
ms.openlocfilehash: d18487d9932227df0ce2de3320fcb71ce94ca735
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063905"
---
# <a name="site-resource-type"></a><span data-ttu-id="8ac91-102">Website-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8ac91-102">site resource type</span></span>

> <span data-ttu-id="8ac91-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ac91-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ac91-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ac91-105">Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.</span><span class="sxs-lookup"><span data-stu-id="8ac91-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="8ac91-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="8ac91-106">Methods</span></span>

| <span data-ttu-id="8ac91-107">Methode</span><span class="sxs-lookup"><span data-stu-id="8ac91-107">Method</span></span>                         | <span data-ttu-id="8ac91-108">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="8ac91-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="8ac91-109">[Stammwebsite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-109">[Get root site][]</span></span>              | <span data-ttu-id="8ac91-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="8ac91-110">GET /sites/root</span></span>
| <span data-ttu-id="8ac91-111">[Website abrufen][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-111">[Get site][]</span></span>                   | <span data-ttu-id="8ac91-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="8ac91-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="8ac91-113">[Website nach Pfad abrufen][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-113">[Get site by path][]</span></span>           | <span data-ttu-id="8ac91-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="8ac91-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="8ac91-115">[Website für eine Gruppe abrufen][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-115">[Get site for a group][]</span></span>       | <span data-ttu-id="8ac91-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="8ac91-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="8ac91-117">[Abrufen von analytics][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-117">[Get analytics][]</span></span>              | <span data-ttu-id="8ac91-118">GET/Sites / {Site-Id} / Analytics</span><span class="sxs-lookup"><span data-stu-id="8ac91-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="8ac91-119">[Abrufen von Aktivitäten nach Intervall][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-119">[Get activities by interval][]</span></span> | <span data-ttu-id="8ac91-120">GET/Sites / {Site-Id} / GetActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="8ac91-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="8ac91-121">[Seiten auflisten][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-121">[List pages][]</span></span>                 | <span data-ttu-id="8ac91-122">GET/Sites / {Site-Id} / pages</span><span class="sxs-lookup"><span data-stu-id="8ac91-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="8ac91-123">[Stamm Websites aufgelistet werden sollen][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-123">[List root sites][]</span></span>            | <span data-ttu-id="8ac91-124">GET/Sites? Filter = Root Ne null & select = SiteCollection WebUrl</span><span class="sxs-lookup"><span data-stu-id="8ac91-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="8ac91-125">[Nach Websites suchen][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-125">[Search for sites][]</span></span>           | <span data-ttu-id="8ac91-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="8ac91-126">GET /sites?search={query}</span></span>

[Website abrufen]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Stammwebsite abrufen]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Website nach Pfad abrufen]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Website für eine Gruppe abrufen]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Abrufen von analytics]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Abrufen von Aktivitäten nach Intervall]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Seiten auflisten]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Stamm Websites aufgelistet werden sollen]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[Nach Websites suchen]: ../api/site-search.md
[Search for sites]: ../api/site-search.md


## <a name="properties"></a><span data-ttu-id="8ac91-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8ac91-136">Properties</span></span>

| <span data-ttu-id="8ac91-137">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8ac91-137">Property name</span></span>            | <span data-ttu-id="8ac91-138">Typ</span><span class="sxs-lookup"><span data-stu-id="8ac91-138">Type</span></span>               | <span data-ttu-id="8ac91-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ac91-139">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="8ac91-140">**id**</span><span class="sxs-lookup"><span data-stu-id="8ac91-140">**id**</span></span>                   | <span data-ttu-id="8ac91-141">string</span><span class="sxs-lookup"><span data-stu-id="8ac91-141">string</span></span>             | <span data-ttu-id="8ac91-p102">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="8ac91-144">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="8ac91-144">**createdDateTime**</span></span>      | <span data-ttu-id="8ac91-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ac91-145">DateTimeOffset</span></span>     | <span data-ttu-id="8ac91-p103">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p103">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="8ac91-148">**description**</span><span class="sxs-lookup"><span data-stu-id="8ac91-148">**description**</span></span>          | <span data-ttu-id="8ac91-149">string</span><span class="sxs-lookup"><span data-stu-id="8ac91-149">string</span></span>             | <span data-ttu-id="8ac91-150">Der beschreibende Text für die Website.</span><span class="sxs-lookup"><span data-stu-id="8ac91-150">The descriptive text for the site.</span></span>
| <span data-ttu-id="8ac91-151">**eTag**</span><span class="sxs-lookup"><span data-stu-id="8ac91-151">**eTag**</span></span>                 | <span data-ttu-id="8ac91-152">string</span><span class="sxs-lookup"><span data-stu-id="8ac91-152">string</span></span>             | <span data-ttu-id="8ac91-p104">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="8ac91-155">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8ac91-155">**displayName**</span></span>          | <span data-ttu-id="8ac91-156">string</span><span class="sxs-lookup"><span data-stu-id="8ac91-156">string</span></span>             | <span data-ttu-id="8ac91-p105">Der vollständigen Titel für die Website. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p105">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="8ac91-159">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8ac91-159">**lastModifiedDateTime**</span></span> | <span data-ttu-id="8ac91-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ac91-160">DateTimeOffset</span></span>     | <span data-ttu-id="8ac91-p106">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p106">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="8ac91-163">**name**</span><span class="sxs-lookup"><span data-stu-id="8ac91-163">**name**</span></span>                 | <span data-ttu-id="8ac91-164">string</span><span class="sxs-lookup"><span data-stu-id="8ac91-164">string</span></span>             | <span data-ttu-id="8ac91-165">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="8ac91-165">The name / title of the item.</span></span>
| <span data-ttu-id="8ac91-166">**root**</span><span class="sxs-lookup"><span data-stu-id="8ac91-166">**root**</span></span>                 | <span data-ttu-id="8ac91-167">[root][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-167">[root][]</span></span>           | <span data-ttu-id="8ac91-p107">Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p107">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="8ac91-170">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="8ac91-170">**sharepointIds**</span></span>        | <span data-ttu-id="8ac91-171">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-171">[sharepointIds][]</span></span>  | <span data-ttu-id="8ac91-p108">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p108">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="8ac91-174">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="8ac91-174">**siteCollection**</span></span>       | <span data-ttu-id="8ac91-175">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-175">[siteCollection][]</span></span> | <span data-ttu-id="8ac91-p109">Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p109">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="8ac91-179">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="8ac91-179">**webUrl**</span></span>               | <span data-ttu-id="8ac91-180">String (URL)</span><span class="sxs-lookup"><span data-stu-id="8ac91-180">string (url)</span></span>       | <span data-ttu-id="8ac91-p110">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="8ac91-183">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8ac91-183">Relationships</span></span>

| <span data-ttu-id="8ac91-184">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="8ac91-184">Relationship name</span></span> | <span data-ttu-id="8ac91-185">Typ</span><span class="sxs-lookup"><span data-stu-id="8ac91-185">Type</span></span>                             | <span data-ttu-id="8ac91-186">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ac91-186">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="8ac91-187">**Analytics**</span><span class="sxs-lookup"><span data-stu-id="8ac91-187">**analytics**</span></span>     | <span data-ttu-id="8ac91-188">[ItemAnalytics][] -Ressource</span><span class="sxs-lookup"><span data-stu-id="8ac91-188">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="8ac91-189">Analytics über die Aktivitäten anzeigen, die auf dieser Site durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="8ac91-189">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="8ac91-190">**columns**</span><span class="sxs-lookup"><span data-stu-id="8ac91-190">**columns**</span></span>       | <span data-ttu-id="8ac91-191">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="8ac91-191">Collection([columnDefinition][])</span></span> | <span data-ttu-id="8ac91-192">Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.</span><span class="sxs-lookup"><span data-stu-id="8ac91-192">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="8ac91-193">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="8ac91-193">**contentTypes**</span></span>  | <span data-ttu-id="8ac91-194">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="8ac91-194">Collection([contentType][])</span></span>      | <span data-ttu-id="8ac91-195">Die Sammlung von für diese Website definierten Inhaltstypen.</span><span class="sxs-lookup"><span data-stu-id="8ac91-195">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="8ac91-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="8ac91-196">**drive**</span></span>         | <span data-ttu-id="8ac91-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="8ac91-197">[drive][]</span></span>                        | <span data-ttu-id="8ac91-198">Das Standardlaufwerk (Dokumentbibliothek) für diese Website.</span><span class="sxs-lookup"><span data-stu-id="8ac91-198">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="8ac91-199">**drives**</span><span class="sxs-lookup"><span data-stu-id="8ac91-199">**drives**</span></span>        | <span data-ttu-id="8ac91-200">Sammlung ([drive][])</span><span class="sxs-lookup"><span data-stu-id="8ac91-200">Collection([drive][])</span></span>            | <span data-ttu-id="8ac91-201">Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="8ac91-201">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="8ac91-202">**items**</span><span class="sxs-lookup"><span data-stu-id="8ac91-202">**items**</span></span>         | <span data-ttu-id="8ac91-203">Sammlung ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="8ac91-203">Collection([baseItem][])</span></span>         | <span data-ttu-id="8ac91-p111">Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="8ac91-p111">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="8ac91-206">**Listen**</span><span class="sxs-lookup"><span data-stu-id="8ac91-206">**lists**</span></span>         | <span data-ttu-id="8ac91-207">Sammlung ([Liste][])</span><span class="sxs-lookup"><span data-stu-id="8ac91-207">Collection([list][])</span></span>             | <span data-ttu-id="8ac91-208">Die Sammlung der Listen unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="8ac91-208">The collection of lists under this site.</span></span>
| <span data-ttu-id="8ac91-209">**Seiten**</span><span class="sxs-lookup"><span data-stu-id="8ac91-209">**pages**</span></span>         | <span data-ttu-id="8ac91-210">Auflistung ([SitePage][])</span><span class="sxs-lookup"><span data-stu-id="8ac91-210">Collection([sitePage][])</span></span>         | <span data-ttu-id="8ac91-211">Die Auflistung von Seiten in der Liste SitePages auf dieser Site.</span><span class="sxs-lookup"><span data-stu-id="8ac91-211">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="8ac91-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="8ac91-212">**sites**</span></span>         | <span data-ttu-id="8ac91-213">Sammlung ([site][])</span><span class="sxs-lookup"><span data-stu-id="8ac91-213">Collection([site][])</span></span>             | <span data-ttu-id="8ac91-214">Die Sammlung der Unterwebsites unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="8ac91-214">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[Website]: site.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="8ac91-226">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8ac91-226">JSON representation</span></span>

<span data-ttu-id="8ac91-227">Es folgt eine JSON-Darstellung einer **site**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="8ac91-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="8ac91-228">Die **site**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="8ac91-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->

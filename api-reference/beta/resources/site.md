---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Website
localization_priority: Priority
ms.openlocfilehash: fb91e9bada227f1a22cf862726ea0b6f658fe469
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871022"
---
# <a name="site-resource-type"></a><span data-ttu-id="fd8f9-102">Website-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd8f9-102">site resource type</span></span>

> <span data-ttu-id="fd8f9-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd8f9-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd8f9-105">Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="fd8f9-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="fd8f9-106">Methods</span></span>

| <span data-ttu-id="fd8f9-107">Methode</span><span class="sxs-lookup"><span data-stu-id="fd8f9-107">Method</span></span>                         | <span data-ttu-id="fd8f9-108">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="fd8f9-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="fd8f9-109">[Stammwebsite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-109">[Get root site][]</span></span>              | <span data-ttu-id="fd8f9-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="fd8f9-110">GET /sites/root</span></span>
| <span data-ttu-id="fd8f9-111">[Website abrufen][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-111">[Get site][]</span></span>                   | <span data-ttu-id="fd8f9-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="fd8f9-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="fd8f9-113">[Website nach Pfad abrufen][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-113">[Get site by path][]</span></span>           | <span data-ttu-id="fd8f9-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="fd8f9-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="fd8f9-115">[Website für eine Gruppe abrufen][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-115">[Get site for a group][]</span></span>       | <span data-ttu-id="fd8f9-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="fd8f9-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="fd8f9-117">[Abrufen von analytics][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-117">[Get analytics][]</span></span>              | <span data-ttu-id="fd8f9-118">GET/Sites / {Site-Id} / Analytics</span><span class="sxs-lookup"><span data-stu-id="fd8f9-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="fd8f9-119">[Abrufen von Aktivitäten nach Intervall][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-119">[Get activities by interval][]</span></span> | <span data-ttu-id="fd8f9-120">GET/Sites / {Site-Id} / GetActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="fd8f9-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="fd8f9-121">[Seiten auflisten][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-121">[List pages][]</span></span>                 | <span data-ttu-id="fd8f9-122">GET/Sites / {Site-Id} / pages</span><span class="sxs-lookup"><span data-stu-id="fd8f9-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="fd8f9-123">[Stamm Websites aufgelistet werden sollen][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-123">[List root sites][]</span></span>            | <span data-ttu-id="fd8f9-124">GET/Sites? Filter = Root Ne null & select = SiteCollection WebUrl</span><span class="sxs-lookup"><span data-stu-id="fd8f9-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="fd8f9-125">[Nach Websites suchen][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-125">[Search for sites][]</span></span>           | <span data-ttu-id="fd8f9-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="fd8f9-126">GET /sites?search={query}</span></span>

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


## <a name="properties"></a><span data-ttu-id="fd8f9-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd8f9-136">Properties</span></span>

| <span data-ttu-id="fd8f9-137">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="fd8f9-137">Property name</span></span>            | <span data-ttu-id="fd8f9-138">Typ</span><span class="sxs-lookup"><span data-stu-id="fd8f9-138">Type</span></span>               | <span data-ttu-id="fd8f9-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd8f9-139">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="fd8f9-140">**id**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-140">**id**</span></span>                   | <span data-ttu-id="fd8f9-141">string</span><span class="sxs-lookup"><span data-stu-id="fd8f9-141">string</span></span>             | <span data-ttu-id="fd8f9-p102">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="fd8f9-144">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-144">**createdDateTime**</span></span>      | <span data-ttu-id="fd8f9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd8f9-145">DateTimeOffset</span></span>     | <span data-ttu-id="fd8f9-p103">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p103">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="fd8f9-148">**description**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-148">**description**</span></span>          | <span data-ttu-id="fd8f9-149">string</span><span class="sxs-lookup"><span data-stu-id="fd8f9-149">string</span></span>             | <span data-ttu-id="fd8f9-150">Der beschreibende Text für die Website.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-150">The descriptive text for the site.</span></span>
| <span data-ttu-id="fd8f9-151">**eTag**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-151">**eTag**</span></span>                 | <span data-ttu-id="fd8f9-152">string</span><span class="sxs-lookup"><span data-stu-id="fd8f9-152">string</span></span>             | <span data-ttu-id="fd8f9-p104">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="fd8f9-155">**displayName**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-155">**displayName**</span></span>          | <span data-ttu-id="fd8f9-156">string</span><span class="sxs-lookup"><span data-stu-id="fd8f9-156">string</span></span>             | <span data-ttu-id="fd8f9-p105">Der vollständigen Titel für die Website. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p105">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="fd8f9-159">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-159">**lastModifiedDateTime**</span></span> | <span data-ttu-id="fd8f9-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd8f9-160">DateTimeOffset</span></span>     | <span data-ttu-id="fd8f9-p106">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p106">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="fd8f9-163">**name**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-163">**name**</span></span>                 | <span data-ttu-id="fd8f9-164">string</span><span class="sxs-lookup"><span data-stu-id="fd8f9-164">string</span></span>             | <span data-ttu-id="fd8f9-165">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-165">The name / title of the item.</span></span>
| <span data-ttu-id="fd8f9-166">**root**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-166">**root**</span></span>                 | <span data-ttu-id="fd8f9-167">[root][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-167">[root][]</span></span>           | <span data-ttu-id="fd8f9-p107">Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p107">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="fd8f9-170">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-170">**sharepointIds**</span></span>        | <span data-ttu-id="fd8f9-171">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-171">[sharepointIds][]</span></span>  | <span data-ttu-id="fd8f9-p108">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p108">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="fd8f9-174">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-174">**siteCollection**</span></span>       | <span data-ttu-id="fd8f9-175">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-175">[siteCollection][]</span></span> | <span data-ttu-id="fd8f9-p109">Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p109">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="fd8f9-179">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-179">**webUrl**</span></span>               | <span data-ttu-id="fd8f9-180">String (URL)</span><span class="sxs-lookup"><span data-stu-id="fd8f9-180">string (url)</span></span>       | <span data-ttu-id="fd8f9-p110">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="fd8f9-183">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fd8f9-183">Relationships</span></span>

| <span data-ttu-id="fd8f9-184">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="fd8f9-184">Relationship name</span></span> | <span data-ttu-id="fd8f9-185">Typ</span><span class="sxs-lookup"><span data-stu-id="fd8f9-185">Type</span></span>                             | <span data-ttu-id="fd8f9-186">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd8f9-186">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="fd8f9-187">**Analytics**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-187">**analytics**</span></span>     | <span data-ttu-id="fd8f9-188">[ItemAnalytics][] -Ressource</span><span class="sxs-lookup"><span data-stu-id="fd8f9-188">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="fd8f9-189">Analytics über die Aktivitäten anzeigen, die auf dieser Site durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-189">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="fd8f9-190">**columns**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-190">**columns**</span></span>       | <span data-ttu-id="fd8f9-191">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="fd8f9-191">Collection([columnDefinition][])</span></span> | <span data-ttu-id="fd8f9-192">Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-192">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="fd8f9-193">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-193">**contentTypes**</span></span>  | <span data-ttu-id="fd8f9-194">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="fd8f9-194">Collection([contentType][])</span></span>      | <span data-ttu-id="fd8f9-195">Die Sammlung von für diese Website definierten Inhaltstypen.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-195">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="fd8f9-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-196">**drive**</span></span>         | <span data-ttu-id="fd8f9-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="fd8f9-197">[drive][]</span></span>                        | <span data-ttu-id="fd8f9-198">Das Standardlaufwerk (Dokumentbibliothek) für diese Website.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-198">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="fd8f9-199">**drives**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-199">**drives**</span></span>        | <span data-ttu-id="fd8f9-200">Sammlung ([drive][])</span><span class="sxs-lookup"><span data-stu-id="fd8f9-200">Collection([drive][])</span></span>            | <span data-ttu-id="fd8f9-201">Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-201">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="fd8f9-202">**items**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-202">**items**</span></span>         | <span data-ttu-id="fd8f9-203">Sammlung ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="fd8f9-203">Collection([baseItem][])</span></span>         | <span data-ttu-id="fd8f9-p111">Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-p111">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="fd8f9-206">**Listen**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-206">**lists**</span></span>         | <span data-ttu-id="fd8f9-207">Sammlung ([Liste][])</span><span class="sxs-lookup"><span data-stu-id="fd8f9-207">Collection([list][])</span></span>             | <span data-ttu-id="fd8f9-208">Die Sammlung der Listen unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-208">The collection of lists under this site.</span></span>
| <span data-ttu-id="fd8f9-209">**Seiten**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-209">**pages**</span></span>         | <span data-ttu-id="fd8f9-210">Auflistung ([SitePage][])</span><span class="sxs-lookup"><span data-stu-id="fd8f9-210">Collection([sitePage][])</span></span>         | <span data-ttu-id="fd8f9-211">Die Auflistung von Seiten in der Liste SitePages auf dieser Site.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-211">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="fd8f9-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="fd8f9-212">**sites**</span></span>         | <span data-ttu-id="fd8f9-213">Sammlung ([site][])</span><span class="sxs-lookup"><span data-stu-id="fd8f9-213">Collection([site][])</span></span>             | <span data-ttu-id="fd8f9-214">Die Sammlung der Unterwebsites unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-214">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="fd8f9-226">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd8f9-226">JSON representation</span></span>

<span data-ttu-id="fd8f9-227">Es folgt eine JSON-Darstellung einer **site**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="fd8f9-228">Die **site**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd8f9-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

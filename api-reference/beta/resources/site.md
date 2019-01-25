---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 17b9b8731a2b4e4ce39fa2ee10535bcb302f1be3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514803"
---
# <a name="site-resource-type"></a><span data-ttu-id="1432e-102">Site-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1432e-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1432e-103">Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.</span><span class="sxs-lookup"><span data-stu-id="1432e-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="1432e-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="1432e-104">Methods</span></span>

| <span data-ttu-id="1432e-105">Method</span><span class="sxs-lookup"><span data-stu-id="1432e-105">Method</span></span>                         | <span data-ttu-id="1432e-106">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="1432e-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="1432e-107">[Stammwebsite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="1432e-107">[Get root site][]</span></span>              | <span data-ttu-id="1432e-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="1432e-108">GET /sites/root</span></span>
| <span data-ttu-id="1432e-109">[Website abrufen][]</span><span class="sxs-lookup"><span data-stu-id="1432e-109">[Get site][]</span></span>                   | <span data-ttu-id="1432e-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="1432e-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="1432e-111">[Website nach Pfad abrufen][]</span><span class="sxs-lookup"><span data-stu-id="1432e-111">[Get site by path][]</span></span>           | <span data-ttu-id="1432e-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="1432e-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="1432e-113">[Website für eine Gruppe abrufen][]</span><span class="sxs-lookup"><span data-stu-id="1432e-113">[Get site for a group][]</span></span>       | <span data-ttu-id="1432e-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="1432e-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="1432e-115">[Analysen abrufen][]</span><span class="sxs-lookup"><span data-stu-id="1432e-115">[Get analytics][]</span></span>              | <span data-ttu-id="1432e-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="1432e-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="1432e-117">[Aktivitäten nach Intervall abrufen][]</span><span class="sxs-lookup"><span data-stu-id="1432e-117">[Get activities by interval][]</span></span> | <span data-ttu-id="1432e-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="1432e-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="1432e-119">[Seiten auflisten][]</span><span class="sxs-lookup"><span data-stu-id="1432e-119">[List pages][]</span></span>                 | <span data-ttu-id="1432e-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="1432e-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="1432e-121">[Stammwebsites auflisten][]</span><span class="sxs-lookup"><span data-stu-id="1432e-121">[List root sites][]</span></span>            | <span data-ttu-id="1432e-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="1432e-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="1432e-123">[Nach Websites suchen][]</span><span class="sxs-lookup"><span data-stu-id="1432e-123">[Search for sites][]</span></span>           | <span data-ttu-id="1432e-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="1432e-124">GET /sites?search={query}</span></span>

[Website abrufen]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Stammwebsite abrufen]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Website nach Pfad abrufen]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Website für eine Gruppe abrufen]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Analysen abrufen]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Aktivitäten nach Intervall abrufen]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Seiten auflisten]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Stammwebsites auflisten]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[Nach Websites suchen]: ../api/site-search.md
[Search for sites]: ../api/site-search.md


## <a name="properties"></a><span data-ttu-id="1432e-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1432e-134">Properties</span></span>

| <span data-ttu-id="1432e-135">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="1432e-135">Property name</span></span>            | <span data-ttu-id="1432e-136">Typ</span><span class="sxs-lookup"><span data-stu-id="1432e-136">Type</span></span>               | <span data-ttu-id="1432e-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1432e-137">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="1432e-138">**id**</span><span class="sxs-lookup"><span data-stu-id="1432e-138">**id**</span></span>                   | <span data-ttu-id="1432e-139">string</span><span class="sxs-lookup"><span data-stu-id="1432e-139">string</span></span>             | <span data-ttu-id="1432e-p101">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p101">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="1432e-142">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="1432e-142">**createdDateTime**</span></span>      | <span data-ttu-id="1432e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1432e-143">DateTimeOffset</span></span>     | <span data-ttu-id="1432e-p102">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="1432e-146">**description**</span><span class="sxs-lookup"><span data-stu-id="1432e-146">**description**</span></span>          | <span data-ttu-id="1432e-147">string</span><span class="sxs-lookup"><span data-stu-id="1432e-147">string</span></span>             | <span data-ttu-id="1432e-148">Der beschreibende Text für die Website.</span><span class="sxs-lookup"><span data-stu-id="1432e-148">The descriptive text for the site.</span></span>
| <span data-ttu-id="1432e-149">**eTag**</span><span class="sxs-lookup"><span data-stu-id="1432e-149">**eTag**</span></span>                 | <span data-ttu-id="1432e-150">string</span><span class="sxs-lookup"><span data-stu-id="1432e-150">string</span></span>             | <span data-ttu-id="1432e-p103">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="1432e-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="1432e-153">**displayName**</span></span>          | <span data-ttu-id="1432e-154">string</span><span class="sxs-lookup"><span data-stu-id="1432e-154">string</span></span>             | <span data-ttu-id="1432e-p104">Der vollständigen Titel für die Website. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="1432e-157">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="1432e-157">**lastModifiedDateTime**</span></span> | <span data-ttu-id="1432e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1432e-158">DateTimeOffset</span></span>     | <span data-ttu-id="1432e-p105">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="1432e-161">**name**</span><span class="sxs-lookup"><span data-stu-id="1432e-161">**name**</span></span>                 | <span data-ttu-id="1432e-162">string</span><span class="sxs-lookup"><span data-stu-id="1432e-162">string</span></span>             | <span data-ttu-id="1432e-163">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="1432e-163">The name / title of the item.</span></span>
| <span data-ttu-id="1432e-164">**root**</span><span class="sxs-lookup"><span data-stu-id="1432e-164">**root**</span></span>                 | <span data-ttu-id="1432e-165">[root][]</span><span class="sxs-lookup"><span data-stu-id="1432e-165">[root][]</span></span>           | <span data-ttu-id="1432e-p106">Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="1432e-168">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="1432e-168">**sharepointIds**</span></span>        | <span data-ttu-id="1432e-169">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="1432e-169">[sharepointIds][]</span></span>  | <span data-ttu-id="1432e-p107">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="1432e-172">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="1432e-172">**siteCollection**</span></span>       | <span data-ttu-id="1432e-173">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="1432e-173">[siteCollection][]</span></span> | <span data-ttu-id="1432e-p108">Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="1432e-177">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="1432e-177">**webUrl**</span></span>               | <span data-ttu-id="1432e-178">String (URL)</span><span class="sxs-lookup"><span data-stu-id="1432e-178">string (url)</span></span>       | <span data-ttu-id="1432e-p109">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1432e-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="1432e-181">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1432e-181">Relationships</span></span>

| <span data-ttu-id="1432e-182">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="1432e-182">Relationship name</span></span> | <span data-ttu-id="1432e-183">Typ</span><span class="sxs-lookup"><span data-stu-id="1432e-183">Type</span></span>                             | <span data-ttu-id="1432e-184">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1432e-184">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="1432e-185">**analytics**</span><span class="sxs-lookup"><span data-stu-id="1432e-185">**analytics**</span></span>     | <span data-ttu-id="1432e-186">[itemAnalytics][]-Ressource</span><span class="sxs-lookup"><span data-stu-id="1432e-186">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="1432e-187">Analysen zu den Anzeigeaktivitäten, die auf dieser Website stattgefunden haben.</span><span class="sxs-lookup"><span data-stu-id="1432e-187">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="1432e-188">**columns**</span><span class="sxs-lookup"><span data-stu-id="1432e-188">**columns**</span></span>       | <span data-ttu-id="1432e-189">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="1432e-189">Collection([columnDefinition][])</span></span> | <span data-ttu-id="1432e-190">Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.</span><span class="sxs-lookup"><span data-stu-id="1432e-190">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="1432e-191">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="1432e-191">**contentTypes**</span></span>  | <span data-ttu-id="1432e-192">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="1432e-192">Collection([contentType][])</span></span>      | <span data-ttu-id="1432e-193">Die Sammlung von für diese Website definierten Inhaltstypen.</span><span class="sxs-lookup"><span data-stu-id="1432e-193">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="1432e-194">**drive**</span><span class="sxs-lookup"><span data-stu-id="1432e-194">**drive**</span></span>         | <span data-ttu-id="1432e-195">[drive][]</span><span class="sxs-lookup"><span data-stu-id="1432e-195">[drive][]</span></span>                        | <span data-ttu-id="1432e-196">Das Standardlaufwerk (Dokumentbibliothek) für diese Website.</span><span class="sxs-lookup"><span data-stu-id="1432e-196">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="1432e-197">**drives**</span><span class="sxs-lookup"><span data-stu-id="1432e-197">**drives**</span></span>        | <span data-ttu-id="1432e-198">Sammlung ([drive][])</span><span class="sxs-lookup"><span data-stu-id="1432e-198">Collection([drive][])</span></span>            | <span data-ttu-id="1432e-199">Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="1432e-199">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="1432e-200">**items**</span><span class="sxs-lookup"><span data-stu-id="1432e-200">**items**</span></span>         | <span data-ttu-id="1432e-201">Sammlung ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="1432e-201">Collection([baseItem][])</span></span>         | <span data-ttu-id="1432e-p110">Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="1432e-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="1432e-204">**Listen**</span><span class="sxs-lookup"><span data-stu-id="1432e-204">**lists**</span></span>         | <span data-ttu-id="1432e-205">Sammlung ([Liste][])</span><span class="sxs-lookup"><span data-stu-id="1432e-205">Collection([list][])</span></span>             | <span data-ttu-id="1432e-206">Die Sammlung der Listen unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="1432e-206">The collection of lists under this site.</span></span>
| <span data-ttu-id="1432e-207">**pages**</span><span class="sxs-lookup"><span data-stu-id="1432e-207">**pages**</span></span>         | <span data-ttu-id="1432e-208">Sammlung([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="1432e-208">Collection([sitePage][])</span></span>         | <span data-ttu-id="1432e-209">Die Sammlung von Seiten in der SitePages-Liste auf dieser Website.</span><span class="sxs-lookup"><span data-stu-id="1432e-209">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="1432e-210">**sites**</span><span class="sxs-lookup"><span data-stu-id="1432e-210">**sites**</span></span>         | <span data-ttu-id="1432e-211">Sammlung ([site][])</span><span class="sxs-lookup"><span data-stu-id="1432e-211">Collection([site][])</span></span>             | <span data-ttu-id="1432e-212">Die Sammlung der Unterwebsites unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="1432e-212">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="1432e-224">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1432e-224">JSON representation</span></span>

<span data-ttu-id="1432e-225">Es folgt eine JSON-Darstellung einer **site**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="1432e-225">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="1432e-226">Die **site**-Ressource wird von [ **baseItem**](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="1432e-226">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/site.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

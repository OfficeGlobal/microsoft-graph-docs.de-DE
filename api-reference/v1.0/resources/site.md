---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Website
ms.openlocfilehash: db465f93f336a51d862daf6e05b1d6bc422247ea
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="site-resource"></a><span data-ttu-id="b25b2-102">Site-Ressource</span><span class="sxs-lookup"><span data-stu-id="b25b2-102">Site resource</span></span>

<span data-ttu-id="b25b2-103">Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.</span><span class="sxs-lookup"><span data-stu-id="b25b2-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="b25b2-104">Aufgaben</span><span class="sxs-lookup"><span data-stu-id="b25b2-104">Tasks</span></span>

<span data-ttu-id="b25b2-105">Alle Beispiele unten beziehen sich auf `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="b25b2-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="b25b2-106">Aufgabenname</span><span class="sxs-lookup"><span data-stu-id="b25b2-106">Task name</span></span>                | <span data-ttu-id="b25b2-107">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="b25b2-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="b25b2-108">[Stammwebsite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="b25b2-108">[Get root site][]</span></span>        | <span data-ttu-id="b25b2-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="b25b2-109">GET /sites/root</span></span>
| <span data-ttu-id="b25b2-110">[Website abrufen][]</span><span class="sxs-lookup"><span data-stu-id="b25b2-110">[Get site][]</span></span>             | <span data-ttu-id="b25b2-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="b25b2-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="b25b2-112">[Website nach Pfad abrufen][]</span><span class="sxs-lookup"><span data-stu-id="b25b2-112">[Get site by path][]</span></span>     | <span data-ttu-id="b25b2-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="b25b2-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="b25b2-114">[Website für eine Gruppe abrufen][]</span><span class="sxs-lookup"><span data-stu-id="b25b2-114">[Get site for a group][]</span></span> | <span data-ttu-id="b25b2-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="b25b2-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="b25b2-116">[Nach Websites suchen][]</span><span class="sxs-lookup"><span data-stu-id="b25b2-116">[Search for sites][]</span></span>     | <span data-ttu-id="b25b2-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="b25b2-117">GET /sites?search={query}</span></span>

[Website abrufen]: ../api/site_get.md
[Stammwebsite abrufen]: ../api/site_get.md
[Website nach Pfad abrufen]: ../api/site_getbypath.md
[Website für eine Gruppe abrufen]: ../api/site_get.md
[Nach Websites suchen]: ../api/site_search.md

## <a name="json-representation"></a><span data-ttu-id="b25b2-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b25b2-123">JSON representation</span></span>

<span data-ttu-id="b25b2-124">Es folgt eine JSON-Darstellung einer **site**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="b25b2-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="b25b2-125">Die **driveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="b25b2-125">The **driveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource",
       "@odata.type": "microsoft.graph.site",
       "keyProperty": "id",
       "optionalProperties": [ "root", "sharepointIds", "siteCollection", "drive", "drives", "sites" ] } -->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "onenote": [ { "@odata.type": "microsoft.graph.onenote"} ],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="b25b2-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b25b2-126">Properties</span></span>

| <span data-ttu-id="b25b2-127">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="b25b2-127">Property name</span></span>            | <span data-ttu-id="b25b2-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b25b2-128">Type</span></span>                                | <span data-ttu-id="b25b2-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b25b2-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b25b2-130">**id**</span><span class="sxs-lookup"><span data-stu-id="b25b2-130">**id**</span></span>                   | <span data-ttu-id="b25b2-131">string</span><span class="sxs-lookup"><span data-stu-id="b25b2-131">string</span></span>                              | <span data-ttu-id="b25b2-p101">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="b25b2-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="b25b2-134">**createdDateTime**</span></span>      | <span data-ttu-id="b25b2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b25b2-135">DateTimeOffset</span></span>                      | <span data-ttu-id="b25b2-p102">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="b25b2-138">**description**</span><span class="sxs-lookup"><span data-stu-id="b25b2-138">**description**</span></span>          | <span data-ttu-id="b25b2-139">string</span><span class="sxs-lookup"><span data-stu-id="b25b2-139">string</span></span>                              | <span data-ttu-id="b25b2-140">Der beschreibende Text für die Website.</span><span class="sxs-lookup"><span data-stu-id="b25b2-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="b25b2-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="b25b2-141">**displayName**</span></span>          | <span data-ttu-id="b25b2-142">string</span><span class="sxs-lookup"><span data-stu-id="b25b2-142">string</span></span>                              | <span data-ttu-id="b25b2-p103">Der vollständigen Titel für die Website. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="b25b2-145">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b25b2-145">**lastModifiedDateTime**</span></span> | <span data-ttu-id="b25b2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b25b2-146">DateTimeOffset</span></span>                      | <span data-ttu-id="b25b2-p104">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p104">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="b25b2-149">**name**</span><span class="sxs-lookup"><span data-stu-id="b25b2-149">**name**</span></span>                 | <span data-ttu-id="b25b2-150">string</span><span class="sxs-lookup"><span data-stu-id="b25b2-150">string</span></span>                              | <span data-ttu-id="b25b2-151">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="b25b2-151">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="b25b2-152">**root**</span><span class="sxs-lookup"><span data-stu-id="b25b2-152">**root**</span></span>                 | [<span data-ttu-id="b25b2-153">root</span><span class="sxs-lookup"><span data-stu-id="b25b2-153">root</span></span>](root.md)                     | <span data-ttu-id="b25b2-p105">Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p105">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="b25b2-156">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="b25b2-156">**sharepointIds**</span></span>        | [<span data-ttu-id="b25b2-157">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b25b2-157">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="b25b2-p106">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="b25b2-160">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="b25b2-160">**siteCollection**</span></span>       | [<span data-ttu-id="b25b2-161">siteCollection</span><span class="sxs-lookup"><span data-stu-id="b25b2-161">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="b25b2-p107">Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p107">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="b25b2-165">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="b25b2-165">**webUrl**</span></span>               | <span data-ttu-id="b25b2-166">String (URL)</span><span class="sxs-lookup"><span data-stu-id="b25b2-166">string (url)</span></span>                        | <span data-ttu-id="b25b2-p108">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p108">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="b25b2-169">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b25b2-169">Relationships</span></span>

| <span data-ttu-id="b25b2-170">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="b25b2-170">Relationship name</span></span> | <span data-ttu-id="b25b2-171">Typ</span><span class="sxs-lookup"><span data-stu-id="b25b2-171">Type</span></span>                             | <span data-ttu-id="b25b2-172">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b25b2-172">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="b25b2-173">**columns**</span><span class="sxs-lookup"><span data-stu-id="b25b2-173">**columns**</span></span>       | <span data-ttu-id="b25b2-174">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="b25b2-174">Collection([columnDefinition][])</span></span> | <span data-ttu-id="b25b2-175">Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.</span><span class="sxs-lookup"><span data-stu-id="b25b2-175">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="b25b2-176">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="b25b2-176">**contentTypes**</span></span>  | <span data-ttu-id="b25b2-177">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="b25b2-177">Collection([contentType][])</span></span>      | <span data-ttu-id="b25b2-178">Die Sammlung von für diese Website definierten Inhaltstypen.</span><span class="sxs-lookup"><span data-stu-id="b25b2-178">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="b25b2-179">**drive**</span><span class="sxs-lookup"><span data-stu-id="b25b2-179">**drive**</span></span>         | <span data-ttu-id="b25b2-180">[drive][]</span><span class="sxs-lookup"><span data-stu-id="b25b2-180">[drive][]</span></span>                        | <span data-ttu-id="b25b2-181">Das Standardlaufwerk (Dokumentbibliothek) für diese Website.</span><span class="sxs-lookup"><span data-stu-id="b25b2-181">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="b25b2-182">**drives**</span><span class="sxs-lookup"><span data-stu-id="b25b2-182">**drives**</span></span>        | <span data-ttu-id="b25b2-183">Sammlung ([drive][])</span><span class="sxs-lookup"><span data-stu-id="b25b2-183">Collection([drive][])</span></span>            | <span data-ttu-id="b25b2-184">Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="b25b2-184">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="b25b2-185">**items**</span><span class="sxs-lookup"><span data-stu-id="b25b2-185">**items**</span></span>         | <span data-ttu-id="b25b2-186">Sammlung ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="b25b2-186">Collection([baseItem][])</span></span>         | <span data-ttu-id="b25b2-p109">Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="b25b2-p109">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="b25b2-189">**lists**</span><span class="sxs-lookup"><span data-stu-id="b25b2-189">**Lists**</span></span>         | <span data-ttu-id="b25b2-190">Sammlung ([list][])</span><span class="sxs-lookup"><span data-stu-id="b25b2-190">Collection([list][])</span></span>             | <span data-ttu-id="b25b2-191">Die Sammlung der Listen unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="b25b2-191">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="b25b2-192">**sites**</span><span class="sxs-lookup"><span data-stu-id="b25b2-192">**sites**</span></span>         | <span data-ttu-id="b25b2-193">Sammlung ([site][])</span><span class="sxs-lookup"><span data-stu-id="b25b2-193">Collection([site][])</span></span>             | <span data-ttu-id="b25b2-194">Die Sammlung der Unterwebsites unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="b25b2-194">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="b25b2-195">**onenote**</span><span class="sxs-lookup"><span data-stu-id="b25b2-195">**onenote**</span></span>       | <span data-ttu-id="b25b2-196">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="b25b2-196">[onenote][]</span></span>                      | <span data-ttu-id="b25b2-197">Ruft den OneNote-Dienst für Notizbuchvorgänge auf.</span><span class="sxs-lookup"><span data-stu-id="b25b2-197">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->

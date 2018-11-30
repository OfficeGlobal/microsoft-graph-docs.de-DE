---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Website
ms.openlocfilehash: ae8962dfa38c3c6f3e06ccb687eb42a4a8262f1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020120"
---
# <a name="site-resource"></a><span data-ttu-id="69966-102">Site-Ressource</span><span class="sxs-lookup"><span data-stu-id="69966-102">Site resource</span></span>

<span data-ttu-id="69966-103">Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.</span><span class="sxs-lookup"><span data-stu-id="69966-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="69966-104">Aufgaben</span><span class="sxs-lookup"><span data-stu-id="69966-104">Tasks</span></span>

<span data-ttu-id="69966-105">Alle Beispiele unten beziehen sich auf `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="69966-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="69966-106">Aufgabenname</span><span class="sxs-lookup"><span data-stu-id="69966-106">Task name</span></span>                | <span data-ttu-id="69966-107">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="69966-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="69966-108">[Stammwebsite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="69966-108">[Get root site][]</span></span>        | <span data-ttu-id="69966-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="69966-109">GET /sites/root</span></span>
| <span data-ttu-id="69966-110">[Website abrufen][]</span><span class="sxs-lookup"><span data-stu-id="69966-110">[Get site][]</span></span>             | <span data-ttu-id="69966-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="69966-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="69966-112">[Website nach Pfad abrufen][]</span><span class="sxs-lookup"><span data-stu-id="69966-112">[Get site by path][]</span></span>     | <span data-ttu-id="69966-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="69966-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="69966-114">[Website für eine Gruppe abrufen][]</span><span class="sxs-lookup"><span data-stu-id="69966-114">[Get site for a group][]</span></span> | <span data-ttu-id="69966-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="69966-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="69966-116">[Nach Websites suchen][]</span><span class="sxs-lookup"><span data-stu-id="69966-116">[Search for sites][]</span></span>     | <span data-ttu-id="69966-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="69966-117">GET /sites?search={query}</span></span>

[Website abrufen]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Stammwebsite abrufen]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Website nach Pfad abrufen]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Website für eine Gruppe abrufen]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Nach Websites suchen]: ../api/site-search.md
[Search for sites]: ../api/site-search.md

## <a name="json-representation"></a><span data-ttu-id="69966-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69966-123">JSON representation</span></span>

<span data-ttu-id="69966-124">Es folgt eine JSON-Darstellung einer **site**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="69966-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="69966-125">Die **site**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="69966-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="69966-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69966-126">Properties</span></span>

| <span data-ttu-id="69966-127">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="69966-127">Property name</span></span>            | <span data-ttu-id="69966-128">Typ</span><span class="sxs-lookup"><span data-stu-id="69966-128">Type</span></span>                                | <span data-ttu-id="69966-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69966-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="69966-130">**id**</span><span class="sxs-lookup"><span data-stu-id="69966-130">**id**</span></span>                   | <span data-ttu-id="69966-131">string</span><span class="sxs-lookup"><span data-stu-id="69966-131">string</span></span>                              | <span data-ttu-id="69966-p101">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="69966-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="69966-134">**createdDateTime**</span></span>      | <span data-ttu-id="69966-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69966-135">DateTimeOffset</span></span>                      | <span data-ttu-id="69966-p102">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="69966-138">**description**</span><span class="sxs-lookup"><span data-stu-id="69966-138">**description**</span></span>          | <span data-ttu-id="69966-139">string</span><span class="sxs-lookup"><span data-stu-id="69966-139">string</span></span>                              | <span data-ttu-id="69966-140">Der beschreibende Text für die Website.</span><span class="sxs-lookup"><span data-stu-id="69966-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="69966-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="69966-141">**displayName**</span></span>          | <span data-ttu-id="69966-142">string</span><span class="sxs-lookup"><span data-stu-id="69966-142">string</span></span>                              | <span data-ttu-id="69966-p103">Der vollständigen Titel für die Website. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="69966-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="69966-145">**eTag**</span></span>                 | <span data-ttu-id="69966-146">string</span><span class="sxs-lookup"><span data-stu-id="69966-146">string</span></span>                              | <span data-ttu-id="69966-p104">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="69966-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="69966-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="69966-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69966-150">DateTimeOffset</span></span>                      | <span data-ttu-id="69966-p105">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="69966-153">**name**</span><span class="sxs-lookup"><span data-stu-id="69966-153">**name**</span></span>                 | <span data-ttu-id="69966-154">string</span><span class="sxs-lookup"><span data-stu-id="69966-154">string</span></span>                              | <span data-ttu-id="69966-155">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="69966-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="69966-156">**root**</span><span class="sxs-lookup"><span data-stu-id="69966-156">**root**</span></span>                 | [<span data-ttu-id="69966-157">root</span><span class="sxs-lookup"><span data-stu-id="69966-157">root</span></span>](root.md)                     | <span data-ttu-id="69966-p106">Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="69966-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="69966-160">**sharepointIds**</span></span>        | [<span data-ttu-id="69966-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="69966-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="69966-p107">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="69966-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="69966-164">**siteCollection**</span></span>       | [<span data-ttu-id="69966-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="69966-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="69966-p108">Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="69966-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="69966-169">**webUrl**</span></span>               | <span data-ttu-id="69966-170">String (URL)</span><span class="sxs-lookup"><span data-stu-id="69966-170">string (url)</span></span>                        | <span data-ttu-id="69966-p109">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="69966-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="69966-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69966-173">Relationships</span></span>

| <span data-ttu-id="69966-174">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="69966-174">Relationship name</span></span> | <span data-ttu-id="69966-175">Typ</span><span class="sxs-lookup"><span data-stu-id="69966-175">Type</span></span>                             | <span data-ttu-id="69966-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69966-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="69966-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="69966-177">**columns**</span></span>       | <span data-ttu-id="69966-178">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="69966-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="69966-179">Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.</span><span class="sxs-lookup"><span data-stu-id="69966-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="69966-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="69966-180">**contentTypes**</span></span>  | <span data-ttu-id="69966-181">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="69966-181">Collection([contentType][])</span></span>      | <span data-ttu-id="69966-182">Die Sammlung von für diese Website definierten Inhaltstypen.</span><span class="sxs-lookup"><span data-stu-id="69966-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="69966-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="69966-183">**drive**</span></span>         | <span data-ttu-id="69966-184">[drive][]</span><span class="sxs-lookup"><span data-stu-id="69966-184">[drive][]</span></span>                        | <span data-ttu-id="69966-185">Das Standardlaufwerk (Dokumentbibliothek) für diese Website.</span><span class="sxs-lookup"><span data-stu-id="69966-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="69966-186">**drives**</span><span class="sxs-lookup"><span data-stu-id="69966-186">**drives**</span></span>        | <span data-ttu-id="69966-187">Sammlung ([drive][])</span><span class="sxs-lookup"><span data-stu-id="69966-187">Collection([drive][])</span></span>            | <span data-ttu-id="69966-188">Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="69966-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="69966-189">**items**</span><span class="sxs-lookup"><span data-stu-id="69966-189">**items**</span></span>         | <span data-ttu-id="69966-190">Sammlung ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="69966-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="69966-p110">Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="69966-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="69966-193">**Listen**</span><span class="sxs-lookup"><span data-stu-id="69966-193">**lists**</span></span>         | <span data-ttu-id="69966-194">Sammlung ([Liste][])</span><span class="sxs-lookup"><span data-stu-id="69966-194">Collection([list][])</span></span>             | <span data-ttu-id="69966-195">Die Sammlung der Listen unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="69966-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="69966-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="69966-196">**sites**</span></span>         | <span data-ttu-id="69966-197">Sammlung ([site][])</span><span class="sxs-lookup"><span data-stu-id="69966-197">Collection([site][])</span></span>             | <span data-ttu-id="69966-198">Die Sammlung der Unterwebsites unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="69966-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="69966-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="69966-199">**onenote**</span></span>       | <span data-ttu-id="69966-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="69966-200">[onenote][]</span></span>                      | <span data-ttu-id="69966-201">Ruft den OneNote-Dienst für Notizbuchvorgänge auf.</span><span class="sxs-lookup"><span data-stu-id="69966-201">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
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

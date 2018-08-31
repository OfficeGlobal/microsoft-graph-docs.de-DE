---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Website
ms.openlocfilehash: 20d31a9cdc0e540c2b2f2d93fedabdc254e9c03e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265715"
---
# <a name="site-resource"></a><span data-ttu-id="01074-102">Site-Ressource</span><span class="sxs-lookup"><span data-stu-id="01074-102">Site resource</span></span>

<span data-ttu-id="01074-103">Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.</span><span class="sxs-lookup"><span data-stu-id="01074-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="01074-104">Aufgaben</span><span class="sxs-lookup"><span data-stu-id="01074-104">Tasks</span></span>

<span data-ttu-id="01074-105">Alle Beispiele unten beziehen sich auf `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="01074-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="01074-106">Aufgabenname</span><span class="sxs-lookup"><span data-stu-id="01074-106">Task name</span></span>                | <span data-ttu-id="01074-107">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="01074-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="01074-108">[Stammwebsite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="01074-108">[Get root site][]</span></span>        | <span data-ttu-id="01074-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="01074-109">GET /sites/root</span></span>
| <span data-ttu-id="01074-110">[Website abrufen][]</span><span class="sxs-lookup"><span data-stu-id="01074-110">[Get site][]</span></span>             | <span data-ttu-id="01074-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="01074-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="01074-112">[Website nach Pfad abrufen][]</span><span class="sxs-lookup"><span data-stu-id="01074-112">[Get site by path][]</span></span>     | <span data-ttu-id="01074-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="01074-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="01074-114">[Website für eine Gruppe abrufen][]</span><span class="sxs-lookup"><span data-stu-id="01074-114">[Get site for a group][]</span></span> | <span data-ttu-id="01074-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="01074-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="01074-116">[Nach Websites suchen][]</span><span class="sxs-lookup"><span data-stu-id="01074-116">[Search for sites][]</span></span>     | <span data-ttu-id="01074-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="01074-117">GET /sites?search={query}</span></span>

[Website abrufen]: ../api/site_get.md
[Get site]: ../api/site_get.md
[Stammwebsite abrufen]: ../api/site_get.md
[Get root site]: ../api/site_get.md
[Website nach Pfad abrufen]: ../api/site_getbypath.md
[Get site by path]: ../api/site_getbypath.md
[Website für eine Gruppe abrufen]: ../api/site_get.md
[Get site for a group]: ../api/site_get.md
[Nach Websites suchen]: ../api/site_search.md
[Search for sites]: ../api/site_search.md

## <a name="json-representation"></a><span data-ttu-id="01074-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="01074-123">JSON representation</span></span>

<span data-ttu-id="01074-124">Es folgt eine JSON-Darstellung einer **site**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="01074-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="01074-125">Die **site**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="01074-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="01074-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="01074-126">Properties</span></span>

| <span data-ttu-id="01074-127">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="01074-127">Property name</span></span>            | <span data-ttu-id="01074-128">Typ</span><span class="sxs-lookup"><span data-stu-id="01074-128">Type</span></span>                                | <span data-ttu-id="01074-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01074-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="01074-130">**ID**</span><span class="sxs-lookup"><span data-stu-id="01074-130">**id**</span></span>                   | <span data-ttu-id="01074-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01074-131">string</span></span>                              | <span data-ttu-id="01074-p101">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="01074-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="01074-134">**createdDateTime**</span></span>      | <span data-ttu-id="01074-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01074-135">DateTimeOffset</span></span>                      | <span data-ttu-id="01074-p102">Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="01074-138">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="01074-138">**description**</span></span>          | <span data-ttu-id="01074-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01074-139">string</span></span>                              | <span data-ttu-id="01074-140">Der beschreibende Text für die Website.</span><span class="sxs-lookup"><span data-stu-id="01074-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="01074-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="01074-141">**displayName**</span></span>          | <span data-ttu-id="01074-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01074-142">string</span></span>                              | <span data-ttu-id="01074-p103">Der vollständigen Titel für die Website. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="01074-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="01074-145">**eTag**</span></span>                 | <span data-ttu-id="01074-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01074-146">string</span></span>                              | <span data-ttu-id="01074-p104">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="01074-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="01074-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="01074-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01074-150">DateTimeOffset</span></span>                      | <span data-ttu-id="01074-p105">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="01074-153">**Name**</span><span class="sxs-lookup"><span data-stu-id="01074-153">**name**</span></span>                 | <span data-ttu-id="01074-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01074-154">string</span></span>                              | <span data-ttu-id="01074-155">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="01074-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="01074-156">**Stamm**</span><span class="sxs-lookup"><span data-stu-id="01074-156">**root**</span></span>                 | [<span data-ttu-id="01074-157">Stamm</span><span class="sxs-lookup"><span data-stu-id="01074-157">root</span></span>](root.md)                     | <span data-ttu-id="01074-p106">Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="01074-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="01074-160">**sharepointIds**</span></span>        | [<span data-ttu-id="01074-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="01074-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="01074-p107">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="01074-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="01074-164">**siteCollection**</span></span>       | [<span data-ttu-id="01074-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="01074-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="01074-p108">Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="01074-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="01074-169">**webUrl**</span></span>               | <span data-ttu-id="01074-170">String (URL)</span><span class="sxs-lookup"><span data-stu-id="01074-170">string (url)</span></span>                        | <span data-ttu-id="01074-p109">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="01074-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="01074-173">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="01074-173">Relationships</span></span>

| <span data-ttu-id="01074-174">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="01074-174">Relationship name</span></span> | <span data-ttu-id="01074-175">Typ</span><span class="sxs-lookup"><span data-stu-id="01074-175">Type</span></span>                             | <span data-ttu-id="01074-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01074-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="01074-177">**Spalten**</span><span class="sxs-lookup"><span data-stu-id="01074-177">**columns**</span></span>       | <span data-ttu-id="01074-178">Sammlung ([ColumnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="01074-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="01074-179">Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.</span><span class="sxs-lookup"><span data-stu-id="01074-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="01074-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="01074-180">**contentTypes**</span></span>  | <span data-ttu-id="01074-181">Sammlung ([contentType][])</span><span class="sxs-lookup"><span data-stu-id="01074-181">Collection([contentType][])</span></span>      | <span data-ttu-id="01074-182">Die Sammlung von für diese Website definierten Inhaltstypen.</span><span class="sxs-lookup"><span data-stu-id="01074-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="01074-183">**Laufwerk**</span><span class="sxs-lookup"><span data-stu-id="01074-183">**drive**</span></span>         | <span data-ttu-id="01074-184">[Laufwerk][]</span><span class="sxs-lookup"><span data-stu-id="01074-184">[drive][]</span></span>                        | <span data-ttu-id="01074-185">Das Standardlaufwerk (Dokumentbibliothek) für diese Website.</span><span class="sxs-lookup"><span data-stu-id="01074-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="01074-186">**Laufwerke**</span><span class="sxs-lookup"><span data-stu-id="01074-186">**drives**</span></span>        | <span data-ttu-id="01074-187">Sammlung ([drive][])</span><span class="sxs-lookup"><span data-stu-id="01074-187">Collection([drive][])</span></span>            | <span data-ttu-id="01074-188">Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="01074-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="01074-189">**Elemente**</span><span class="sxs-lookup"><span data-stu-id="01074-189">**items**</span></span>         | <span data-ttu-id="01074-190">Sammlung ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="01074-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="01074-p110">Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="01074-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="01074-193">**Listen**</span><span class="sxs-lookup"><span data-stu-id="01074-193">**lists**</span></span>         | <span data-ttu-id="01074-194">Sammlung ([Liste][])</span><span class="sxs-lookup"><span data-stu-id="01074-194">Collection([list][])</span></span>             | <span data-ttu-id="01074-195">Die Sammlung der Listen unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="01074-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="01074-196">**Sites**</span><span class="sxs-lookup"><span data-stu-id="01074-196">**sites**</span></span>         | <span data-ttu-id="01074-197">Sammlung ([site][])</span><span class="sxs-lookup"><span data-stu-id="01074-197">Collection([site][])</span></span>             | <span data-ttu-id="01074-198">Die Sammlung der Unterwebsites unter dieser Website.</span><span class="sxs-lookup"><span data-stu-id="01074-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="01074-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="01074-199">**onenote**</span></span>       | <span data-ttu-id="01074-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="01074-200">[onenote][]</span></span>                      | <span data-ttu-id="01074-201">Ruft den OneNote-Dienst für Notizbuchvorgänge auf.</span><span class="sxs-lookup"><span data-stu-id="01074-201">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
[Laufwerk]: drive.md
[drive]: drive.md
[identitySet]: identityset.md
[Liste]: list.md
[list]: list.md
[Site]: site.md
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

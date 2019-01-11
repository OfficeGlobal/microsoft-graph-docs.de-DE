---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.openlocfilehash: d4673138106e23afedb5ff0f28d8ce72fa2797b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871491"
---
# <a name="sitepage-resource"></a><span data-ttu-id="da228-102">SitePage-Ressource</span><span class="sxs-lookup"><span data-stu-id="da228-102">sitePage resource</span></span>

> <span data-ttu-id="da228-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="da228-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da228-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da228-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da228-105">Diese Ressource stellt eine Seite in der SitePages [Liste][]dar.</span><span class="sxs-lookup"><span data-stu-id="da228-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="da228-106">Sie enthält den Titel, Layout und eine Auflistung von [WebPart][]s.</span><span class="sxs-lookup"><span data-stu-id="da228-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="da228-107">Aufgaben auf einer Seite</span><span class="sxs-lookup"><span data-stu-id="da228-107">Tasks on a page</span></span>

<span data-ttu-id="da228-108">Die folgenden Aufgaben sind für **SitePage** Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="da228-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="da228-109">Alle unten stehenden Beispiele sind relativ zu einer [Website][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="da228-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="da228-110">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="da228-110">Common task</span></span>                     | <span data-ttu-id="da228-111">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="da228-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="da228-112">[Seiten auflisten][]</span><span class="sxs-lookup"><span data-stu-id="da228-112">[List pages][]</span></span>                  | <span data-ttu-id="da228-113">Abrufen von /pages</span><span class="sxs-lookup"><span data-stu-id="da228-113">GET /pages</span></span>
| <span data-ttu-id="da228-114">[Seite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="da228-114">[Get page][]</span></span>                    | <span data-ttu-id="da228-115">Abrufen von /pages/ {Seiten-Id}</span><span class="sxs-lookup"><span data-stu-id="da228-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="da228-116">[Create][]</span><span class="sxs-lookup"><span data-stu-id="da228-116">[Create][]</span></span>                      | <span data-ttu-id="da228-117">POST-/pages</span><span class="sxs-lookup"><span data-stu-id="da228-117">POST /pages</span></span>
| <span data-ttu-id="da228-118">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="da228-118">[Delete][]</span></span>                      | <span data-ttu-id="da228-119">Löschen von /pages/ {Seiten-Id}</span><span class="sxs-lookup"><span data-stu-id="da228-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="da228-120">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="da228-120">[Publish][]</span></span>                     | <span data-ttu-id="da228-121">Posten Sie /pages/ {Seiten-Id} / veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="da228-121">POST /pages/{page-id}/publish</span></span>

[Seiten auflisten]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Seite abrufen]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="da228-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da228-127">JSON representation</span></span>

<span data-ttu-id="da228-128">Es folgt eine JSON-Darstellung einer **SitePage** Ressource.</span><span class="sxs-lookup"><span data-stu-id="da228-128">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="da228-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da228-129">Properties</span></span>

<span data-ttu-id="da228-130">Die Ressource **SitePage** hat die folgenden Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="da228-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="da228-131">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="da228-131">Property name</span></span>    | <span data-ttu-id="da228-132">Typ</span><span class="sxs-lookup"><span data-stu-id="da228-132">Type</span></span>                         | <span data-ttu-id="da228-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da228-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="da228-134">contentType</span><span class="sxs-lookup"><span data-stu-id="da228-134">contentType</span></span>      | <span data-ttu-id="da228-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="da228-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="da228-136">Der Inhaltstyp der Seite.</span><span class="sxs-lookup"><span data-stu-id="da228-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="da228-137">Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="da228-137">Page Content</span></span>

<span data-ttu-id="da228-138">Die Ressource **SitePage** hat die folgenden Felder Content.</span><span class="sxs-lookup"><span data-stu-id="da228-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="da228-139">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="da228-139">Property name</span></span>      | <span data-ttu-id="da228-140">Typ</span><span class="sxs-lookup"><span data-stu-id="da228-140">Type</span></span>                       | <span data-ttu-id="da228-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da228-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="da228-142">title</span><span class="sxs-lookup"><span data-stu-id="da228-142">title</span></span>              | <span data-ttu-id="da228-143">string</span><span class="sxs-lookup"><span data-stu-id="da228-143">string</span></span>                     | <span data-ttu-id="da228-144">Der Titel der Seite.</span><span class="sxs-lookup"><span data-stu-id="da228-144">The title of the page.</span></span>
| <span data-ttu-id="da228-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="da228-145">pageLayout</span></span>         | <span data-ttu-id="da228-146">string</span><span class="sxs-lookup"><span data-stu-id="da228-146">string</span></span>                     | <span data-ttu-id="da228-147">Der Name des auf der Seite auf das Seitenlayout.</span><span class="sxs-lookup"><span data-stu-id="da228-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="da228-148">webParts</span><span class="sxs-lookup"><span data-stu-id="da228-148">webParts</span></span>           | <span data-ttu-id="da228-149">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="da228-149">[webPart][]</span></span>                | <span data-ttu-id="da228-150">Die Webparts auf der Seite.</span><span class="sxs-lookup"><span data-stu-id="da228-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="da228-151">Erstellen von Metadaten</span><span class="sxs-lookup"><span data-stu-id="da228-151">Authoring Metadata</span></span>

<span data-ttu-id="da228-152">Die Ressource **SitePage** hat die folgende authoring-bezogenen Metadaten.</span><span class="sxs-lookup"><span data-stu-id="da228-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="da228-153">Die PublishingState-Eigenschaft wird die Seite Status wie ausgecheckt oder veröffentlicht authoring widerspiegeln.</span><span class="sxs-lookup"><span data-stu-id="da228-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="da228-154">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="da228-154">Property name</span></span>          | <span data-ttu-id="da228-155">Typ</span><span class="sxs-lookup"><span data-stu-id="da228-155">Type</span></span>                   | <span data-ttu-id="da228-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da228-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="da228-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="da228-157">publishingState</span></span>        | <span data-ttu-id="da228-158">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="da228-158">[publicationFacet][]</span></span>   | <span data-ttu-id="da228-159">Den Veröffentlichungsstatus und die MM.mm Version der Seite.</span><span class="sxs-lookup"><span data-stu-id="da228-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="da228-160">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="da228-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="da228-161">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="da228-161">Property name</span></span>        | <span data-ttu-id="da228-162">Typ</span><span class="sxs-lookup"><span data-stu-id="da228-162">Type</span></span>              | <span data-ttu-id="da228-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da228-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="da228-164">id</span><span class="sxs-lookup"><span data-stu-id="da228-164">id</span></span>                   | <span data-ttu-id="da228-165">string</span><span class="sxs-lookup"><span data-stu-id="da228-165">string</span></span>            | <span data-ttu-id="da228-p105">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da228-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="da228-168">name</span><span class="sxs-lookup"><span data-stu-id="da228-168">name</span></span>                 | <span data-ttu-id="da228-169">string</span><span class="sxs-lookup"><span data-stu-id="da228-169">string</span></span>            | <span data-ttu-id="da228-170">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="da228-170">The name / title of the item.</span></span>
| <span data-ttu-id="da228-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="da228-171">createdBy</span></span>            | <span data-ttu-id="da228-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="da228-172">[identitySet][]</span></span>   | <span data-ttu-id="da228-173">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="da228-173">Identity of the creator of this item.</span></span> <span data-ttu-id="da228-174">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da228-174">Read-only.</span></span>
| <span data-ttu-id="da228-175">eTag</span><span class="sxs-lookup"><span data-stu-id="da228-175">eTag</span></span>                 | <span data-ttu-id="da228-176">string</span><span class="sxs-lookup"><span data-stu-id="da228-176">string</span></span>            | <span data-ttu-id="da228-p107">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da228-p107">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="da228-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="da228-179">lastModifiedBy</span></span>       | <span data-ttu-id="da228-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="da228-180">[identitySet][]</span></span>   | <span data-ttu-id="da228-181">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="da228-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="da228-182">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da228-182">Read-only.</span></span>
| <span data-ttu-id="da228-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da228-183">lastModifiedDateTime</span></span> | <span data-ttu-id="da228-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da228-184">DateTimeOffset</span></span>    | <span data-ttu-id="da228-p109">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da228-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="da228-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="da228-187">parentReference</span></span>      | <span data-ttu-id="da228-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="da228-188">[itemReference][]</span></span> | <span data-ttu-id="da228-p110">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da228-p110">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="da228-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="da228-191">webUrl</span></span>               | <span data-ttu-id="da228-192">String (URL)</span><span class="sxs-lookup"><span data-stu-id="da228-192">string (url)</span></span>      | <span data-ttu-id="da228-p111">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da228-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="da228-195">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="da228-195">Relationships</span></span>

<span data-ttu-id="da228-196">Die Ressource **SitePage** hat keine Beziehung zu anderen Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="da228-196">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[Website]: site.md
[site]: site.md
[webPart]: webpart.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  }
} -->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->

---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: sitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522301"
---
# <a name="sitepage-resource"></a><span data-ttu-id="6ee1d-102">SitePage-Ressource</span><span class="sxs-lookup"><span data-stu-id="6ee1d-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ee1d-103">Diese Ressource stellt eine Seite in der SitePages [Liste][]dar.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="6ee1d-104">Sie enthält den Titel, Layout und eine Auflistung von [WebPart][]s.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="6ee1d-105">Aufgaben auf einer Seite</span><span class="sxs-lookup"><span data-stu-id="6ee1d-105">Tasks on a page</span></span>

<span data-ttu-id="6ee1d-106">Die folgenden Aufgaben sind für **SitePage** Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="6ee1d-107">Alle Beispiele unten beziehen sich auf  eine Website, z. B.: [][].</span><span class="sxs-lookup"><span data-stu-id="6ee1d-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="6ee1d-108">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="6ee1d-108">Common task</span></span>                     | <span data-ttu-id="6ee1d-109">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="6ee1d-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="6ee1d-110">[Seiten auflisten][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-110">[List pages][]</span></span>                  | <span data-ttu-id="6ee1d-111">GET Pages</span><span class="sxs-lookup"><span data-stu-id="6ee1d-111">GET /pages</span></span>
| <span data-ttu-id="6ee1d-112">[Seite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-112">[Get page][]</span></span>                    | <span data-ttu-id="6ee1d-113">Abrufen von /pages/ {Seiten-Id}</span><span class="sxs-lookup"><span data-stu-id="6ee1d-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="6ee1d-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-114">[Create][]</span></span>                      | <span data-ttu-id="6ee1d-115">POST Seiten</span><span class="sxs-lookup"><span data-stu-id="6ee1d-115">POST /pages</span></span>
| <span data-ttu-id="6ee1d-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-116">[Delete][]</span></span>                      | <span data-ttu-id="6ee1d-117">Löschen von /pages/ {Seiten-Id}</span><span class="sxs-lookup"><span data-stu-id="6ee1d-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="6ee1d-118">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-118">[Publish][]</span></span>                     | <span data-ttu-id="6ee1d-119">Posten Sie /pages/ {Seiten-Id} / veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="6ee1d-119">POST /pages/{page-id}/publish</span></span>

[Seiten auflisten]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Seite abrufen]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="6ee1d-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ee1d-125">JSON representation</span></span>

<span data-ttu-id="6ee1d-126">Es folgt eine JSON-Darstellung einer **SitePage** Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6ee1d-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ee1d-127">Properties</span></span>

<span data-ttu-id="6ee1d-128">Die Ressource **SitePage** hat die folgenden Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="6ee1d-129">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="6ee1d-129">Property name</span></span>    | <span data-ttu-id="6ee1d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6ee1d-130">Type</span></span>                         | <span data-ttu-id="6ee1d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ee1d-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="6ee1d-132">contentType</span><span class="sxs-lookup"><span data-stu-id="6ee1d-132">contentType</span></span>      | <span data-ttu-id="6ee1d-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="6ee1d-134">Der Inhaltstyp der Seite.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="6ee1d-135">Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="6ee1d-135">Page Content</span></span>

<span data-ttu-id="6ee1d-136">Die Ressource **SitePage** hat die folgenden Felder Content.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="6ee1d-137">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="6ee1d-137">Property name</span></span>      | <span data-ttu-id="6ee1d-138">Typ</span><span class="sxs-lookup"><span data-stu-id="6ee1d-138">Type</span></span>                       | <span data-ttu-id="6ee1d-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ee1d-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="6ee1d-140">title</span><span class="sxs-lookup"><span data-stu-id="6ee1d-140">title</span></span>              | <span data-ttu-id="6ee1d-141">string</span><span class="sxs-lookup"><span data-stu-id="6ee1d-141">string</span></span>                     | <span data-ttu-id="6ee1d-142">Der Titel der Seite.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-142">The title of the page.</span></span>
| <span data-ttu-id="6ee1d-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="6ee1d-143">pageLayout</span></span>         | <span data-ttu-id="6ee1d-144">string</span><span class="sxs-lookup"><span data-stu-id="6ee1d-144">string</span></span>                     | <span data-ttu-id="6ee1d-145">Der Name des auf der Seite auf das Seitenlayout.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="6ee1d-146">webParts</span><span class="sxs-lookup"><span data-stu-id="6ee1d-146">webParts</span></span>           | <span data-ttu-id="6ee1d-147">Webpart</span><span class="sxs-lookup"><span data-stu-id="6ee1d-147">[webPart][]</span></span>                | <span data-ttu-id="6ee1d-148">Die Webparts auf der Seite.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="6ee1d-149">Erstellen von Metadaten</span><span class="sxs-lookup"><span data-stu-id="6ee1d-149">Authoring Metadata</span></span>

<span data-ttu-id="6ee1d-150">Die Ressource **SitePage** hat die folgende authoring-bezogenen Metadaten.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="6ee1d-151">Die PublishingState-Eigenschaft wird die Seite Status wie ausgecheckt oder veröffentlicht authoring widerspiegeln.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="6ee1d-152">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="6ee1d-152">Property name</span></span>          | <span data-ttu-id="6ee1d-153">Typ</span><span class="sxs-lookup"><span data-stu-id="6ee1d-153">Type</span></span>                   | <span data-ttu-id="6ee1d-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ee1d-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="6ee1d-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="6ee1d-155">publishingState</span></span>        | <span data-ttu-id="6ee1d-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-156">[publicationFacet][]</span></span>   | <span data-ttu-id="6ee1d-157">Den Veröffentlichungsstatus und die MM.mm Version der Seite.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="6ee1d-158">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="6ee1d-159">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="6ee1d-159">Property name</span></span>        | <span data-ttu-id="6ee1d-160">Typ</span><span class="sxs-lookup"><span data-stu-id="6ee1d-160">Type</span></span>              | <span data-ttu-id="6ee1d-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ee1d-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="6ee1d-162">id</span><span class="sxs-lookup"><span data-stu-id="6ee1d-162">id</span></span>                   | <span data-ttu-id="6ee1d-163">string</span><span class="sxs-lookup"><span data-stu-id="6ee1d-163">string</span></span>            | <span data-ttu-id="6ee1d-p104">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="6ee1d-166">name</span><span class="sxs-lookup"><span data-stu-id="6ee1d-166">name</span></span>                 | <span data-ttu-id="6ee1d-167">string</span><span class="sxs-lookup"><span data-stu-id="6ee1d-167">string</span></span>            | <span data-ttu-id="6ee1d-168">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-168">The name / title of the item.</span></span>
| <span data-ttu-id="6ee1d-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="6ee1d-169">createdBy</span></span>            | <span data-ttu-id="6ee1d-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-170">[identitySet][]</span></span>   | <span data-ttu-id="6ee1d-171">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-171">Identity of the creator of this item.</span></span> <span data-ttu-id="6ee1d-172">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-172">Read-only.</span></span>
| <span data-ttu-id="6ee1d-173">eTag</span><span class="sxs-lookup"><span data-stu-id="6ee1d-173">eTag</span></span>                 | <span data-ttu-id="6ee1d-174">string</span><span class="sxs-lookup"><span data-stu-id="6ee1d-174">string</span></span>            | <span data-ttu-id="6ee1d-p106">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="6ee1d-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6ee1d-177">lastModifiedBy</span></span>       | <span data-ttu-id="6ee1d-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-178">[identitySet][]</span></span>   | <span data-ttu-id="6ee1d-179">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="6ee1d-180">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-180">Read-only.</span></span>
| <span data-ttu-id="6ee1d-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ee1d-181">lastModifiedDateTime</span></span> | <span data-ttu-id="6ee1d-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ee1d-182">DateTimeOffset</span></span>    | <span data-ttu-id="6ee1d-p108">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6ee1d-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="6ee1d-185">parentReference</span></span>      | <span data-ttu-id="6ee1d-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6ee1d-186">[itemReference][]</span></span> | <span data-ttu-id="6ee1d-p109">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6ee1d-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="6ee1d-189">webUrl</span></span>               | <span data-ttu-id="6ee1d-190">String (URL)</span><span class="sxs-lookup"><span data-stu-id="6ee1d-190">string (url)</span></span>      | <span data-ttu-id="6ee1d-p110">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="6ee1d-193">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ee1d-193">Relationships</span></span>

<span data-ttu-id="6ee1d-194">Die Ressource **SitePage** hat keine Beziehung zu anderen Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="6ee1d-194">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
<span data-ttu-id="6ee1d-202">Webpart</span><span class="sxs-lookup"><span data-stu-id="6ee1d-202">[webPart]: webpart.md</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->

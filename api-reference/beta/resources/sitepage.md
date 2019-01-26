---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9ecc23abbee165bce9fd4d9a2a5d8aac8aa02f41
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576241"
---
# <a name="sitepage-resource"></a><span data-ttu-id="2dedf-102">SitePage-Ressource</span><span class="sxs-lookup"><span data-stu-id="2dedf-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dedf-103">Diese Ressource stellt eine Seite in der SitePages [Liste][]dar.</span><span class="sxs-lookup"><span data-stu-id="2dedf-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="2dedf-104">Sie enthält den Titel, Layout und eine Auflistung von [WebPart][]s.</span><span class="sxs-lookup"><span data-stu-id="2dedf-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="2dedf-105">Aufgaben auf einer Seite</span><span class="sxs-lookup"><span data-stu-id="2dedf-105">Tasks on a page</span></span>

<span data-ttu-id="2dedf-106">Die folgenden Aufgaben sind für **SitePage** Ressourcen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2dedf-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="2dedf-107">Alle unten stehenden Beispiele sind relativ zu einer [Website][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="2dedf-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="2dedf-108">Häufige Aufgaben</span><span class="sxs-lookup"><span data-stu-id="2dedf-108">Common task</span></span>                     | <span data-ttu-id="2dedf-109">HTTP-Methode</span><span class="sxs-lookup"><span data-stu-id="2dedf-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="2dedf-110">[Seiten auflisten][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-110">[List pages][]</span></span>                  | <span data-ttu-id="2dedf-111">Abrufen von /pages</span><span class="sxs-lookup"><span data-stu-id="2dedf-111">GET /pages</span></span>
| <span data-ttu-id="2dedf-112">[Seite abrufen][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-112">[Get page][]</span></span>                    | <span data-ttu-id="2dedf-113">Abrufen von /pages/ {Seiten-Id}</span><span class="sxs-lookup"><span data-stu-id="2dedf-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="2dedf-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-114">[Create][]</span></span>                      | <span data-ttu-id="2dedf-115">POST-/pages</span><span class="sxs-lookup"><span data-stu-id="2dedf-115">POST /pages</span></span>
| <span data-ttu-id="2dedf-116">[Löschen][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-116">[Delete][]</span></span>                      | <span data-ttu-id="2dedf-117">Löschen von /pages/ {Seiten-Id}</span><span class="sxs-lookup"><span data-stu-id="2dedf-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="2dedf-118">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-118">[Publish][]</span></span>                     | <span data-ttu-id="2dedf-119">Posten Sie /pages/ {Seiten-Id} / veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="2dedf-119">POST /pages/{page-id}/publish</span></span>

[Seiten auflisten]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Seite abrufen]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="2dedf-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2dedf-125">JSON representation</span></span>

<span data-ttu-id="2dedf-126">Es folgt eine JSON-Darstellung einer **SitePage** Ressource.</span><span class="sxs-lookup"><span data-stu-id="2dedf-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

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

## <a name="properties"></a><span data-ttu-id="2dedf-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2dedf-127">Properties</span></span>

<span data-ttu-id="2dedf-128">Die Ressource **SitePage** hat die folgenden Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="2dedf-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="2dedf-129">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="2dedf-129">Property name</span></span>    | <span data-ttu-id="2dedf-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2dedf-130">Type</span></span>                         | <span data-ttu-id="2dedf-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dedf-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="2dedf-132">contentType</span><span class="sxs-lookup"><span data-stu-id="2dedf-132">contentType</span></span>      | <span data-ttu-id="2dedf-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="2dedf-134">Der Inhaltstyp der Seite.</span><span class="sxs-lookup"><span data-stu-id="2dedf-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="2dedf-135">Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="2dedf-135">Page Content</span></span>

<span data-ttu-id="2dedf-136">Die Ressource **SitePage** hat die folgenden Felder Content.</span><span class="sxs-lookup"><span data-stu-id="2dedf-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="2dedf-137">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="2dedf-137">Property name</span></span>      | <span data-ttu-id="2dedf-138">Typ</span><span class="sxs-lookup"><span data-stu-id="2dedf-138">Type</span></span>                       | <span data-ttu-id="2dedf-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dedf-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="2dedf-140">title</span><span class="sxs-lookup"><span data-stu-id="2dedf-140">title</span></span>              | <span data-ttu-id="2dedf-141">string</span><span class="sxs-lookup"><span data-stu-id="2dedf-141">string</span></span>                     | <span data-ttu-id="2dedf-142">Der Titel der Seite.</span><span class="sxs-lookup"><span data-stu-id="2dedf-142">The title of the page.</span></span>
| <span data-ttu-id="2dedf-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="2dedf-143">pageLayout</span></span>         | <span data-ttu-id="2dedf-144">string</span><span class="sxs-lookup"><span data-stu-id="2dedf-144">string</span></span>                     | <span data-ttu-id="2dedf-145">Der Name des auf der Seite auf das Seitenlayout.</span><span class="sxs-lookup"><span data-stu-id="2dedf-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="2dedf-146">webParts</span><span class="sxs-lookup"><span data-stu-id="2dedf-146">webParts</span></span>           | <span data-ttu-id="2dedf-147">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-147">[webPart][]</span></span>                | <span data-ttu-id="2dedf-148">Die Webparts auf der Seite.</span><span class="sxs-lookup"><span data-stu-id="2dedf-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="2dedf-149">Erstellen von Metadaten</span><span class="sxs-lookup"><span data-stu-id="2dedf-149">Authoring Metadata</span></span>

<span data-ttu-id="2dedf-150">Die Ressource **SitePage** hat die folgende authoring-bezogenen Metadaten.</span><span class="sxs-lookup"><span data-stu-id="2dedf-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="2dedf-151">Die PublishingState-Eigenschaft wird die Seite Status wie ausgecheckt oder veröffentlicht authoring widerspiegeln.</span><span class="sxs-lookup"><span data-stu-id="2dedf-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="2dedf-152">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="2dedf-152">Property name</span></span>          | <span data-ttu-id="2dedf-153">Typ</span><span class="sxs-lookup"><span data-stu-id="2dedf-153">Type</span></span>                   | <span data-ttu-id="2dedf-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dedf-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="2dedf-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="2dedf-155">publishingState</span></span>        | <span data-ttu-id="2dedf-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-156">[publicationFacet][]</span></span>   | <span data-ttu-id="2dedf-157">Den Veröffentlichungsstatus und die MM.mm Version der Seite.</span><span class="sxs-lookup"><span data-stu-id="2dedf-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="2dedf-158">Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.</span><span class="sxs-lookup"><span data-stu-id="2dedf-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="2dedf-159">Eigenschaftsname</span><span class="sxs-lookup"><span data-stu-id="2dedf-159">Property name</span></span>        | <span data-ttu-id="2dedf-160">Typ</span><span class="sxs-lookup"><span data-stu-id="2dedf-160">Type</span></span>              | <span data-ttu-id="2dedf-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2dedf-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="2dedf-162">id</span><span class="sxs-lookup"><span data-stu-id="2dedf-162">id</span></span>                   | <span data-ttu-id="2dedf-163">string</span><span class="sxs-lookup"><span data-stu-id="2dedf-163">string</span></span>            | <span data-ttu-id="2dedf-p104">Der eindeutige Bezeichner des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dedf-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="2dedf-166">name</span><span class="sxs-lookup"><span data-stu-id="2dedf-166">name</span></span>                 | <span data-ttu-id="2dedf-167">string</span><span class="sxs-lookup"><span data-stu-id="2dedf-167">string</span></span>            | <span data-ttu-id="2dedf-168">Der Name/Titel des Elements.</span><span class="sxs-lookup"><span data-stu-id="2dedf-168">The name / title of the item.</span></span>
| <span data-ttu-id="2dedf-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="2dedf-169">createdBy</span></span>            | <span data-ttu-id="2dedf-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-170">[identitySet][]</span></span>   | <span data-ttu-id="2dedf-171">Die Identität des Erstellers dieses Elements.</span><span class="sxs-lookup"><span data-stu-id="2dedf-171">Identity of the creator of this item.</span></span> <span data-ttu-id="2dedf-172">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dedf-172">Read-only.</span></span>
| <span data-ttu-id="2dedf-173">eTag</span><span class="sxs-lookup"><span data-stu-id="2dedf-173">eTag</span></span>                 | <span data-ttu-id="2dedf-174">string</span><span class="sxs-lookup"><span data-stu-id="2dedf-174">string</span></span>            | <span data-ttu-id="2dedf-p106">ETag für das Element. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dedf-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="2dedf-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2dedf-177">lastModifiedBy</span></span>       | <span data-ttu-id="2dedf-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-178">[identitySet][]</span></span>   | <span data-ttu-id="2dedf-179">Die Identität derPerson, die dieses Element zuletzt geändert hat.</span><span class="sxs-lookup"><span data-stu-id="2dedf-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="2dedf-180">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dedf-180">Read-only.</span></span>
| <span data-ttu-id="2dedf-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dedf-181">lastModifiedDateTime</span></span> | <span data-ttu-id="2dedf-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dedf-182">DateTimeOffset</span></span>    | <span data-ttu-id="2dedf-p108">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dedf-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="2dedf-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="2dedf-185">parentReference</span></span>      | <span data-ttu-id="2dedf-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="2dedf-186">[itemReference][]</span></span> | <span data-ttu-id="2dedf-p109">Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dedf-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="2dedf-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="2dedf-189">webUrl</span></span>               | <span data-ttu-id="2dedf-190">String (URL)</span><span class="sxs-lookup"><span data-stu-id="2dedf-190">string (url)</span></span>      | <span data-ttu-id="2dedf-p110">URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2dedf-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="2dedf-193">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2dedf-193">Relationships</span></span>

<span data-ttu-id="2dedf-194">Die Ressource **SitePage** hat keine Beziehung zu anderen Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="2dedf-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
[webPart]: webpart.md

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

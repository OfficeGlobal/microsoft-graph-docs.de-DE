---
title: Abrufen von OneNote-Inhalten und -Strukturen mit Microsoft Graph
description: " Enterprise-Notizbücher in Office 365"
author: Jewan-microsoft
ms.openlocfilehash: 3eff4548114d498b31d086f4a4825787c0971665
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325011"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="2f6bf-103">Abrufen von OneNote-Inhalten und -Strukturen mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2f6bf-103">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="2f6bf-104">**Gilt für**: Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365</span><span class="sxs-lookup"><span data-stu-id="2f6bf-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="2f6bf-105">Um OneNote-Inhalte und -Strukturen abzurufen, senden Sie eine GET-Anforderung an den Zielendpunkt.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-105">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="2f6bf-106">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-106">For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="2f6bf-107">Wenn die Anforderung erfolgreich ist, gibt Microsoft Graph den HTTP-Statuscode 200 und die Entitäten bzw. Inhalte zurück, die Sie angefordert haben.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-107">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="2f6bf-108">OneNote-Entitäten werden als JSON-Objekte zurückgegeben, die der Spezifikation der OData-Version 4.0 entsprechen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-108">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="2f6bf-109">Mithilfe von Abfragezeichenfolgenoptionen können Sie Ihre Abfragen filtern und die Leistung verbessern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-109">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="2f6bf-110">Erstellen des Anforderungs-URI</span><span class="sxs-lookup"><span data-stu-id="2f6bf-110">Construct the request URI</span></span>

<span data-ttu-id="2f6bf-111">Um den Anforderungs-URI zu erstellen, beginnen Sie mit der Stamm-URL des Diensts:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-111">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="2f6bf-112">Fügen Sie dann den Endpunkt der Ressource an, die Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-112">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="2f6bf-113">([Ressourcenpfade](#resource-paths-for-get-requests) werden im nächsten Abschnitt gezeigt.)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-113">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="2f6bf-114">Ihr vollständiger Anforderungs-URI gleicht einem der folgenden Beispiele:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-114">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="2f6bf-115">**Hinweis:** Hier erfahren Sie mehr über die [Stamm-URL des Diensts](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-115">**Note:** Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="2f6bf-116">Ressourcenpfade für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2f6bf-116">Resource paths for GET requests</span></span>

<span data-ttu-id="2f6bf-117">Verwenden Sie die folgenden Ressourcenpfade, um Seiten, Abschnitte, Abschnittsgruppen, Notizbücher und Bild- oder Dateiressourcen abzurufen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-117">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="2f6bf-118">Seitensammlung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-118">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="2f6bf-119">Seitenentität</span><span class="sxs-lookup"><span data-stu-id="2f6bf-119">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="2f6bf-120">Seitenvorschau</span><span class="sxs-lookup"><span data-stu-id="2f6bf-120">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="2f6bf-121">HTML-Inhalt einer Seite</span><span class="sxs-lookup"><span data-stu-id="2f6bf-121">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="2f6bf-122">Abschnittsammlung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-122">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="2f6bf-123">Abschnittentität</span><span class="sxs-lookup"><span data-stu-id="2f6bf-123">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="2f6bf-124">Abschnittsgruppen-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-124">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="2f6bf-125">Abschnittsgruppen-Entität</span><span class="sxs-lookup"><span data-stu-id="2f6bf-125">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="2f6bf-126">Notebook-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-126">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="2f6bf-127">Notebook-Entität</span><span class="sxs-lookup"><span data-stu-id="2f6bf-127">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="2f6bf-128">Bild- oder andere Dateiressource</span><span class="sxs-lookup"><span data-stu-id="2f6bf-128">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="2f6bf-129">Seitensammlung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-129">Page collection</span></span>

<span data-ttu-id="2f6bf-130">Rufen Sie Seiten (Metadaten) aus allen Notizbüchern ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-130">Get pages (metadata) across all notebooks.</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="2f6bf-131">Rufen Sie Seiten (Metadaten) aus einem bestimmten Abschnitt ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-131">Get pages (metadata) from a specific section.</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="2f6bf-132">Die `search`-Abfragezeichenfolgenoption ist nur für Heimanwender-Notizbücher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-132">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="2f6bf-133">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-133">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="2f6bf-134">Die Standardabfrage erweitert den übergeordneten Abschnitt und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-134">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="2f6bf-135">Standardmäßig werden nur die ersten 20 Einträge für *GET pages*-Anforderungen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-135">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="2f6bf-136">Anforderungen, die keine **top**-Abfragezeichenfolgenoption enthalten, geben einen `@odata.nextLink`-Link in der Antwort zurück, mit dem Sie die nächsten 20 Einträge abrufen können.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-136">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="2f6bf-137">Verwenden Sie für die Sammlung der Seiten in einem Abschnitt **pagelevel**, um die Einzugsebene von Seiten und ihre Reihenfolge innerhalb des Abschnitts zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-137">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="2f6bf-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-138">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="2f6bf-139">Seitenentität</span><span class="sxs-lookup"><span data-stu-id="2f6bf-139">Page entity</span></span>

<span data-ttu-id="2f6bf-140">Abrufen der Metadaten für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-140">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="2f6bf-141">Seiten können die Eigenschaften **parentNotebook** und **parentSection** erweitern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-141">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="2f6bf-142">Die Standardabfrage erweitert den übergeordneten Abschnitt und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-142">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="2f6bf-143">Verwenden Sie **pagelevel**, um die Einzugsebene der Seite und ihre Reihenfolge im übergeordneten Abschnitt zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-143">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="2f6bf-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-144">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="2f6bf-145">Seitenvorschau</span><span class="sxs-lookup"><span data-stu-id="2f6bf-145">Page preview</span></span>

<span data-ttu-id="2f6bf-146">Rufen Sie Text- und Bild-Vorschauinhalt für eine Seite ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-146">Get text and image preview content for a page.</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="2f6bf-147">Die JSON-Antwort enthält den Vorschauinhalt, anhand dessen Benutzer feststellen können, was sich auf der Seite befindet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-147">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

<span data-ttu-id="2f6bf-148">Die **previewText**-Eigenschaft enthält einen Textausschnitt von der Seite.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-148">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="2f6bf-149">Microsoft Graph gibt vollständige Ausdrücke im Umfang von maximal 300 Zeichen zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-149">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="2f6bf-150">Wenn die Seite über ein Bild verfügt, das zum Erstellen einer Vorschau der Benutzeroberfläche verwendet werden kann, enthält die **href**-Eigenschaft im **previewImageUrl**-Objekt einen Link zu einer öffentlichen, vorab authentifizierten [Bildressource](#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-150">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="2f6bf-151">Sie können diesen Link in HTML-Code verwenden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-151">You can use this link in HTML.</span></span> <span data-ttu-id="2f6bf-152">Andernfalls gibt **href** NULL zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-152">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="2f6bf-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-153">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="2f6bf-154">HTML-Inhalt einer Seite</span><span class="sxs-lookup"><span data-stu-id="2f6bf-154">Page HTML content</span></span>

<span data-ttu-id="2f6bf-155">Rufen Sie den HTML-Code einer Seite ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-155">Get the HTML content of a page.</span></span>

`../pages/{page-id}/content[?includeIDs,preAuthenticated]`

<span data-ttu-id="2f6bf-156">(*Weitere Informationen zu [zurückgegebenen HTML-Inhalten](onenote-input-output-html.md)*)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-156">(*learn more about [returned HTML content](onenote-input-output-html.md)*)</span></span> 

<br/>

<span data-ttu-id="2f6bf-157">Verwenden Sie die Abfragezeichenfolgenoption **includeIDs=true**, um die zum [Aktualisieren der Seite](onenote-update-page.md) generierten IDs abzurufen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-157">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote-update-page.md).</span></span>

<span data-ttu-id="2f6bf-158">Verwenden Sie die Abfragezeichenfolgenoption **preAuthenticated=true** zum Abrufen von öffentlichen URLs zu den [Bildressourcen](#image-or-other-file-resource), die sich auf der Seite befinden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-158">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page.</span></span> <span data-ttu-id="2f6bf-159">Die öffentlichen URLs sind eine Stunde lang gültig.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-159">The public URLs are valid for one hour.</span></span> 



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="2f6bf-160">Abschnittsammlung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-160">Section collection</span></span>

<span data-ttu-id="2f6bf-161">Rufen Sie alle Abschnitte aus allen Notizbüchern im Besitz des Benutzers ab, einschließlich der Abschnitte in geschachtelten Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-161">Get all sections from all notebooks that are owned by the user, including sections in nested section groups.</span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="2f6bf-162">Rufen Sie alle Abschnitte, die sich direkt unter einer bestimmten Abschnittsgruppe befinden ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-162">Get all sections that are directly under a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="2f6bf-163">Rufen Sie alle Abschnitte ab, die sich direkt unter einem bestimmten Notizbuch befinden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-163">Get all sections that are directly under a specific notebook.</span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="2f6bf-164">Abschnitte können die Eigenschaften **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-164">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="2f6bf-165">Die Standardsortierreihenfolge für Abschnitte ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-165">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="2f6bf-166">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-166">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="2f6bf-167">Abschnittentität</span><span class="sxs-lookup"><span data-stu-id="2f6bf-167">Section entity</span></span>

<span data-ttu-id="2f6bf-168">Rufen Sie einen bestimmten Abschnitt ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-168">Get a specific section.</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="2f6bf-169">Abschnitte können die Eigenschaften **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-169">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="2f6bf-170">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-170">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="2f6bf-171">Abschnittsgruppen-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-171">SectionGroup collection</span></span>

<span data-ttu-id="2f6bf-172">Rufen Sie alle Abschnittsgruppen aus allen Notizbüchern im Besitz des Benutzers ab, einschließlich geschachtelter Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-172">Get all section groups from all notebooks that are owned by the user, including nested section groups.</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="2f6bf-173">Rufen Sie alle Abschnittsgruppen ab, die sich direkt unter einem bestimmten Notizbuch befinden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-173">Get all section groups that are directly under a specific notebook.</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="2f6bf-174">Abschnittsgruppen können die Eigenschaften **sections**, **sectionGroups**, **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-174">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="2f6bf-175">Die Standardsortierreihenfolge für Abschnittsgruppen ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-175">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="2f6bf-176">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-176">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="2f6bf-177">Abschnittsgruppen-Entität</span><span class="sxs-lookup"><span data-stu-id="2f6bf-177">SectionGroup entity</span></span>

<span data-ttu-id="2f6bf-178">Rufen Sie eine bestimmte Abschnittsgruppe ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-178">Get a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="2f6bf-179">Abschnittsgruppen können die Eigenschaften **sections**, **sectionGroups**, **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-179">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="2f6bf-180">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-180">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="2f6bf-181">Notebook-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-181">Notebook collection</span></span>

<span data-ttu-id="2f6bf-182">Rufen Sie alle Notizbücher ab, deren Eigentümer der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-182">Get all the notebooks that are owned by the user.</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="2f6bf-183">Notizbücher können die Eigenschaften **sections** und **sectionGroups** erweitern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-183">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="2f6bf-184">Die Standardsortierreihenfolge für Notizbücher ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-184">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="2f6bf-185">Notebook-Entität</span><span class="sxs-lookup"><span data-stu-id="2f6bf-185">Notebook entity</span></span>

<span data-ttu-id="2f6bf-186">Rufen Sie ein bestimmtes Notizbuch ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-186">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="2f6bf-187">Notizbücher können die Eigenschaften **sections** und **sectionGroups** erweitern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-187">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="2f6bf-188">Bild- oder andere Dateiressource</span><span class="sxs-lookup"><span data-stu-id="2f6bf-188">Image or other file resource</span></span>

<span data-ttu-id="2f6bf-189">Rufen Sie die Binärdaten einer bestimmten Ressource ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-189">Get the binary data of a specific resource.</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="2f6bf-190">Sie finden den Ressourcen-URI der Datei im [Ausgabe-HTML-Code](onenote-input-output-html.md) der Seite.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-190">You can find the file's resource URI in the page's [output HTML](onenote-input-output-html.md).</span></span>

<span data-ttu-id="2f6bf-191">Beispielsweise enthält ein **img**-Tag Endpunkte für das Originalbild im **data-fullres-src**-Attribut und das optimierte Bild im **src**-Attribut.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-191">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="2f6bf-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-192">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="2f6bf-193">Und ein **object**-Tag enthält den Endpunkt für die Dateiressource im **data**-Attribut.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-193">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="2f6bf-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-194">Example</span></span>

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="2f6bf-195">Um öffentliche, vorab authentifizierte URLs für die Bildressourcen auf einer Seite zu erhalten, fügen Sie `preAuthenticated=true` in die Abfragezeichenfolge ein, wenn Sie [die Seiteninhalte abrufen](#page-html-content) (**Beispiel:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-195">To get public, pre-authenticated URLs to the image resources on a page, include `preAuthenticated=true` in the query string when you [retrieve the page content](#page-html-content) (**example:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="2f6bf-196">Die öffentlichen URLs, die im [Ausgabe-HTML-Code](onenote-input-output-html.md#output-html-examples-for-images) zurückgegeben werden, sind eine Stunde lang gültig.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-196">The public URLs that are returned in the [output HTML](onenote-input-output-html.md#output-html-examples-for-images) are valid for one hour.</span></span> <span data-ttu-id="2f6bf-197">Ohne dieses Flag können Bilder nicht direkt in einem Browser gerendert werden, da sie wie die restlichen Seiteninhalte privat sind und eine Autorisierung erforderlich ist, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-197">Without this flag, retrieved images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="2f6bf-198">**Hinweis:** Das Abrufen einer Sammlung von Ressourcen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-198">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="2f6bf-199">Beim Abrufen einer Dateiressource müssen Sie keinen **Accept**-Inhaltstyp in der Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-199">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="2f6bf-200">Weitere Informationen über GET-Anforderungen finden Sie unter den folgenden Ressourcen in der Referenz zur Microsoft Graph-API:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-200">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="2f6bf-201">GET Pages</span><span class="sxs-lookup"><span data-stu-id="2f6bf-201">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="2f6bf-202">GET Sections</span><span class="sxs-lookup"><span data-stu-id="2f6bf-202">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="2f6bf-203">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="2f6bf-203">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="2f6bf-204">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="2f6bf-204">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="2f6bf-205">Beispiele für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2f6bf-205">Example GET requests</span></span>

<span data-ttu-id="2f6bf-206">Sie können Abfragen für OneNote-Entitäten stellen und Seiteninhalte durchsuchen, um genau die gesuchten Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-206">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="2f6bf-207">Die folgenden Beispiele zeigen einige Verwendungsmöglichkeiten für [unterstützte Abfragezeichenfolgenoptionen](#supported-odata-query-string-options) in GET-Anforderungen für Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-207">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="2f6bf-208">**Zur Erinnerung:**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-208">**Remember:**</span></span>

- <span data-ttu-id="2f6bf-209">Alle GET-Anforderungen beginnen mit der [Stamm-URL des Diensts](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-209">All GET requests start with the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span> <br/><br/><span data-ttu-id="2f6bf-210">**Beispiele**: `https://www.onenote.com/api/v1.0/me/notes` und `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span><span class="sxs-lookup"><span data-stu-id="2f6bf-210">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="2f6bf-211">Leerzeichen in der URL-Abfragezeichenfolge müssen mit %20 codiert sein.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-211">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="2f6bf-212">**Beispiel**: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="2f6bf-212">**Example**: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="2f6bf-213">Bei Eigenschaftennamen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-213">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="2f6bf-214">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-214">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="2f6bf-215">**Beispiel**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="2f6bf-215">**Example**: `filter=tolower(name) eq 'spring'`</span></span>
 

### <a name="search--filter"></a><span data-ttu-id="2f6bf-216">search & filter</span><span class="sxs-lookup"><span data-stu-id="2f6bf-216">search & filter</span></span>  

<span data-ttu-id="2f6bf-217">Abrufen aller Seiten, die den Begriff *recipe* enthalten und von einer bestimmten App erstellt wurden (`search` ist nur für Heimanwender-Notizbücher verfügbar).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-217">Get all pages that contain the term *recipe* that were created by a specific app (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="2f6bf-218">search & select</span><span class="sxs-lookup"><span data-stu-id="2f6bf-218">search & select</span></span>  

<span data-ttu-id="2f6bf-219">Abrufen des Titels, der OneNote-Clientlinks und des **contentUrl**-Links für alle Seiten, die den Begriff *golgi app* enthalten (`search` ist nur für Heimanwender-Notizbücher verfügbar).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-219">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app* (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="2f6bf-220">expand</span><span class="sxs-lookup"><span data-stu-id="2f6bf-220">expand</span></span> 

<span data-ttu-id="2f6bf-221">Abrufen aller Notizbücher und Erweitern ihrer Abschnitte und Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-221">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="2f6bf-222">Abrufen einer bestimmten Abschnittsgruppe und Erweitern ihrer Abschnitte und Abschnittsgruppen:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-222">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="2f6bf-223">Abrufen einer Seite und Erweitern Ihres übergeordneten Abschnitts und übergeordneten Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-223">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="2f6bf-224">expand (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-224">expand (multiple levels)</span></span>  

<span data-ttu-id="2f6bf-225">Abrufen aller Notizbücher und Erweitern ihrer Abschnitte und Abschnittsgruppen sowie aller Abschnitte in jeder Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-225">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="2f6bf-226">**Hinweis:** Das Erweitern übergeordneter Elemente von untergeordneten Entitäten oder das Erweitern von untergeordneten Elementen von übergeordneten Entitäten erstellt einen Zirkelbezug und wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-226">**Note:** Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="2f6bf-227">expand & select (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-227">expand & select (multiple levels)</span></span>  

<span data-ttu-id="2f6bf-228">Abrufen des Namens und des **self**-Links für eine bestimmte Abschnittsgruppe sowie des Namens und **self**-Links für alle enthaltenen Abschnitte.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-228">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="2f6bf-229">Abrufen des Namens und des **self**-Links für alle Abschnitte sowie des Namens und der Erstellungszeit des übergeordneten Notizbuchs jedes Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-229">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="2f6bf-230">Abrufen des Titels und der ID für alle Seiten sowie Abrufen des Namens des übergeordneten Abschnitts und des übergeordneten Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-230">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="2f6bf-231">expand & levels (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-231">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="2f6bf-232">Abrufen aller Notizbücher, Abschnitte und Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-232">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="2f6bf-233">filter</span><span class="sxs-lookup"><span data-stu-id="2f6bf-233">filter</span></span>

<span data-ttu-id="2f6bf-234">Abrufen aller Abschnitte, die im Oktober 2014 erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-234">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="2f6bf-235">Abrufen der Seiten, die von einer bestimmten App seit dem 1. Januar 2015 erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-235">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="2f6bf-236">filter & expand</span><span class="sxs-lookup"><span data-stu-id="2f6bf-236">filter & expand</span></span>  

<span data-ttu-id="2f6bf-237">Rufen Sie alle Seiten in einem bestimmten Notizbuch ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-237">Get all pages in a specific notebook.</span></span> <span data-ttu-id="2f6bf-238">Die API gibt standardmäßig 20 Seiten zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-238">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="2f6bf-239">Rufen Sie den Namens und den **pagesUrl**-Link für alle Abschnitte aus dem Notizbuch *School* ab.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-239">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="2f6bf-240">In OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet. Verwenden Sie daher am besten die **tolower**-Funktion.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-240">OData string comparisons are case-sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="2f6bf-241">filter & select & orderby</span><span class="sxs-lookup"><span data-stu-id="2f6bf-241">filter & select & orderby</span></span>   

<span data-ttu-id="2f6bf-242">Abrufen des Namens und des **pagesUrl**-Links für alle Abschnitte, die den Ausdruck *spring* im Abschnittsnamen enthalten.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-242">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="2f6bf-243">Sortieren der Abschnitte nach dem Datum der letzten Änderung.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-243">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="2f6bf-244">orderby</span><span class="sxs-lookup"><span data-stu-id="2f6bf-244">orderby</span></span>

<span data-ttu-id="2f6bf-245">Abrufen der ersten 20 Seiten, sortiert nach der **createdByAppId**-Eigenschaft und dann nach der letzten Erstellungszeit.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-245">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="2f6bf-246">Die API gibt standardmäßig 20 Seiten zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-246">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="2f6bf-247">search & filter & top</span><span class="sxs-lookup"><span data-stu-id="2f6bf-247">search & filter & top</span></span> 

<span data-ttu-id="2f6bf-248">Abrufen der fünf neuesten Seiten, die seit dem 1. Januar 2015 erstellt wurden und die den Ausdruck *cell division* enthalten.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-248">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="2f6bf-249">Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-249">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="2f6bf-250">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc` (`search` ist nur für Heimanwender-Notizbücher verfügbar).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-250">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="2f6bf-251">search & filter & top & skip</span><span class="sxs-lookup"><span data-stu-id="2f6bf-251">search & filter & top & skip</span></span>  

<span data-ttu-id="2f6bf-252">Rufen Sie die folgenden fünf Seiten im Resultset ab (`search` ist nur für Heimanwender-Notizbücher verfügbar).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-252">Get the next five pages in the result set (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="2f6bf-253">Und die folgenden fünf (`search` ist nur für Heimanwender-Notizbücher verfügbar)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-253">And the next five (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="2f6bf-254">**Hinweis:** Wenn **search** und **filter** auf dieselbe Anforderung angewendet werden, enthält das Ergebnis nur die Entitäten, die beide Kriterien erfüllen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-254">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="2f6bf-255">select</span><span class="sxs-lookup"><span data-stu-id="2f6bf-255">select</span></span>

<span data-ttu-id="2f6bf-256">Abrufen von Name, Erstellungszeit und **self**-Link für alle Abschnitte in den Notizbüchern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-256">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="2f6bf-257">Abrufen des Titels, der Erstellungszeit und der OneNote-Clientlinks für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-257">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="2f6bf-258">select & expand & filter (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-258">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="2f6bf-259">Abrufen von Name und **pagesUrl**-Link für alle Abschnitte im Standardnotizbuch des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-259">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="2f6bf-260">top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="2f6bf-260">top & select & orderby</span></span> 

<span data-ttu-id="2f6bf-261">Abrufen des Titels und des **self**-Links für die ersten 50 Seiten, alphabetisch sortiert nach Titel.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-261">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="2f6bf-262">Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-262">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="2f6bf-263">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-263">The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="2f6bf-264">skip & top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="2f6bf-264">skip & top & select & orderby</span></span>  

<span data-ttu-id="2f6bf-p117">Abrufen der Seiten 51 bis 100. Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-p117">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="2f6bf-267">**Hinweis:** GET-Anforderungen für Seiten, die die Standardanzahl von Einträgen abrufen (d. h., sie enthalten keinen **top**-Ausdruck) geben einen **@odata.nextLink**-Link in der Antwort zurück, mit dem Sie die nächsten 20 Einträge abrufen können.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-267">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="2f6bf-268">Unterstützte Optionen für OData-Abfragezeichenfolgen</span><span class="sxs-lookup"><span data-stu-id="2f6bf-268">Supported OData query string options</span></span>

<span data-ttu-id="2f6bf-269">Beim Senden von GET-Anforderungen an Microsoft Graph können Sie die Abfrage mit Optionen für OData-Abfragezeichenfolgen anpassen und so genau die gewünschten Informationen erhalten.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-269">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="2f6bf-270">Sie können auch eine Leistungssteigerung erzielen, indem die Anzahl der Aufrufe an den Dienst und die Größe der Antwortnutzlast reduziert wird.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-270">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="2f6bf-271">**Hinweis:** Zur besseren Lesbarkeit wird in den Beispielen in diesem Artikel nicht die erforderliche Prozentcodierung %20 für Leerzeichen in der URL-Abfragezeichenfolge verwendet: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="2f6bf-271">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="2f6bf-272">Abfrageoption</span><span class="sxs-lookup"><span data-stu-id="2f6bf-272">Query option</span></span> | <span data-ttu-id="2f6bf-273">Beispiel und Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-273">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="2f6bf-274">count</span><span class="sxs-lookup"><span data-stu-id="2f6bf-274">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="2f6bf-p119">Die Anzahl der Einträge in der Auflistung. Der Wert wird in der Antwort in der **@odata.count**-Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-p119">The count of entities in the collection. The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="2f6bf-277">expand</span><span class="sxs-lookup"><span data-stu-id="2f6bf-277">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="2f6bf-278">Die Navigationseigenschaften, die inline in der Antwort zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-278">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="2f6bf-279">Die folgenden Eigenschaften werden für **expand**-Ausdrücke unterstützt:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-279">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="2f6bf-280">– Seiten: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-280">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="2f6bf-281">– Abschnitte: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-281">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="2f6bf-282">– Abschnittsgruppen: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-282">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="2f6bf-283">– Notizbücher: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-283">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="2f6bf-284">Standardmäßig erweitern GET-Anforderungen für Seiten **parentSection** und wählen die Eigenschaften **id**, **name** und **self** des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-284">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties.</span></span> <span data-ttu-id="2f6bf-285">Standardmäßig erweitern GET-Anforderungen für Abschnitte und Abschnittsgruppen **parentNotebook** und **parentSectionGroup** und wählen die Eigenschaften **id**, **name** und **self** der übergeordneten Elemente aus.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-285">Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties.</span></span> </p><p><span data-ttu-id="2f6bf-286">Kann für eine einzelne Entität oder eine Sammlung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-286">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="2f6bf-287">Trennen Sie mehrere Eigenschaften durch Kommas.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-287">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="2f6bf-288">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-288">Property names are case-sensitive.</span></span></p> |   
| <span data-ttu-id="2f6bf-289">filter</span><span class="sxs-lookup"><span data-stu-id="2f6bf-289">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="2f6bf-290">Ein boolescher Ausdruck, der angibt, ob ein Eintrag in das Resultset aufgenommen werden soll.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-290">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="2f6bf-291">Unterstützt die folgenden OData-Operatoren und -Funktionen:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-291">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="2f6bf-292">– Vergleichsoperatoren: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-292">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="2f6bf-293">– Logische Operatoren: **and**, **or**, **not**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-293">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="2f6bf-294">– Zeichenfolgenfunktionen: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-294">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="2f6bf-295">Bei [Eigenschaften](#onenote-entity-properties)namen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-295">[Property](#onenote-entity-properties) names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="2f6bf-296">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-296">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="2f6bf-297">**Beispiel**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="2f6bf-297">**Example**: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="2f6bf-298">orderby</span><span class="sxs-lookup"><span data-stu-id="2f6bf-298">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="2f6bf-p124">Die [Eigenschaften](#onenote-entity-properties), nach denen sortiert werden soll, mit einer optionalen Sortierreihenfolge **asc** (Standard) oder **desc**. Sie können nach jeder beliebigen Eigenschaft der Entität in der angeforderten Auflistung sortieren.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-p124">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="2f6bf-301">Die Standardsortierreihenfolge für Notizbücher, Abschnittsgruppen und Abschnitte ist `name asc` und für Seiten `lastModifiedTime desc` (zuletzt geänderte Seite zuerst).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-301">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="2f6bf-302">Trennen Sie mehrere Eigenschaften durch Kommas, und führen Sie sie in der Reihenfolge auf, in der sie angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-302">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="2f6bf-303">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-303">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="2f6bf-304">search</span><span class="sxs-lookup"><span data-stu-id="2f6bf-304">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="2f6bf-305">Nur für Heimanwender-Notizbücher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-305">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="2f6bf-p126">Der zu suchende Begriff oder Ausdruck im Seitentitel, Seitentext, Alternativtext für Bilder und OCR-Text für Bilder. Standardmäßig werden die Ergebnisse von Suchabfragen nach Relevanz sortiert zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-p126">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="2f6bf-308">OneNote verwendet die Bing-Volltextsuche, um die Suche nach Wortgruppen, Wortstammerkennung, Toleranz gegen Rechtschreibfehler, Relevanz und Bewertung, Worttrennung, mehrere Sprachen und andere Volltext-Suchfunktionen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-308">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="2f6bf-309">In Suchzeichenfolgen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-309">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="2f6bf-310">Gilt nur für Seiten in Notizbüchern im Besitz des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-310">Applies only to pages in notebooks owned by the user.</span></span> <span data-ttu-id="2f6bf-311">Indizierter Inhalt ist privat und nur für den Besitzer zugänglich.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-311">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="2f6bf-312">Kennwortgeschützte Seiten werden nicht indiziert.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-312">Password-protected pages are not indexed.</span></span> <span data-ttu-id="2f6bf-313">Gilt nur für den `pages`-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-313">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="2f6bf-314">select</span><span class="sxs-lookup"><span data-stu-id="2f6bf-314">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="2f6bf-315">Die [Eigenschaften](#onenote-entity-properties), die zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-315">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="2f6bf-316">Kann für eine einzelne Entität oder eine Sammlung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-316">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="2f6bf-317">Trennen Sie mehrere Eigenschaften durch Kommas.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-317">Separate multiple properties with commas.</span></span> <span data-ttu-id="2f6bf-318">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-318">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="2f6bf-319">skip</span><span class="sxs-lookup"><span data-stu-id="2f6bf-319">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="2f6bf-320">Die Anzahl der Einträge, die im Resultset übersprungen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-320">The number of entries to skip in the result set.</span></span> <span data-ttu-id="2f6bf-321">In der Regel für die Seitenverwaltung der Ergebnisse verwendet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-321">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="2f6bf-322">Nach oben</span><span class="sxs-lookup"><span data-stu-id="2f6bf-322">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="2f6bf-323">Die Anzahl der zurückzugebenden Einträge im Resultset, maximal 100.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-323">The number of entries to return in the result set, up to a maximum of 100.</span></span> <span data-ttu-id="2f6bf-324">Der Standardwert ist 20.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-324">The default value is 20.</span></span></p> |  

<span data-ttu-id="2f6bf-325">Microsoft Graph bietet außerdem die `pagelevel`-Zeichenfolgenoption, mit der Sie die Ebene und die Reihenfolge der Seiten innerhalb des übergeordneten Abschnitts abrufen können.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-325">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="2f6bf-326">Gilt nur für Abfragen für Seiten in einem bestimmten Abschnitt oder für Abfragen für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-326">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="2f6bf-327">Beispiele</span><span class="sxs-lookup"><span data-stu-id="2f6bf-327">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="2f6bf-328">Unterstützte OData-Operatoren und -Funktionen</span><span class="sxs-lookup"><span data-stu-id="2f6bf-328">Supported OData operators and functions</span></span>

<span data-ttu-id="2f6bf-329">Microsoft Graph unterstützt die folgenden OData-Operatoren und Funktionen in **filter**-Ausdrücken.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-329">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="2f6bf-330">Beachten Sie bei der Verwendung von OData-Ausdrücken Folgendes:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-330">When using OData expressions, remember:</span></span>

- <span data-ttu-id="2f6bf-331">Leerzeichen in der URL-Abfagezeichenfolge müssen durch die Codierung `%20` ersetzt werden.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-331">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="2f6bf-332">**Beispiel:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="2f6bf-332">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="2f6bf-333">Bei Eigenschaftennamen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-333">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="2f6bf-334">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-334">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="2f6bf-335">**Beispiel:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="2f6bf-335">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="2f6bf-336">Vergleichsoperator</span><span class="sxs-lookup"><span data-stu-id="2f6bf-336">Comparison operator</span></span> | <span data-ttu-id="2f6bf-337">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-337">Example</span></span> |  
|------|------|  
| <span data-ttu-id="2f6bf-338">eq</span><span class="sxs-lookup"><span data-stu-id="2f6bf-338">eq</span></span><br /><span data-ttu-id="2f6bf-339">(gleich)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-339">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="2f6bf-340">ne</span><span class="sxs-lookup"><span data-stu-id="2f6bf-340">ne</span></span><br /><span data-ttu-id="2f6bf-341">(nicht gleich)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-341">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="2f6bf-342">gt</span><span class="sxs-lookup"><span data-stu-id="2f6bf-342">gt</span></span><br /><span data-ttu-id="2f6bf-343">(größer als)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-343">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="2f6bf-344">ge</span><span class="sxs-lookup"><span data-stu-id="2f6bf-344">ge</span></span><br /><span data-ttu-id="2f6bf-345">(größer als oder gleich)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-345">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="2f6bf-346">lt</span><span class="sxs-lookup"><span data-stu-id="2f6bf-346">lt</span></span><br /><span data-ttu-id="2f6bf-347">(kleiner als)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-347">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="2f6bf-348">le</span><span class="sxs-lookup"><span data-stu-id="2f6bf-348">le</span></span><br /><span data-ttu-id="2f6bf-349">(kleiner als oder gleich)</span><span class="sxs-lookup"><span data-stu-id="2f6bf-349">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="2f6bf-350">Logischer Operator</span><span class="sxs-lookup"><span data-stu-id="2f6bf-350">Logical operator</span></span> | <span data-ttu-id="2f6bf-351">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-351">Example</span></span> |  
|------|------|  
| <span data-ttu-id="2f6bf-352">und</span><span class="sxs-lookup"><span data-stu-id="2f6bf-352">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="2f6bf-353">oder</span><span class="sxs-lookup"><span data-stu-id="2f6bf-353">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="2f6bf-354">not</span><span class="sxs-lookup"><span data-stu-id="2f6bf-354">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="2f6bf-355">String-Funktion</span><span class="sxs-lookup"><span data-stu-id="2f6bf-355">String function</span></span> | <span data-ttu-id="2f6bf-356">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-356">Example</span></span> |  
|------|------|   
| <span data-ttu-id="2f6bf-357">contains</span><span class="sxs-lookup"><span data-stu-id="2f6bf-357">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="2f6bf-358">endswith</span><span class="sxs-lookup"><span data-stu-id="2f6bf-358">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="2f6bf-359">startswith</span><span class="sxs-lookup"><span data-stu-id="2f6bf-359">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="2f6bf-360">length</span><span class="sxs-lookup"><span data-stu-id="2f6bf-360">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="2f6bf-361">indexof</span><span class="sxs-lookup"><span data-stu-id="2f6bf-361">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="2f6bf-362">substring</span><span class="sxs-lookup"><span data-stu-id="2f6bf-362">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="2f6bf-363">tolower</span><span class="sxs-lookup"><span data-stu-id="2f6bf-363">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="2f6bf-364">toupper</span><span class="sxs-lookup"><span data-stu-id="2f6bf-364">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="2f6bf-365">trim</span><span class="sxs-lookup"><span data-stu-id="2f6bf-365">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="2f6bf-366">concat</span><span class="sxs-lookup"><span data-stu-id="2f6bf-366">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="2f6bf-367">OneNote-Entitätseigenschaften</span><span class="sxs-lookup"><span data-stu-id="2f6bf-367">OneNote entity properties</span></span>

<span data-ttu-id="2f6bf-368">Die Abfrageausdrücke **filter**, **select**, **expand** und **orderby** können Eigenschaften von OneNote-Entitäten enthalten.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-368">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="2f6bf-369">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6bf-369">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="2f6bf-370">Bei Eigenschaftennamen in Abfrageausdrücken wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-370">Property names are case-sensitive in query expressions.</span></span>

<span data-ttu-id="2f6bf-371">Die Liste der Eigenschaften und Eigenschaftentypen finden Sie unter den folgenden Ressourcen in der Referenz zur Microsoft Graph-API:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-371">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="2f6bf-372">GET Pages</span><span class="sxs-lookup"><span data-stu-id="2f6bf-372">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="2f6bf-373">GET Sections</span><span class="sxs-lookup"><span data-stu-id="2f6bf-373">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="2f6bf-374">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="2f6bf-374">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="2f6bf-375">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="2f6bf-375">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 



<span data-ttu-id="2f6bf-376">Die Abfragezeichenfolgenoption **expand** kann mit folgenden Navigationseigenschaften verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-376">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="2f6bf-377">Seiten: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-377">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="2f6bf-378">Abschnitte: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-378">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="2f6bf-379">Abschnittsgruppen: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-379">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="2f6bf-380">Notizbücher: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="2f6bf-380">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="2f6bf-381">Anforderungs- and Antwortinformationen für *GET*-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2f6bf-381">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="2f6bf-382">Anforderungsdaten</span><span class="sxs-lookup"><span data-stu-id="2f6bf-382">Request data</span></span> | <span data-ttu-id="2f6bf-383">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-383">Description</span></span> |  
|------|------|  
| <span data-ttu-id="2f6bf-384">Protokoll</span><span class="sxs-lookup"><span data-stu-id="2f6bf-384">Protocol</span></span> | <span data-ttu-id="2f6bf-385">Alle Anforderungen verwenden das SSL/TLS HTTPS-Protokoll.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-385">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="2f6bf-386">Header „Authorization“</span><span class="sxs-lookup"><span data-stu-id="2f6bf-386">Authorization header</span></span> | <p><span data-ttu-id="2f6bf-387">`Bearer {token}`, wobei `{token}` ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-387">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="2f6bf-388">Wenn dies fehlt oder ungültig ist, schlägt die Anforderung mit dem Statuscode 401 fehl.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-388">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="2f6bf-389">Siehe [Authentifizierung und Berechtigungen](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-389">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="2f6bf-390">Header „Accept“</span><span class="sxs-lookup"><span data-stu-id="2f6bf-390">Accept header</span></span> | <p> <span data-ttu-id="2f6bf-391">`application/json` für OneNote-Entitäten und -Entitätenmengen</span><span class="sxs-lookup"><span data-stu-id="2f6bf-391">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="2f6bf-392">`text/html` für Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="2f6bf-392">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="2f6bf-393">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="2f6bf-393">Response data</span></span> | <span data-ttu-id="2f6bf-394">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f6bf-394">Description</span></span> |  
|------|------|  
| <span data-ttu-id="2f6bf-395">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="2f6bf-395">Success code</span></span> | <span data-ttu-id="2f6bf-396">HTTP-Statuscode 200.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-396">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="2f6bf-397">Antworttext</span><span class="sxs-lookup"><span data-stu-id="2f6bf-397">Response body</span></span> | <span data-ttu-id="2f6bf-398">Eine OData-Darstellung der Entität oder der Entitätenmenge im JSON-Format, der HTML-Code der Seite oder Binärdaten der Dateiressource.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-398">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="2f6bf-399">Fehler</span><span class="sxs-lookup"><span data-stu-id="2f6bf-399">Errors</span></span> | <span data-ttu-id="2f6bf-400">Wenn die Anforderung nicht erfüllt wird, gibt die API [Fehler](onenote-error-codes.md) im **@api.diagnostics**-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-400">If the request fails, the API returns [errors](onenote-error-codes.md) in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="2f6bf-401">Header „X-CorrelationId“</span><span class="sxs-lookup"><span data-stu-id="2f6bf-401">X-CorrelationId header</span></span> | <span data-ttu-id="2f6bf-402">Ein globaler Bezeichner (GUID), über den die Anforderung eindeutig identifiziert wird.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-402">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="2f6bf-403">Sie können diesen Wert zusammen mit dem Wert des Date-Headers verwenden, um zusammen mit dem Microsoft Support Probleme zu behandeln.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-403">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="2f6bf-404">Erstellen der Stamm-URL des Microsoft Graph-Notizendiensts</span><span class="sxs-lookup"><span data-stu-id="2f6bf-404">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="2f6bf-405">Die Stamm-URL des Microsoft Graph-Notizendienses verwendet das folgende Format für alle Aufrufe von Microsoft Graph-Notizen:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-405">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="2f6bf-406">Das Segment `version` in der URL ist die Version von Microsoft Graph, die verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-406">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="2f6bf-407">Verwenden Sie `v1.0` für stabilen Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-407">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="2f6bf-408">Verwenden Sie `beta`, um ein Feature zu testen, das sich in der Entwicklung befindet.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-408">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="2f6bf-409">Features und Funktionen in der Betaversion ändern sich möglicherweise, sodass Sie es nicht in Ihrem Produktionscode verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-409">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="2f6bf-410">Verwenden Sie `me` für OneNote-Inhalt, auf den der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-410">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="2f6bf-411">Verwenden Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-411">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="2f6bf-412">Verwenden Sie [Microsoft Graph](https://graph.microsoft.com/v1.0/users), um Benutzer-IDs abzurufen.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-412">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="2f6bf-413">Berechtigungen für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2f6bf-413">Permissions for GET requests</span></span>

<span data-ttu-id="2f6bf-414">Um OneNote-Inhalte oder -Strukturen abzurufen, müssen Sie entsprechende Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-414">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="2f6bf-415">Die folgenden Bereiche lassen GET-Anforderungen für Microsoft Graph zu.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-415">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="2f6bf-416">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="2f6bf-416">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="2f6bf-417">Wählen Sie zwischen:</span><span class="sxs-lookup"><span data-stu-id="2f6bf-417">Choose from:</span></span>

- <span data-ttu-id="2f6bf-418">Notes.Read</span><span class="sxs-lookup"><span data-stu-id="2f6bf-418">Notes.read</span></span>
- <span data-ttu-id="2f6bf-419">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f6bf-419">Notes.ReadWrite</span></span>
- <span data-ttu-id="2f6bf-420">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f6bf-420">Notes.ReadWrite.All</span></span>

<span data-ttu-id="2f6bf-421">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f6bf-421">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="2f6bf-422">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2f6bf-422">See also</span></span>

- [<span data-ttu-id="2f6bf-423">Eingabe- und Ausgabe-HTML für OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="2f6bf-423">Input and output HTML for OneNote pages</span></span>](onenote-input-output-html.md)
- [<span data-ttu-id="2f6bf-424">Integrieren in OneNote</span><span class="sxs-lookup"><span data-stu-id="2f6bf-424">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="2f6bf-425">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="2f6bf-425">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="2f6bf-426">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="2f6bf-426">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="2f6bf-427">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="2f6bf-427">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

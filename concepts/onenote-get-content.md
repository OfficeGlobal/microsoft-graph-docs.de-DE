# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="f03d5-101">Abrufen von OneNote-Inhalten und -Strukturen mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f03d5-101">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="f03d5-102">*__Gilt für:__ Privatanwender-Notizbücher auf OneDrive | Enterprise-Notizbücher auf Office 365*</span><span class="sxs-lookup"><span data-stu-id="f03d5-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="f03d5-103">Um OneNote-Inhalte und -Strukturen abzurufen, senden Sie eine GET-Anforderung an den Zielendpunkt.</span><span class="sxs-lookup"><span data-stu-id="f03d5-103">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="f03d5-104">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="f03d5-104">For example:</span></span>

`GET ../onenote/pages/{id}`</p>

<span data-ttu-id="f03d5-105">Wenn die Anforderung erfolgreich ist, gibt Microsoft Graph den HTTP-Statuscode 200 und die Entitäten bzw. Inhalte zurück, die Sie angefordert haben.</span><span class="sxs-lookup"><span data-stu-id="f03d5-105">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="f03d5-106">OneNote-Entitäten werden als JSON-Objekte zurückgegeben, die der Spezifikation der OData-Version 4.0 entsprechen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-106">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="f03d5-107">Mithilfe von Abfragezeichenfolgenoptionen können Sie Ihre Abfragen filtern und die Leistung verbessern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-107">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="f03d5-108">Erstellen des Anforderungs-URI</span><span class="sxs-lookup"><span data-stu-id="f03d5-108">Construct the request</span></span>

<span data-ttu-id="f03d5-109">Um den Anforderungs-URI zu erstellen, beginnen Sie mit der Stamm-URL des Diensts:</span><span class="sxs-lookup"><span data-stu-id="f03d5-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="f03d5-110">Fügen Sie dann den Endpunkt der Ressource an, die Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-110">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="f03d5-111">([Ressourcenpfade](#resource-paths-for-get-requests) werden im nächsten Abschnitt gezeigt.)</span><span class="sxs-lookup"><span data-stu-id="f03d5-111">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>


<span data-ttu-id="f03d5-112">Ihr vollständiger Anforderungs-URI gleicht einem der folgenden Beispiele:</span><span class="sxs-lookup"><span data-stu-id="f03d5-112">Your full request URI will look like one of these examples:</span></span>
- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`</p>

> <span data-ttu-id="f03d5-113">**Hinweis:** Hier erfahren Sie mehr über die [Stamm-URL des Diensts](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="f03d5-113">**Note:** Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="resource-paths"></a>
## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="f03d5-114">Ressourcenpfade für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="f03d5-114">Resource paths for GET requests</span></span>

<span data-ttu-id="f03d5-115">Verwenden Sie die folgenden Ressourcenpfade, um Seiten, Abschnitte, Abschnittsgruppen, Notizbücher und Bild- oder Dateiressourcen abzurufen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-115">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

<span data-ttu-id="f03d5-116">[Page-Sammlung](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Page-Entität](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Seitenvorschau](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[HTML-Inhalt einer Seite](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp;[Section-Sammlung](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Section-Entität](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup-Sammlung](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup-Entität](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook-Sammlung](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook-Entität](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Bild oder andere Dateiressource](#image-or-other-file-resource)</span><span class="sxs-lookup"><span data-stu-id="f03d5-116">[Page collection](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Page entity](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Page preview](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[Page HTML content](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp; [Section collection](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Section entity](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup collection](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp; [SectionGroup entity](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook collection](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook entity](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp; [Image or other file resource](#image-or-other-file-resource)</span></span>

<a name="get-pages"></a>
### <a name="page-collection"></a><span data-ttu-id="f03d5-117">Page-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f03d5-117">Page collection</span></span>

<span data-ttu-id="f03d5-118">Abrufen von Seiten (Metadaten) aus allen Notizbüchern</span><span class="sxs-lookup"><span data-stu-id="f03d5-118">Get pages (metadata) across all notebooks</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<span data-ttu-id="f03d5-119">Abrufen von Seiten (Metadaten) aus einem bestimmten Abschnitt</span><span class="sxs-lookup"><span data-stu-id="f03d5-119">Get pages (metadata) from a specific section</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

 
<span data-ttu-id="f03d5-120">Die `search`-Abfragezeichenfolgenoption ist nur für Heimanwender-Notizbücher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f03d5-120">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="f03d5-121">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-121">The default sort order is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="f03d5-122">Die Standardabfrage erweitert den übergeordneten Abschnitt und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="f03d5-122">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="f03d5-123">Standardmäßig werden nur die ersten 20 Einträge für *GET pages*-Anforderungen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f03d5-123">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="f03d5-124">Anforderungen, die keine **top**-Abfragezeichenfolgenoption enthalten, geben einen **@odata.nextLink**-Link in der Antwort zurück, mit dem Sie die nächsten 20 Einträge abrufen können.</span><span class="sxs-lookup"><span data-stu-id="f03d5-124">GET requests for pages that retrieve the default number of entries (that is, they don’t specify a top expression) return an @odata.nextLink link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="f03d5-125">Verwenden Sie für die Sammlung der Seiten in einem Abschnitt **pagelevel**, um die Einzugsebene von Seiten und ihre Reihenfolge innerhalb des Abschnitts zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="f03d5-125">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

<span data-ttu-id="f03d5-126">**Beispiel:**  `GET ../sections/{section-id}/pages?pagelevel=true`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-126">Example</span></span>

- - -

<a name="get-page"></a> 
### <a name="page-entity"></a><span data-ttu-id="f03d5-127">Page-Entität</span><span class="sxs-lookup"><span data-stu-id="f03d5-127">Page entity</span></span>

<span data-ttu-id="f03d5-128">Abrufen der Metadaten für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="f03d5-128">Get the metadata for a folder.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 


<span data-ttu-id="f03d5-129">Seiten können die Eigenschaften **parentNotebook** und **parentSection** erweitern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-129">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="f03d5-130">Die Standardabfrage erweitert den übergeordneten Abschnitt und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="f03d5-130">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="f03d5-131">Verwenden Sie **pagelevel**, um die Einzugsebene der Seite und ihre Reihenfolge im übergeordneten Abschnitt zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="f03d5-131">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> <span data-ttu-id="f03d5-132">Beispiel: `GET ../pages/{page-id}?pagelevel=true`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-132">Example: `GET ../pages/{page-id}?pagelevel=true`.</span></span>

- - -

<a name="get-page-preview"></a> 
### <a name="page-preview"></a><span data-ttu-id="f03d5-133">Seitenvorschau</span><span class="sxs-lookup"><span data-stu-id="f03d5-133">Page break preview.</span></span>

<span data-ttu-id="f03d5-134">Abrufen von Text- und Bild-Vorschauinhalt für eine Seite</span><span class="sxs-lookup"><span data-stu-id="f03d5-134">Get text and image preview content for a page</span></span>

`../pages/{page-id}/preview`


<span data-ttu-id="f03d5-135">Die JSON-Antwort enthält den Vorschauinhalt, anhand dessen Benutzer feststellen können, was sich auf der Seite befindet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-135">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

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

<span data-ttu-id="f03d5-136">Die **previewText**-Eigenschaft enthält einen Textausschnitt von der Seite.</span><span class="sxs-lookup"><span data-stu-id="f03d5-136">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="f03d5-137">Microsoft Graph gibt vollständige Ausdrücke im Umfang von maximal 300 Zeichen zurück.</span><span class="sxs-lookup"><span data-stu-id="f03d5-137">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="f03d5-138">Wenn die Seite über ein Bild verfügt, das zum Erstellen einer Vorschau der Benutzeroberfläche verwendet werden kann, enthält die **href**-Eigenschaft im **previewImageUrl**-Objekt einen Link zu einer öffentlichen, vorab authentifizierten [Bildressource](#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="f03d5-138">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="f03d5-139">Sie können diesen Link in HTML-Code verwenden.</span><span class="sxs-lookup"><span data-stu-id="f03d5-139">You can use this link in HTML,</span></span>

<span data-ttu-id="f03d5-140">**Beispiel: ** `<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-140">Example</span></span> <span data-ttu-id="f03d5-141">Andernfalls gibt **href** NULL zurück.</span><span class="sxs-lookup"><span data-stu-id="f03d5-141">Otherwise, **href** returns null.</span></span>

- - -

<a name="get-page-content"></a> 
### <a name="page-html-content"></a><span data-ttu-id="f03d5-142">HTML-Inhalt einer Seite</span><span class="sxs-lookup"><span data-stu-id="f03d5-142">Page HTML content</span></span>

<span data-ttu-id="f03d5-143">Abrufen des HTML-Codes einer Seite `../pages/{page-id}/content[?includeIDs,preAuthenticated]`</span><span class="sxs-lookup"><span data-stu-id="f03d5-143">Get the HTML content of a page `../pages/{page-id}/content[?includeIDs,preAuthenticated]`</span></span>

<span data-ttu-id="f03d5-144">(*Weitere Informationen zu [zurückgegebenen HTML-Inhalten](onenote_input_output_html.md)*)</span><span class="sxs-lookup"><span data-stu-id="f03d5-144">(*learn more about [returned HTML content](onenote_input_output_html.md)*)</span></span> 

 
<span data-ttu-id="f03d5-145">Verwenden Sie die Abfragezeichenfolgenoption **includeIDs=true**, um die zum [Aktualisieren der Seite](onenote_update_page.md) generierten IDs abzurufen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-145">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote_update_page.md).</span></span>

<span data-ttu-id="f03d5-146">Verwenden Sie die Abfragezeichenfolgenoption **preAuthenticated=true** zum Abrufen von öffentlichen URLs zu den [Bildressourcen](#image-or-other-file-resource), die sich auf der Seite befinden.</span><span class="sxs-lookup"><span data-stu-id="f03d5-146">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page.</span></span> <span data-ttu-id="f03d5-147">Die öffentlichen URLs sind eine Stunde lang gültig.</span><span class="sxs-lookup"><span data-stu-id="f03d5-147">The public URLs that are returned are valid for one hour.</span></span> 

- - -

<a name="get-sections"></a>
### <a name="section-collection"></a><span data-ttu-id="f03d5-148">Section-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f03d5-148">Section collection</span></span>

<span data-ttu-id="f03d5-149">Abrufen aller Abschnitte aus allen Notizbüchern im Besitz des Benutzers, einschließlich der Abschnitte in geschachtelten Abschnittsgruppen `../sections[?filter,orderby,select,top,skip,expand,count]`</span><span class="sxs-lookup"><span data-stu-id="f03d5-149">Get all sections from all notebooks that are owned by the user, including sections in nested section groups `../sections[?filter,orderby,select,top,skip,expand,count]`</span></span> 

<span data-ttu-id="f03d5-150">Abrufen aller Abschnitte, die sich direkt unter einer bestimmten Abschnittsgruppe befinden</span><span class="sxs-lookup"><span data-stu-id="f03d5-150">Get all sections that are directly under a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="f03d5-151">Abrufen aller Abschnitte, die sich direkt unter einem bestimmten Notizbuch befinden `../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`</span><span class="sxs-lookup"><span data-stu-id="f03d5-151">Get all sections that are directly under a specific notebook `../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`</span></span> 

 
<span data-ttu-id="f03d5-152">Abschnitte können die Eigenschaften **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-152">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="f03d5-153">Die Standardsortierreihenfolge für Abschnitte ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-153">The default sort order is `name asc`.</span></span>

<span data-ttu-id="f03d5-154">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="f03d5-154">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section"></a>
### <a name="section-entity"></a><span data-ttu-id="f03d5-155">Section-Entität</span><span class="sxs-lookup"><span data-stu-id="f03d5-155">Section entity</span></span>

<span data-ttu-id="f03d5-156">Abrufen eines bestimmten Abschnitts</span><span class="sxs-lookup"><span data-stu-id="f03d5-156">Get a specific entity</span></span>

`../sections/{section-id}[?select,expand]` 

 
<span data-ttu-id="f03d5-157">Abschnitte können die Eigenschaften **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-157">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="f03d5-158">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="f03d5-158">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section-groups"></a>
### <a name="sectiongroup-collection"></a><span data-ttu-id="f03d5-159">SectionGroup-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f03d5-159">SectionGroup collection</span></span>

<span data-ttu-id="f03d5-160">Abrufen aller Abschnittsgruppen aus allen Notizbüchern im Besitz des Benutzers, einschließlich geschachtelter Abschnittsgruppen</span><span class="sxs-lookup"><span data-stu-id="f03d5-160">Get all section groups from all notebooks that are owned by the user, including nested section groups</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="f03d5-161">Abrufen aller Abschnittsgruppen, die sich direkt unter einem bestimmten Notizbuch befinden</span><span class="sxs-lookup"><span data-stu-id="f03d5-161">Get all section groups that are directly under a specific notebook</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="f03d5-162">Abschnittsgruppen können die Eigenschaften **sections**, **sectionGroups**, **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-162">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="f03d5-163">Die Standardsortierreihenfolge für Abschnittsgruppen ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-163">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="f03d5-164">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="f03d5-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section-group"></a>
### <a name="sectiongroup-entity"></a><span data-ttu-id="f03d5-165">SectionGroup-Entität</span><span class="sxs-lookup"><span data-stu-id="f03d5-165">SectionGroup entity</span></span>

<span data-ttu-id="f03d5-166">Abrufen einer bestimmten Abschnittsgruppe</span><span class="sxs-lookup"><span data-stu-id="f03d5-166">Get a specific section group and expand its sections and section groups.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 


<span data-ttu-id="f03d5-167">Abschnittsgruppen können die Eigenschaften **sections**, **sectionGroups**, **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-167">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="f03d5-168">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="f03d5-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-notebooks"></a>
### <a name="notebook-collection"></a><span data-ttu-id="f03d5-169">Notebook-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f03d5-169">notebook collection</span></span>

<span data-ttu-id="f03d5-170">Abrufen aller Notizbücher, deren Eigentümer der Benutzer ist</span><span class="sxs-lookup"><span data-stu-id="f03d5-170">Get all the notebooks that are owned by the user</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

 
<span data-ttu-id="f03d5-171">Notizbücher können die Eigenschaften **sections** und **sectionGroups** erweitern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-171">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="f03d5-172">Die Standardsortierreihenfolge für Notizbücher ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-172">The default sort order is `name asc`.</span></span> 

- - -

<a name="get-notebook"></a>
### <a name="notebook-entity"></a><span data-ttu-id="f03d5-173">Notebook-Entität</span><span class="sxs-lookup"><span data-stu-id="f03d5-173">Notebook entity</span></span>

<span data-ttu-id="f03d5-174">Abrufen eines bestimmten Notizbuchs `../notebooks/{notebook-id}[?select,expand]`</span><span class="sxs-lookup"><span data-stu-id="f03d5-174">Get a specific notebook `../notebooks/{notebook-id}[?select,expand]`</span></span> 


<span data-ttu-id="f03d5-175">Notizbücher können die Eigenschaften **sections** und **sectionGroups** erweitern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-175">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

- - -

<a name="get-resource"></a>
### <a name="image-or-other-file-resource"></a><span data-ttu-id="f03d5-176">Bild- oder andere Dateiressource</span><span class="sxs-lookup"><span data-stu-id="f03d5-176">Image or other file resource</span></span>

<span data-ttu-id="f03d5-177">Abrufen der Binärdaten einer bestimmten Ressource</span><span class="sxs-lookup"><span data-stu-id="f03d5-177">Get the binary data of a specific resource by sending a GET request to the resource's  endpoint:</span></span> 

`../resources/{resource-id}/$value` 


<span data-ttu-id="f03d5-178">Sie finden den Ressourcen-URI der Datei im [Ausgabe-HTML-Code](onenote_input_output_html.md) der Seite.</span><span class="sxs-lookup"><span data-stu-id="f03d5-178">You can find the file's resource URI in the page's [output HTML](onenote_input_output_html.md).</span></span>

<span data-ttu-id="f03d5-179">Beispielsweise enthält ein **img**-Tag Endpunkte für das Originalbild im **data-fullres-src**-Attribut und das optimierte Bild im **src**-Attribut.</span><span class="sxs-lookup"><span data-stu-id="f03d5-179">In the page HTML, an **** tag includes endpoints for the original image resource in the **** attribute and the optimized image in the **** attribute:</span></span> 

<span data-ttu-id="f03d5-180">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="f03d5-180">**Example**</span></span>

```
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="f03d5-181">Und ein **object**-Tag enthält den Endpunkt für die Dateiressource im **data**-Attribut.</span><span class="sxs-lookup"><span data-stu-id="f03d5-181">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

<span data-ttu-id="f03d5-182">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="f03d5-182">**Example**</span></span>

```
<object
    data="http://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="f03d5-183">Um öffentliche, vorab authentifizierte URLs für die Bildressourcen auf einer Seite zu erhalten, fügen Sie **preAuthenticated=true** in die Abfragezeichenfolge ein, wenn Sie [die Seiteninhalte abrufen](#page-html-content) (**Beispiel:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="f03d5-183">To get public URLs to the image resources on a page, include preAuthenticated=true in the query string when you retrieve the page content (example: ).</span></span> <span data-ttu-id="f03d5-184">Die öffentlichen URLs, die im [Ausgabe-HTML-Code](onenote_input_output_html.md#output-html-examples-for-images) zurückgegeben werden, sind eine Stunde lang gültig.</span><span class="sxs-lookup"><span data-stu-id="f03d5-184">The public URLs that are returned are valid for one hour.</span></span> <span data-ttu-id="f03d5-185">Ohne dieses Flag können Bilder nicht direkt in einem Browser gerendert werden, da sie wie die restlichen Seiteninhalte privat sind und eine Autorisierung erforderlich ist, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-185">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="f03d5-186">**Hinweis:** Das Abrufen einer Sammlung von Ressourcen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f03d5-186">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="f03d5-187">Beim Abrufen einer Dateiressource müssen Sie keinen **Accept**-Inhaltstyp in der Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="f03d5-187">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="f03d5-188">Weitere Informationen zu GET-Anforderungen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="f03d5-188">For more information about GET requests, see:</span></span> 
- [<span data-ttu-id="f03d5-189">GET Pages</span><span class="sxs-lookup"><span data-stu-id="f03d5-189">Get pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="f03d5-190">GET Sections</span><span class="sxs-lookup"><span data-stu-id="f03d5-190">GET sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="f03d5-191">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="f03d5-191">GET sectiongroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="f03d5-192">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="f03d5-192">GET notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 

<span data-ttu-id="f03d5-193">in der Microsoft Graph-API-REST-Referenz.</span><span class="sxs-lookup"><span data-stu-id="f03d5-193">in the Microsoft Graph API REST reference.</span></span>


<a name="example"></a>
## <a name="example-get-requests"></a><span data-ttu-id="f03d5-194">Beispiele für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="f03d5-194">Example GET requests</span></span>
<span data-ttu-id="f03d5-195">Sie können Abfragen für OneNote-Entitäten stellen und Seiteninhalte durchsuchen, um genau die gesuchten Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-195">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="f03d5-196">Die folgenden Beispiele zeigen einige Verwendungsmöglichkeiten für [unterstützte Abfragezeichenfolgenoptionen](#supported-odata-query-string-options) in GET-Anforderungen für Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f03d5-196">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="f03d5-197">**Zur Erinnerung:**</span><span class="sxs-lookup"><span data-stu-id="f03d5-197">**Remember:**</span></span>

- <span data-ttu-id="f03d5-198">Alle GET-Anforderungen beginnen mit der [Stamm-URL des Diensts](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="f03d5-198">All GET requests start with the service root URL, for example:</span></span>

  <span data-ttu-id="f03d5-199">**Beispiele:**</span><span class="sxs-lookup"><span data-stu-id="f03d5-199">**Examples**</span></span> 
  - `https://www.onenote.com/api/v1.0/me/notes`
  - `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`

- <span data-ttu-id="f03d5-200">Leerzeichen in der URL-Abfragezeichenfolge müssen mit %20 codiert sein.</span><span class="sxs-lookup"><span data-stu-id="f03d5-200">Spaces in the URL query string must be replaced with  the %20 encoding. Example:  filter=isDefault%20eq%20true</span></span>

<span data-ttu-id="f03d5-201">Beispiel: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="f03d5-201">Example: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="f03d5-202">Bei Eigenschaftennamen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-202">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="f03d5-203">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="f03d5-203">Property names and OData string comparisons are case sensitive. We recommend using the OData **tolower** function for string comparisons. Example: filter=tolower(name) eq 'spring'</span></span>

   <span data-ttu-id="f03d5-204">Beispiel: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="f03d5-204">Example: `filter=tolower(name) eq 'spring'`</span></span>
 

<span data-ttu-id="f03d5-205">**search & filter**</span><span class="sxs-lookup"><span data-stu-id="f03d5-205">**search & filter**</span></span>  

<span data-ttu-id="f03d5-206">Abrufen aller Seiten, die den Begriff *recipe* enthalten und von einer bestimmten App erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="f03d5-206">Get all pages that contain the term *recipe* that were created by a specific app.</span></span>  <span data-ttu-id="f03d5-207">(`search` ist nur für Heimanwender-Notizbücher verfügbar)</span><span class="sxs-lookup"><span data-stu-id="f03d5-207">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
<span data-ttu-id="f03d5-208">**search & select**</span><span class="sxs-lookup"><span data-stu-id="f03d5-208">**search & select**</span></span>  

<span data-ttu-id="f03d5-209">Abrufen des Titels, der OneNote-Clientlinks und des **contentUrl**-Links für alle Seiten, die den Begriff *golgi app* enthalten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-209">Get the title, oncshort client links, and contentUrl link for all pages that contain the term golgi app.</span></span>  <span data-ttu-id="f03d5-210">(`search` ist nur für Heimanwender-Notizbücher verfügbar)</span><span class="sxs-lookup"><span data-stu-id="f03d5-210">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
<span data-ttu-id="f03d5-211">**expand**</span><span class="sxs-lookup"><span data-stu-id="f03d5-211">**expand**</span></span>  

<span data-ttu-id="f03d5-212">Abrufen aller Notizbücher und Erweitern ihrer Abschnitte und Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-212">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```
 
<span data-ttu-id="f03d5-213">Abrufen einer bestimmten Abschnittsgruppe und Erweitern ihrer Abschnitte und Abschnittsgruppen:</span><span class="sxs-lookup"><span data-stu-id="f03d5-213">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<span data-ttu-id="f03d5-214">Abrufen einer Seite und Erweitern Ihres übergeordneten Abschnitts und übergeordneten Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="f03d5-214">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

<span data-ttu-id="f03d5-215">**expand** (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="f03d5-215">expand (multiple levels)</span></span>  

<span data-ttu-id="f03d5-216">Abrufen aller Notizbücher und Erweitern ihrer Abschnitte und Abschnittsgruppen sowie aller Abschnitte in jeder Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="f03d5-216">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
><span data-ttu-id="f03d5-217">Das Erweitern übergeordneter Elemente von untergeordneten Entitäten oder das Erweitern von untergeordneten Elementen von übergeordneten Entitäten erstellt einen Zirkelbezug und wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f03d5-217">Expanding parents of child entities or expanding children of parent entities creates a circular reference and  is not supported.</span></span>

 
<span data-ttu-id="f03d5-218">**expand & select** (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="f03d5-218">expand & select (multiple levels)</span></span>  

<span data-ttu-id="f03d5-219">Abrufen des Namens und des **self**-Links für eine bestimmte Abschnittsgruppe sowie des Namens und **self**-Links für alle enthaltenen Abschnitte.</span><span class="sxs-lookup"><span data-stu-id="f03d5-219">Get the name and **self** link for a specific section group, and get the name and self links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```
 
<span data-ttu-id="f03d5-220">Abrufen des Namens und des **self**-Links für alle Abschnitte sowie des Namens und der Erstellungszeit des übergeordneten Notizbuchs jedes Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="f03d5-220">Get the name and **self** link for all sections, and get the name and created time of its parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```
 
<span data-ttu-id="f03d5-221">Abrufen des Titels und der ID für alle Seiten sowie Abrufen des Namens des übergeordneten Abschnitts und des übergeordneten Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="f03d5-221">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

<span data-ttu-id="f03d5-222">**expand & levels** (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="f03d5-222">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="f03d5-223">Abrufen aller Notizbücher, Abschnitte und Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-223">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
<span data-ttu-id="f03d5-224">**filter**</span><span class="sxs-lookup"><span data-stu-id="f03d5-224">**filter**</span></span>  

<span data-ttu-id="f03d5-225">Abrufen aller Abschnitte, die im Oktober 2014 erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="f03d5-225">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<span data-ttu-id="f03d5-226">Abrufen der Seiten, die von einer bestimmten App seit dem 1. Januar 2015 erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="f03d5-226">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

<span data-ttu-id="f03d5-227">**filter & expand**</span><span class="sxs-lookup"><span data-stu-id="f03d5-227">**filter & expand**</span></span>  

<span data-ttu-id="f03d5-228">Abrufen aller Seiten in einem bestimmten Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="f03d5-228">Get all pages in a specific notebook.</span></span> <span data-ttu-id="f03d5-229">Die API gibt standardmäßig 20 Seiten zurück.</span><span class="sxs-lookup"><span data-stu-id="f03d5-229">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<span data-ttu-id="f03d5-230">Abrufen des Namens und des **pagesUrl**-Links für alle Abschnitte aus dem Notizbuch *School*.</span><span class="sxs-lookup"><span data-stu-id="f03d5-230">Get the name and pagesUrl link for all sections in the user's default  notebook.</span></span> <span data-ttu-id="f03d5-231">In OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet. Verwenden Sie daher am besten die **tolower**-Funktion.</span><span class="sxs-lookup"><span data-stu-id="f03d5-231">Get the name and **pagesUrl** link for all sections from the School notebook.  OData string comparisons are case sensitive, so use the tolower function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

<span data-ttu-id="f03d5-232">**filter & select & orderby**</span><span class="sxs-lookup"><span data-stu-id="f03d5-232">**filter & select & orderby**</span></span>   

<span data-ttu-id="f03d5-233">Abrufen des Namens und des **pagesUrl**-Links für alle Abschnitte, die den Ausdruck *spring* im Abschnittsnamen enthalten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-233">Get the name and **pagesUrl** link for  all sections that contain the term *spring* in the section name. Order sections by last modified date.</span></span> <span data-ttu-id="f03d5-234">Sortieren der Abschnitte nach dem Datum der letzten Änderung.</span><span class="sxs-lookup"><span data-stu-id="f03d5-234">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
<span data-ttu-id="f03d5-235">**orderby**</span><span class="sxs-lookup"><span data-stu-id="f03d5-235">**orderby**</span></span>  

<span data-ttu-id="f03d5-236">Abrufen der ersten 20 Seiten, sortiert nach der **createdByAppId**-Eigenschaft und dann nach der letzten Erstellungszeit.</span><span class="sxs-lookup"><span data-stu-id="f03d5-236">Get the first  20 pages ordered by **createdByAppId** property and then by most recent created time. The API returns 20 pages by default.</span></span> <span data-ttu-id="f03d5-237">Die API gibt standardmäßig 20 Seiten zurück.</span><span class="sxs-lookup"><span data-stu-id="f03d5-237">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

<span data-ttu-id="f03d5-238">**search & filter & top**</span><span class="sxs-lookup"><span data-stu-id="f03d5-238">**search & filter & top**</span></span>  

<span data-ttu-id="f03d5-239">Abrufen der fünf neuesten Seiten, die seit dem 1. Januar 2015 erstellt wurden und die den Ausdruck *cell division* enthalten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-239">Get the five  newest pages  created since January 1, 2015 that contain the phrase *cell division. The API returns 20 pages by default with a maximum of 100. The default sort order for pages lastModifiedTime desc*.</span></span> <span data-ttu-id="f03d5-240">Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="f03d5-240">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="f03d5-241">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-241">The default sort order is `lastModifiedTime desc`.</span></span> <span data-ttu-id="f03d5-242">(`search` ist nur für Heimanwender-Notizbücher verfügbar)</span><span class="sxs-lookup"><span data-stu-id="f03d5-242">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

<span data-ttu-id="f03d5-243">**search & filter & top & skip**</span><span class="sxs-lookup"><span data-stu-id="f03d5-243">**search & filter & top & skip**</span></span>  

<span data-ttu-id="f03d5-244">Abrufen der nächsten fünf Seiten im Resultset.</span><span class="sxs-lookup"><span data-stu-id="f03d5-244">Get the next five  pages  in the result set.</span></span> <span data-ttu-id="f03d5-245">(`search` ist nur für Heimanwender-Notizbücher verfügbar)</span><span class="sxs-lookup"><span data-stu-id="f03d5-245">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<span data-ttu-id="f03d5-246">Und der nächsten fünf.</span><span class="sxs-lookup"><span data-stu-id="f03d5-246">And the next five.</span></span> <span data-ttu-id="f03d5-247">(`search` ist nur für Heimanwender-Notizbücher verfügbar)</span><span class="sxs-lookup"><span data-stu-id="f03d5-247">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="f03d5-248">**Hinweis:** Wenn **search** und **filter** auf dieselbe Anforderung angewendet werden, enthält das Ergebnis nur die Entitäten, die beide Kriterien erfüllen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-248">If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
<span data-ttu-id="f03d5-249">**select**</span><span class="sxs-lookup"><span data-stu-id="f03d5-249">**select**</span></span>  

<span data-ttu-id="f03d5-250">Abrufen von Name, Erstellungszeit und **self**-Link für alle Abschnitte in den Notizbüchern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f03d5-250">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<span data-ttu-id="f03d5-251">Abrufen des Titels, der Erstellungszeit und der OneNote-Clientlinks für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="f03d5-251">Get the title, created time, and oncshort client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

<span data-ttu-id="f03d5-252">**select & expand & filter** (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="f03d5-252">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="f03d5-253">Abrufen von Name und **pagesUrl**-Link für alle Abschnitte im Standardnotizbuch des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f03d5-253">Get the name and **pagesUrl** link for all sections in the user's default  notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

<span data-ttu-id="f03d5-254">**top & select & orderby**</span><span class="sxs-lookup"><span data-stu-id="f03d5-254">**top & select & orderby**</span></span>  

<span data-ttu-id="f03d5-255">Abrufen des Titels und des **self**-Links für die ersten 50 Seiten, alphabetisch sortiert nach Titel.</span><span class="sxs-lookup"><span data-stu-id="f03d5-255">Get the title and **self** link for the first 50 pages, ordered alphabetically by title. The API returns 20 entries by default with a maximum of 100. The default sort order for pages lastModifiedTime desc.</span></span> <span data-ttu-id="f03d5-256">Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="f03d5-256">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="f03d5-257">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="f03d5-257">The default sort order is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

<span data-ttu-id="f03d5-258">**skip & top & select & orderby**</span><span class="sxs-lookup"><span data-stu-id="f03d5-258">**skip & top & select & orderby**</span></span>  

<span data-ttu-id="f03d5-p123">Abrufen der Seiten 51 bis 100. Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="f03d5-p123">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="f03d5-261">**Hinweis:** GET-Anforderungen für Seiten, die die Standardanzahl von Einträgen abrufen (d. h., sie enthalten keinen **top**-Ausdruck) geben einen **@odata.nextLink**-Link in der Antwort zurück, mit dem Sie die nächsten 20 Einträge abrufen können.</span><span class="sxs-lookup"><span data-stu-id="f03d5-261">GET requests for **pages** that retrieve the default number of entries (that is, they don’t specify a **top** expression) return an @odata.nextLink link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="query-options"></a>
## <a name="supported-odata-query-string-options"></a><span data-ttu-id="f03d5-262">Unterstützte Optionen für OData-Abfragezeichenfolgen</span><span class="sxs-lookup"><span data-stu-id="f03d5-262">Supported OData query string options</span></span>

<span data-ttu-id="f03d5-263">Beim Senden von GET-Anforderungen an Microsoft Graph können Sie die Abfrage mit Optionen für OData-Abfragezeichenfolgen anpassen und so genau die gewünschten Informationen erhalten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-263">When sending GET requests to the onnvshort API, you can use OData query string options to customize your query and get just the information you need. They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span> <span data-ttu-id="f03d5-264">Sie können auch eine Leistungssteigerung erzielen, indem die Anzahl der Aufrufe an den Dienst und die Größe der Antwortnutzlast reduziert wird.</span><span class="sxs-lookup"><span data-stu-id="f03d5-264">When sending GET requests to the onnvshort API, you can use OData query string options to customize your query and get just the information you need. They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="f03d5-265">**Hinweis:** Zur besseren Lesbarkeit wird in den Beispielen in diesem Artikel nicht die erforderliche Prozentcodierung %20 für Leerzeichen in der URL-Abfragezeichenfolge verwendet: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="f03d5-265">For readability, the examples in this article don't use the  %20`filter=isDefault%20eq%20true` percent-encoding required for spaces in the URL query string. Example:  filter=isDefault%20eq%20true</span></span>
 
| <span data-ttu-id="f03d5-266">Abfrageoption</span><span class="sxs-lookup"><span data-stu-id="f03d5-266">Query option</span></span> | <span data-ttu-id="f03d5-267">Beispiel und Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f03d5-267">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="f03d5-268">count</span><span class="sxs-lookup"><span data-stu-id="f03d5-268">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="f03d5-269">Die Anzahl der Entitäten in der Sammlung.</span><span class="sxs-lookup"><span data-stu-id="f03d5-269">The count of entities in the collection.</span></span> <span data-ttu-id="f03d5-270">Der Wert wird in der Antwort in der **@odata.count**-Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f03d5-270">The count of entities in the collection. The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="f03d5-271">expand</span><span class="sxs-lookup"><span data-stu-id="f03d5-271">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="f03d5-272">Die Navigationseigenschaften, die inline in der Antwort zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-272">The navigation properties to return inline  in the response. The following properties are supported for expand expressions:</span></span> <span data-ttu-id="f03d5-273">Die folgenden Eigenschaften werden für **expand**-Ausdrücke unterstützt:</span><span class="sxs-lookup"><span data-stu-id="f03d5-273">The navigation properties to return inline  in the response. The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="f03d5-274">– Seiten: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="f03d5-274">Pages: 
**parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="f03d5-275">– Abschnitte: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="f03d5-275">Sections: 
**parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="f03d5-276">– Abschnittsgruppen: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="f03d5-276">Section groups: 
**sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="f03d5-277">– Notizbücher: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="f03d5-277">Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="f03d5-278">Standardmäßig erweitern GET-Anforderungen für Seiten **parentSection** und wählen die Eigenschaften **id**, **name** und **self** des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="f03d5-278">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties. Default GET requests for sections and section groups expand both parentNotebook and parentSectionGroup, and select the parents' id, name, and self properties.</span></span> <span data-ttu-id="f03d5-279">Standardmäßig erweitern GET-Anforderungen für Abschnitte und Abschnittsgruppen **parentNotebook** und **parentSectionGroup** und wählen die Eigenschaften **id**, **name** und **self** der übergeordneten Elemente aus.</span><span class="sxs-lookup"><span data-stu-id="f03d5-279">By default, GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties.</span></span> </p><p><span data-ttu-id="f03d5-280">Kann für eine einzelne Entität oder eine Sammlung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="f03d5-280">Can be used  for a single  entity or a collection. Separate  multiple properties with commas. Property names are case sensitive.</span></span> <span data-ttu-id="f03d5-281">Trennen Sie mehrere Eigenschaften durch Kommas.</span><span class="sxs-lookup"><span data-stu-id="f03d5-281">Separate multiple properties with commas.</span></span> <span data-ttu-id="f03d5-282">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-282">Property names are case sensitive.</span></span></p> |   
| <span data-ttu-id="f03d5-283">filter</span><span class="sxs-lookup"><span data-stu-id="f03d5-283">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="f03d5-284">Ein boolescher Ausdruck, der angibt, ob ein Eintrag in das Resultset aufgenommen werden soll.</span><span class="sxs-lookup"><span data-stu-id="f03d5-284">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="f03d5-285">Unterstützt die folgenden OData-Operatoren und -Funktionen:</span><span class="sxs-lookup"><span data-stu-id="f03d5-285">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="f03d5-286">– Vergleichsoperatoren: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span><span class="sxs-lookup"><span data-stu-id="f03d5-286">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="f03d5-287">– Logische Operatoren: **and**, **or**, **not**</span><span class="sxs-lookup"><span data-stu-id="f03d5-287">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="f03d5-288">– Zeichenfolgenfunktionen: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span><span class="sxs-lookup"><span data-stu-id="f03d5-288">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="f03d5-289">Bei [Eigenschaften](#onenote-entity-properties)namen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-289">[Property](#onenote-entity-properties) names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="f03d5-290">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="f03d5-290">Property names and OData string comparisons are case sensitive. We recommend using the OData **tolower** function for string comparisons. Example: filter=tolower(name) eq 'spring'</span></span> <span data-ttu-id="f03d5-291">Beispiel: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="f03d5-291">Example: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="f03d5-292">orderby</span><span class="sxs-lookup"><span data-stu-id="f03d5-292">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="f03d5-293">Die [Eigenschaften](#onenote-entity-properties), nach denen sortiert werden soll, mit einer optionalen Sortierreihenfolge **asc** (Standard) oder **desc**.</span><span class="sxs-lookup"><span data-stu-id="f03d5-293">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span> <span data-ttu-id="f03d5-294">Sie können nach jeder beliebigen Eigenschaft der Entität in der angeforderten Sammlung sortieren.</span><span class="sxs-lookup"><span data-stu-id="f03d5-294">The properties to sort by, with an optional asc (default) or desc sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="f03d5-295">Die Standardsortierreihenfolge für Notizbücher, Abschnittsgruppen und Abschnitte ist `name asc` und für Seiten `lastModifiedTime desc` (zuletzt geänderte Seite zuerst).</span><span class="sxs-lookup"><span data-stu-id="f03d5-295">The default sort order for notebooks, section groups, and sections is name asc`name asc`, and for pages is lastModifiedTime desc`lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="f03d5-296">Trennen Sie mehrere Eigenschaften durch Kommas, und führen Sie sie in der Reihenfolge auf, in der sie angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-296">Separate  multiple properties with commas, and list them in the order that you want them applied. Property names are case sensitive.</span></span> <span data-ttu-id="f03d5-297">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-297">Property names are case sensitive.</span></span></p> |  
| <span data-ttu-id="f03d5-298">search</span><span class="sxs-lookup"><span data-stu-id="f03d5-298">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="f03d5-299">Nur für Heimanwender-Notizbücher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f03d5-299">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="f03d5-300">Der zu suchende Begriff oder Ausdruck im Seitentitel, Seitentext, Alternativtext für Bilder und OCR-Text für Bilder.</span><span class="sxs-lookup"><span data-stu-id="f03d5-300">
The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span> <span data-ttu-id="f03d5-301">Standardmäßig werden die Ergebnisse von Suchabfragen nach Relevanz sortiert zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f03d5-301">By default, search results are sorted by relevance rank.</span></span></p><p><span data-ttu-id="f03d5-302">OneNote verwendet die Bing-Volltextsuche, um die Suche nach Wortgruppen, Wortstammerkennung, Toleranz gegen Rechtschreibfehler, Relevanz und Bewertung, Worttrennung, mehrere Sprachen und andere Volltext-Suchfunktionen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-302">onnvshort uses Bing full text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features. Search strings are case insensitive.</span></span> <span data-ttu-id="f03d5-303">In Suchzeichenfolgen wird die Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-303">Search strings are case insensitive.</span></span></p><p><span data-ttu-id="f03d5-304">Gilt nur für Seiten in Notizbüchern im Besitz des Benutzers (nicht in für den Benutzer freigegebenen).</span><span class="sxs-lookup"><span data-stu-id="f03d5-304">Applies only to pages in notebooks owned by the user (not shared with the user).</span></span> <span data-ttu-id="f03d5-305">Indizierter Inhalt ist privat und nur für den Besitzer zugänglich.</span><span class="sxs-lookup"><span data-stu-id="f03d5-305">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="f03d5-306">Kennwortgeschützte Seiten werden nicht indiziert.</span><span class="sxs-lookup"><span data-stu-id="f03d5-306">Password-protected pages are not indexed.</span></span> <span data-ttu-id="f03d5-307">Gilt nur für den `pages`-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="f03d5-307">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="f03d5-308">select</span><span class="sxs-lookup"><span data-stu-id="f03d5-308">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="f03d5-309">Die [Eigenschaften](#onenote-entity-properties), die zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-309">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="f03d5-310">Kann für eine einzelne Entität oder eine Sammlung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="f03d5-310">Can be used  for  a single  entity or for a collection. Separate  multiple properties with commas. Property names are case sensitive.</span></span> <span data-ttu-id="f03d5-311">Trennen Sie mehrere Eigenschaften durch Kommas.</span><span class="sxs-lookup"><span data-stu-id="f03d5-311">Separate multiple properties with commas.</span></span> <span data-ttu-id="f03d5-312">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-312">Property names are case sensitive.</span></span></p> |  
| <span data-ttu-id="f03d5-313">skip</span><span class="sxs-lookup"><span data-stu-id="f03d5-313">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="f03d5-314">Die Anzahl der Einträge, die im Resultset übersprungen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-314">The number of entries  to skip in the result set. Typically used for paging results.</span></span> <span data-ttu-id="f03d5-315">In der Regel für die Seitenverwaltung der Ergebnisse verwendet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-315">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="f03d5-316">Nach oben</span><span class="sxs-lookup"><span data-stu-id="f03d5-316">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="f03d5-317">Die Anzahl der zurückzugebenden Einträge im Resultset, maximal 100.</span><span class="sxs-lookup"><span data-stu-id="f03d5-317">The number of entries to return in the result set, up to a maximum of 100. The default value for pages is 20.</span></span> <span data-ttu-id="f03d5-318">Der Standardwert ist 20.</span><span class="sxs-lookup"><span data-stu-id="f03d5-318">The default value is 20.</span></span></p> |  

<span data-ttu-id="f03d5-319">Microsoft Graph bietet außerdem die `pagelevel`-Zeichenfolgenoption, mit der Sie die Ebene und die Reihenfolge der Seiten innerhalb des übergeordneten Abschnitts abrufen können.</span><span class="sxs-lookup"><span data-stu-id="f03d5-319">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="f03d5-320">Gilt nur für Abfragen für Seiten in einem bestimmten Abschnitt oder für Abfragen für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="f03d5-320">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

<span data-ttu-id="f03d5-321">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="f03d5-321">**Example**</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="f03d5-322">Unterstützte OData-Operatoren und -Funktionen</span><span class="sxs-lookup"><span data-stu-id="f03d5-322">Supported OData operators and functions</span></span>

<span data-ttu-id="f03d5-323">Microsoft Graph unterstützt die folgenden OData-Operatoren und Funktionen in **filter**-Ausdrücken.</span><span class="sxs-lookup"><span data-stu-id="f03d5-323">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="f03d5-324">Beachten Sie bei der Verwendung von OData-Ausdrücken Folgendes:</span><span class="sxs-lookup"><span data-stu-id="f03d5-324">When using OData expressions, remember:</span></span>  
- <span data-ttu-id="f03d5-325">Leerzeichen in der URL-Abfagezeichenfolge müssen durch die Codierung `%20` ersetzt werden.</span><span class="sxs-lookup"><span data-stu-id="f03d5-325">Spaces in the URL query string must be replaced with  the %20`%20` encoding. Example:  filter=isDefault%20eq%20true</span></span>

   <span data-ttu-id="f03d5-326">**Beispiel:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="f03d5-326">Example</span></span>
- <span data-ttu-id="f03d5-327">Bei Eigenschaftennamen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-327">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="f03d5-328">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="f03d5-328">Property names and OData string comparisons are case sensitive. We recommend using the OData **tolower** function for string comparisons. Example: filter=tolower(name) eq 'spring'</span></span>
   
   <span data-ttu-id="f03d5-329">**Beispiel:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="f03d5-329">Example</span></span>

| <span data-ttu-id="f03d5-330">Vergleichsoperator</span><span class="sxs-lookup"><span data-stu-id="f03d5-330">comparison operator</span></span> | <span data-ttu-id="f03d5-331">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f03d5-331">Example</span></span> |  
|------|------|  
| <span data-ttu-id="f03d5-332">eq</span><span class="sxs-lookup"><span data-stu-id="f03d5-332">eq</span></span><br /><span data-ttu-id="f03d5-333">(gleich)</span><span class="sxs-lookup"><span data-stu-id="f03d5-333">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="f03d5-334">ne</span><span class="sxs-lookup"><span data-stu-id="f03d5-334">ne</span></span><br /><span data-ttu-id="f03d5-335">(nicht gleich)</span><span class="sxs-lookup"><span data-stu-id="f03d5-335">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="f03d5-336">gt</span><span class="sxs-lookup"><span data-stu-id="f03d5-336">gt</span></span><br /><span data-ttu-id="f03d5-337">(größer als)</span><span class="sxs-lookup"><span data-stu-id="f03d5-337">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="f03d5-338">ge</span><span class="sxs-lookup"><span data-stu-id="f03d5-338">ge</span></span><br /><span data-ttu-id="f03d5-339">(größer als oder gleich)</span><span class="sxs-lookup"><span data-stu-id="f03d5-339">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="f03d5-340">lt</span><span class="sxs-lookup"><span data-stu-id="f03d5-340">lt</span></span><br /><span data-ttu-id="f03d5-341">(kleiner als)</span><span class="sxs-lookup"><span data-stu-id="f03d5-341">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="f03d5-342">le</span><span class="sxs-lookup"><span data-stu-id="f03d5-342">le</span></span><br /><span data-ttu-id="f03d5-343">(kleiner als oder gleich)</span><span class="sxs-lookup"><span data-stu-id="f03d5-343">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  
 
| <span data-ttu-id="f03d5-344">Logischer Operator</span><span class="sxs-lookup"><span data-stu-id="f03d5-344">Logical operator</span></span> | <span data-ttu-id="f03d5-345">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f03d5-345">Example</span></span> |  
|------|------|  
| <span data-ttu-id="f03d5-346">und</span><span class="sxs-lookup"><span data-stu-id="f03d5-346">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="f03d5-347">oder</span><span class="sxs-lookup"><span data-stu-id="f03d5-347">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="f03d5-348">not</span><span class="sxs-lookup"><span data-stu-id="f03d5-348">NOT</span></span> | `not contains(tolower(title),'school')` |  
 
| <span data-ttu-id="f03d5-349">String-Funktion</span><span class="sxs-lookup"><span data-stu-id="f03d5-349">String Function</span></span> | <span data-ttu-id="f03d5-350">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f03d5-350">Example</span></span> |  
|------|------|   
| <span data-ttu-id="f03d5-351">contains</span><span class="sxs-lookup"><span data-stu-id="f03d5-351">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="f03d5-352">endswith</span><span class="sxs-lookup"><span data-stu-id="f03d5-352">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="f03d5-353">startswith</span><span class="sxs-lookup"><span data-stu-id="f03d5-353">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="f03d5-354">length</span><span class="sxs-lookup"><span data-stu-id="f03d5-354">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="f03d5-355">indexof</span><span class="sxs-lookup"><span data-stu-id="f03d5-355">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="f03d5-356">substring</span><span class="sxs-lookup"><span data-stu-id="f03d5-356">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="f03d5-357">tolower</span><span class="sxs-lookup"><span data-stu-id="f03d5-357">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="f03d5-358">toupper</span><span class="sxs-lookup"><span data-stu-id="f03d5-358">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="f03d5-359">trim</span><span class="sxs-lookup"><span data-stu-id="f03d5-359">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="f03d5-360">concat</span><span class="sxs-lookup"><span data-stu-id="f03d5-360">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>
## <a name="onenote-entity-properties"></a><span data-ttu-id="f03d5-361">OneNote-Entitätseigenschaften</span><span class="sxs-lookup"><span data-stu-id="f03d5-361">OneNote entity properties</span></span>

<span data-ttu-id="f03d5-362">Die Abfrageausdrücke **filter**, **select**, **expand** und **orderby** können Eigenschaften von OneNote-Entitäten enthalten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-362">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

<span data-ttu-id="f03d5-363">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="f03d5-363">**Example**</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="f03d5-364">Bei Eigenschaftennamen in Abfrageausdrücken wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-364">Property names are case sensitive in query expressions.</span></span>

<span data-ttu-id="f03d5-365">Die Liste der Eigenschaften und Eigenschaftentypen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="f03d5-365">For the list of properties and property types, see:</span></span>

- [<span data-ttu-id="f03d5-366">GET Pages</span><span class="sxs-lookup"><span data-stu-id="f03d5-366">Get pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="f03d5-367">GET Sections</span><span class="sxs-lookup"><span data-stu-id="f03d5-367">GET sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="f03d5-368">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="f03d5-368">GET sectiongroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="f03d5-369">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="f03d5-369">GET notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 

<span data-ttu-id="f03d5-370">in der Microsoft Graph-API-REST-Referenz.</span><span class="sxs-lookup"><span data-stu-id="f03d5-370">in the Microsoft Graph API REST reference.</span></span>

<span data-ttu-id="f03d5-371">Die Abfragezeichenfolgenoption **expand** kann mit folgenden Navigationseigenschaften verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="f03d5-371">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="f03d5-372">Seiten: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="f03d5-372">Pages: 
**parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="f03d5-373">Abschnitte: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="f03d5-373">Sections: 
**parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="f03d5-374">Abschnittsgruppen: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="f03d5-374">Section groups: 
**sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="f03d5-375">Notizbücher: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="f03d5-375">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>
## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="f03d5-376">Anforderungs- and Antwortinformationen für *GET*-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="f03d5-376">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="f03d5-377">Anforderungsdaten</span><span class="sxs-lookup"><span data-stu-id="f03d5-377">Request data</span></span> | <span data-ttu-id="f03d5-378">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f03d5-378">Description</span></span> |  
|------|------|  
| <span data-ttu-id="f03d5-379">Protokoll</span><span class="sxs-lookup"><span data-stu-id="f03d5-379">Protocol</span></span> | <span data-ttu-id="f03d5-380">Alle Anforderungen verwenden das SSL/TLS HTTPS-Protokoll.</span><span class="sxs-lookup"><span data-stu-id="f03d5-380">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="f03d5-381">Header „Authorization“</span><span class="sxs-lookup"><span data-stu-id="f03d5-381">Authorization header</span></span> | <p><span data-ttu-id="f03d5-382">`Bearer {token}`, wobei *{token}* ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</span><span class="sxs-lookup"><span data-stu-id="f03d5-382">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="f03d5-383">Wenn dies fehlt oder ungültig ist, schlägt die Anforderung mit dem Statuscode 401 fehl.</span><span class="sxs-lookup"><span data-stu-id="f03d5-383">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="f03d5-384">Siehe [Authentifizierung und Berechtigungen](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f03d5-384">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="f03d5-385">Header „Accept“</span><span class="sxs-lookup"><span data-stu-id="f03d5-385">accept header</span></span> | <p><span data-ttu-id="f03d5-386">- `application/json` für OneNote-Entitäten und -Entitätenmengen</span><span class="sxs-lookup"><span data-stu-id="f03d5-386">- `application/json` for OneNote entities and entity sets</span></span></p><p><span data-ttu-id="f03d5-387">- `text/html` für Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="f03d5-387">- `text/html` for page content</span></span></p> | 

| <span data-ttu-id="f03d5-388">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="f03d5-388">Response data</span></span> | <span data-ttu-id="f03d5-389">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f03d5-389">Description</span></span> |  
|------|------|  
| <span data-ttu-id="f03d5-390">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="f03d5-390">Success code</span></span> | <span data-ttu-id="f03d5-391">HTTP-Statuscode 200.</span><span class="sxs-lookup"><span data-stu-id="f03d5-391">A 200 (OK) status code.</span></span> |  
| <span data-ttu-id="f03d5-392">Antworttext</span><span class="sxs-lookup"><span data-stu-id="f03d5-392">Response body</span></span> | <span data-ttu-id="f03d5-393">Eine OData-Darstellung der Entität oder der Entitätenmenge im JSON-Format, der HTML-Code der Seite oder Binärdaten der Dateiressource.</span><span class="sxs-lookup"><span data-stu-id="f03d5-393">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="f03d5-394">Fehler</span><span class="sxs-lookup"><span data-stu-id="f03d5-394">Errors</span></span> | <span data-ttu-id="f03d5-395">Wenn die Anforderung nicht erfüllt wird, gibt die API [Fehler](onenote_error_codes.md) im **@api.diagnostics**-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f03d5-395">If the update request fails, the API returns errors in the **api.diagnostics** object in the response body. The request will fail if:</span></span> |  
| <span data-ttu-id="f03d5-396">Header „X-CorrelationId“</span><span class="sxs-lookup"><span data-stu-id="f03d5-396">X-CorrelationId header</span></span> | <span data-ttu-id="f03d5-397">Ein globaler Bezeichner (GUID), über den die Anforderung eindeutig identifiziert wird.</span><span class="sxs-lookup"><span data-stu-id="f03d5-397">A GUID that uniquely identifies a query request.</span></span> <span data-ttu-id="f03d5-398">Sie können diesen Wert zusammen mit dem Wert des Date-Headers verwenden, um zusammen mit dem Microsoft Support Probleme zu behandeln.</span><span class="sxs-lookup"><span data-stu-id="f03d5-398">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>
### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="f03d5-399">Erstellen der Stamm-URL des Microsoft Graph-Notizendiensts</span><span class="sxs-lookup"><span data-stu-id="f03d5-399">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="f03d5-400">Die Stamm-URL des Microsoft Graph-Notizendienses verwendet das folgende Format für alle Aufrufe von Microsoft Graph-Notizen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-400">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes.</span></span> <span data-ttu-id="f03d5-401">`https://graph.microsoft.com/{version}/me/onenote/`  Das `version`-Segment in der URL stellt die Version von Microsoft Graph dar, die Sie verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-401">`https://graph.microsoft.com/{version}/me/onenote/`  The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="f03d5-402">Verwenden Sie `v1.0` für stabilen Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="f03d5-402">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="f03d5-403">Verwenden Sie `beta`, um ein Feature zu testen, das sich in der Entwicklung befindet.</span><span class="sxs-lookup"><span data-stu-id="f03d5-403">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="f03d5-404">Features und Funktionen in der Betaversion ändern sich möglicherweise, sodass Sie es nicht in Ihrem Produktionscode verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="f03d5-404">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> <span data-ttu-id="f03d5-405">Verwenden Sie `me` für OneNote-Inhalt, auf den der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte).</span><span class="sxs-lookup"><span data-stu-id="f03d5-405">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="f03d5-406">Verwenden Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="f03d5-406">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="f03d5-407">Verwenden Sie [Microsoft Graph](https://graph.microsoft.com/v1.0/users), um Benutzer-IDs abzurufen.</span><span class="sxs-lookup"><span data-stu-id="f03d5-407">Use the [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>
## <a name="permissions-for-get-requests"></a><span data-ttu-id="f03d5-408">Berechtigungen für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="f03d5-408">Permissions for GET requests</span></span>

<span data-ttu-id="f03d5-409">Um OneNote-Inhalte oder -Strukturen abzurufen, müssen Sie entsprechende Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="f03d5-409">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="f03d5-410">Die folgenden Bereiche lassen GET-Anforderungen für Microsoft Graph zu.</span><span class="sxs-lookup"><span data-stu-id="f03d5-410">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="f03d5-411">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="f03d5-411">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="f03d5-412">Wählen Sie zwischen:</span><span class="sxs-lookup"><span data-stu-id="f03d5-412">Choose from:</span></span> 
- <span data-ttu-id="f03d5-413">Notes.Read</span><span class="sxs-lookup"><span data-stu-id="f03d5-413">Notes.Read</span></span>
- <span data-ttu-id="f03d5-414">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f03d5-414">Notes.ReadWrite</span></span>
- <span data-ttu-id="f03d5-415">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03d5-415">Notes.ReadWrite.All</span></span>


<span data-ttu-id="f03d5-416">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f03d5-416">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>

<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="f03d5-417">Weitere Ressourcen</span><span class="sxs-lookup"><span data-stu-id="f03d5-417">Additional resources</span></span>

- [<span data-ttu-id="f03d5-418">Eingabe- und Ausgabe-HTML für OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="f03d5-418">Input and output HTML for OneNote pages</span></span>](onenote_input_output_html.md)
- [<span data-ttu-id="f03d5-419">Integrieren in OneNote</span><span class="sxs-lookup"><span data-stu-id="f03d5-419">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="f03d5-420">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="f03d5-420">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="f03d5-421">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="f03d5-421">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="f03d5-422">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="f03d5-422">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="40d0c-101">Abrufen von OneNote-Inhalten und -Strukturen mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="40d0c-101">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="40d0c-102">**Gilt für**: Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365</span><span class="sxs-lookup"><span data-stu-id="40d0c-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="40d0c-103">Um OneNote-Inhalte und -Strukturen abzurufen, senden Sie eine GET-Anforderung an den Zielendpunkt.</span><span class="sxs-lookup"><span data-stu-id="40d0c-103">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="40d0c-104">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="40d0c-104">For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="40d0c-105">Wenn die Anforderung erfolgreich ist, gibt Microsoft Graph den HTTP-Statuscode 200 und die Entitäten bzw. Inhalte zurück, die Sie angefordert haben.</span><span class="sxs-lookup"><span data-stu-id="40d0c-105">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="40d0c-106">OneNote-Entitäten werden als JSON-Objekte zurückgegeben, die der Spezifikation der OData-Version 4.0 entsprechen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-106">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="40d0c-107">Mithilfe von Abfragezeichenfolgenoptionen können Sie Ihre Abfragen filtern und die Leistung verbessern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-107">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="40d0c-108">Erstellen des Anforderungs-URI</span><span class="sxs-lookup"><span data-stu-id="40d0c-108">Construct the request URI</span></span>

<span data-ttu-id="40d0c-109">Um den Anforderungs-URI zu erstellen, beginnen Sie mit der Stamm-URL des Diensts:</span><span class="sxs-lookup"><span data-stu-id="40d0c-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="40d0c-110">Fügen Sie dann den Endpunkt der Ressource an, die Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="40d0c-110">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="40d0c-111">([Ressourcenpfade](#resource-paths-for-get-requests) werden im nächsten Abschnitt gezeigt.)</span><span class="sxs-lookup"><span data-stu-id="40d0c-111">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="40d0c-112">Ihr vollständiger Anforderungs-URI gleicht einem der folgenden Beispiele:</span><span class="sxs-lookup"><span data-stu-id="40d0c-112">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="40d0c-113">**Hinweis:** Hier erfahren Sie mehr über die [Stamm-URL des Diensts](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="40d0c-113">**Note:** Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="40d0c-114">Ressourcenpfade für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="40d0c-114">Resource paths for GET requests</span></span>

<span data-ttu-id="40d0c-115">Verwenden Sie die folgenden Ressourcenpfade, um Seiten, Abschnitte, Abschnittsgruppen, Notizbücher und Bild- oder Dateiressourcen abzurufen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-115">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="40d0c-116">Seitensammlung</span><span class="sxs-lookup"><span data-stu-id="40d0c-116">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="40d0c-117">Seitenentität</span><span class="sxs-lookup"><span data-stu-id="40d0c-117">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="40d0c-118">Seitenvorschau</span><span class="sxs-lookup"><span data-stu-id="40d0c-118">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="40d0c-119">HTML-Inhalt einer Seite</span><span class="sxs-lookup"><span data-stu-id="40d0c-119">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="40d0c-120">Abschnittsammlung</span><span class="sxs-lookup"><span data-stu-id="40d0c-120">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="40d0c-121">Abschnittentität</span><span class="sxs-lookup"><span data-stu-id="40d0c-121">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="40d0c-122">Abschnittsgruppen-Sammlung</span><span class="sxs-lookup"><span data-stu-id="40d0c-122">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="40d0c-123">Abschnittsgruppen-Entität</span><span class="sxs-lookup"><span data-stu-id="40d0c-123">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="40d0c-124">Notebook-Sammlung</span><span class="sxs-lookup"><span data-stu-id="40d0c-124">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="40d0c-125">Notebook-Entität</span><span class="sxs-lookup"><span data-stu-id="40d0c-125">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="40d0c-126">Bild- oder andere Dateiressource</span><span class="sxs-lookup"><span data-stu-id="40d0c-126">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="40d0c-127">Seitensammlung</span><span class="sxs-lookup"><span data-stu-id="40d0c-127">Page collection</span></span>

<span data-ttu-id="40d0c-128">Rufen Sie Seiten (Metadaten) aus allen Notizbüchern ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-128">Get pages (metadata) across all notebooks</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="40d0c-129">Rufen Sie Seiten (Metadaten) aus einem bestimmten Abschnitt ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-129">Get pages (metadata) from a specific section</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="40d0c-130">Die `search`-Abfragezeichenfolgenoption ist nur für Heimanwender-Notizbücher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="40d0c-130">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="40d0c-131">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="40d0c-131">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="40d0c-132">Die Standardabfrage erweitert den übergeordneten Abschnitt und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="40d0c-132">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="40d0c-133">Standardmäßig werden nur die ersten 20 Einträge für *GET pages*-Anforderungen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40d0c-133">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="40d0c-134">Anforderungen, die keine **top**-Abfragezeichenfolgenoption enthalten, geben einen `@odata.nextLink`-Link in der Antwort zurück, mit dem Sie die nächsten 20 Einträge abrufen können.</span><span class="sxs-lookup"><span data-stu-id="40d0c-134">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="40d0c-135">Verwenden Sie für die Sammlung der Seiten in einem Abschnitt **pagelevel**, um die Einzugsebene von Seiten und ihre Reihenfolge innerhalb des Abschnitts zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="40d0c-135">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="40d0c-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-136">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="40d0c-137">Seitenentität</span><span class="sxs-lookup"><span data-stu-id="40d0c-137">Page entity</span></span>

<span data-ttu-id="40d0c-138">Abrufen der Metadaten für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="40d0c-138">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="40d0c-139">Seiten können die Eigenschaften **parentNotebook** und **parentSection** erweitern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-139">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="40d0c-140">Die Standardabfrage erweitert den übergeordneten Abschnitt und wählt die Eigenschaften `id`, `name` und `self` des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="40d0c-140">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="40d0c-141">Verwenden Sie **pagelevel**, um die Einzugsebene der Seite und ihre Reihenfolge im übergeordneten Abschnitt zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="40d0c-141">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="40d0c-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-142">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="40d0c-143">Seitenvorschau</span><span class="sxs-lookup"><span data-stu-id="40d0c-143">Page preview</span></span>

<span data-ttu-id="40d0c-144">Rufen Sie Text- und Bild-Vorschauinhalt für eine Seite ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-144">Get text and image preview content for a page</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="40d0c-145">Die JSON-Antwort enthält den Vorschauinhalt, anhand dessen Benutzer feststellen können, was sich auf der Seite befindet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-145">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

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

<span data-ttu-id="40d0c-146">Die **previewText**-Eigenschaft enthält einen Textausschnitt von der Seite.</span><span class="sxs-lookup"><span data-stu-id="40d0c-146">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="40d0c-147">Microsoft Graph gibt vollständige Ausdrücke im Umfang von maximal 300 Zeichen zurück.</span><span class="sxs-lookup"><span data-stu-id="40d0c-147">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="40d0c-148">Wenn die Seite über ein Bild verfügt, das zum Erstellen einer Vorschau der Benutzeroberfläche verwendet werden kann, enthält die **href**-Eigenschaft im **previewImageUrl**-Objekt einen Link zu einer öffentlichen, vorab authentifizierten [Bildressource](#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="40d0c-148">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="40d0c-149">Sie können diesen Link in HTML-Code verwenden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-149">You can use this link in HTML,</span></span> <span data-ttu-id="40d0c-150">Andernfalls gibt **href** NULL zurück.</span><span class="sxs-lookup"><span data-stu-id="40d0c-150">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="40d0c-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-151">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="40d0c-152">HTML-Inhalt einer Seite</span><span class="sxs-lookup"><span data-stu-id="40d0c-152">Page HTML content</span></span>

<span data-ttu-id="40d0c-153">Rufen Sie den HTML-Code einer Seite ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-153">Get the HTML content of a page </span></span>

`../pages/{page-id}/content[?includeIDs,preAuthenticated]`

<span data-ttu-id="40d0c-154">(*Weitere Informationen zu [zurückgegebenen HTML-Inhalten](onenote_input_output_html.md)*)</span><span class="sxs-lookup"><span data-stu-id="40d0c-154">(*learn more about [returned HTML content](onenote_input_output_html.md)*)</span></span> 

<br/>

<span data-ttu-id="40d0c-155">Verwenden Sie die Abfragezeichenfolgenoption **includeIDs=true**, um die zum [Aktualisieren der Seite](onenote_update_page.md) generierten IDs abzurufen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-155">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote_update_page.md).</span></span>

<span data-ttu-id="40d0c-156">Verwenden Sie die Abfragezeichenfolgenoption **preAuthenticated=true** zum Abrufen von öffentlichen URLs zu den [Bildressourcen](#image-or-other-file-resource), die sich auf der Seite befinden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-156">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page.</span></span> <span data-ttu-id="40d0c-157">Die öffentlichen URLs sind eine Stunde lang gültig.</span><span class="sxs-lookup"><span data-stu-id="40d0c-157">The public URLs are valid for one hour.</span></span> 



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="40d0c-158">Abschnittsammlung</span><span class="sxs-lookup"><span data-stu-id="40d0c-158">Section collection</span></span>

<span data-ttu-id="40d0c-159">Rufen Sie alle Abschnitte aus allen Notizbüchern im Besitz des Benutzers ab, einschließlich der Abschnitte in geschachtelten Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-159">Get all sections from all notebooks that are owned by the user, including sections in nested section groups </span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="40d0c-160">Rufen Sie alle Abschnitte, die sich direkt unter einer bestimmten Abschnittsgruppe befinden ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-160">Get all sections that are directly under a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="40d0c-161">Rufen Sie alle Abschnitte ab, die sich direkt unter einem bestimmten Notizbuch befinden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-161">Get all sections that are directly under a specific notebook </span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="40d0c-162">Abschnitte können die Eigenschaften **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-162">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="40d0c-163">Die Standardsortierreihenfolge für Abschnitte ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="40d0c-163">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="40d0c-164">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="40d0c-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="40d0c-165">Abschnittentität</span><span class="sxs-lookup"><span data-stu-id="40d0c-165">Section entity</span></span>

<span data-ttu-id="40d0c-166">Rufen Sie einen bestimmten Abschnitt ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-166">Get a specific section</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="40d0c-167">Abschnitte können die Eigenschaften **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-167">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="40d0c-168">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="40d0c-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="40d0c-169">Abschnittsgruppen-Sammlung</span><span class="sxs-lookup"><span data-stu-id="40d0c-169">SectionGroup collection</span></span>

<span data-ttu-id="40d0c-170">Rufen Sie alle Abschnittsgruppen aus allen Notizbüchern im Besitz des Benutzers ab, einschließlich geschachtelter Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-170">Get all section groups from all notebooks that are owned by the user, including nested section groups</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="40d0c-171">Rufen Sie alle Abschnittsgruppen ab, die sich direkt unter einem bestimmten Notizbuch befinden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-171">Get all section groups that are directly under a specific notebook</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="40d0c-172">Abschnittsgruppen können die Eigenschaften **sections**, **sectionGroups**, **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-172">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="40d0c-173">Die Standardsortierreihenfolge für Abschnittsgruppen ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="40d0c-173">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="40d0c-174">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="40d0c-174">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="40d0c-175">Abschnittsgruppen-Entität</span><span class="sxs-lookup"><span data-stu-id="40d0c-175">SectionGroup entity</span></span>

<span data-ttu-id="40d0c-176">Rufen Sie eine bestimmte Abschnittsgruppe ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-176">Get a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="40d0c-177">Abschnittsgruppen können die Eigenschaften **sections**, **sectionGroups**, **parentNotebook** und **parentSectionGroup** erweitern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-177">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="40d0c-178">Die Standardabfrage erweitert das übergeordnete Notizbuch und die übergeordnete Abschnittsgruppe und wählt deren Eigenschaften `id`, `name` und `self` aus.</span><span class="sxs-lookup"><span data-stu-id="40d0c-178">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="40d0c-179">Notebook-Sammlung</span><span class="sxs-lookup"><span data-stu-id="40d0c-179">Notebook collection</span></span>

<span data-ttu-id="40d0c-180">Rufen Sie alle Notizbücher ab, deren Eigentümer der Benutzer ist.</span><span class="sxs-lookup"><span data-stu-id="40d0c-180">Get all the notebooks that are owned by the user</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="40d0c-181">Notizbücher können die Eigenschaften **sections** und **sectionGroups** erweitern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-181">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="40d0c-182">Die Standardsortierreihenfolge für Notizbücher ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="40d0c-182">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="40d0c-183">Notebook-Entität</span><span class="sxs-lookup"><span data-stu-id="40d0c-183">Notebook entity</span></span>

<span data-ttu-id="40d0c-184">Rufen Sie ein bestimmtes Notizbuch ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-184">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="40d0c-185">Notizbücher können die Eigenschaften **sections** und **sectionGroups** erweitern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-185">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="40d0c-186">Bild- oder andere Dateiressource</span><span class="sxs-lookup"><span data-stu-id="40d0c-186">Image or other file resource</span></span>

<span data-ttu-id="40d0c-187">Rufen Sie die Binärdaten einer bestimmten Ressource ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-187">Get the binary data of a specific resource</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="40d0c-188">Sie finden den Ressourcen-URI der Datei im [Ausgabe-HTML-Code](onenote_input_output_html.md) der Seite.</span><span class="sxs-lookup"><span data-stu-id="40d0c-188">You can find the file's resource URI in the page's [output HTML](onenote_input_output_html.md).</span></span>

<span data-ttu-id="40d0c-189">Beispielsweise enthält ein **img**-Tag Endpunkte für das Originalbild im **data-fullres-src**-Attribut und das optimierte Bild im **src**-Attribut.</span><span class="sxs-lookup"><span data-stu-id="40d0c-189">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="40d0c-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-190">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="40d0c-191">Und ein **object**-Tag enthält den Endpunkt für die Dateiressource im **data**-Attribut.</span><span class="sxs-lookup"><span data-stu-id="40d0c-191">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="40d0c-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-192">Example</span></span>

```html
<object
    data="http://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="40d0c-193">Um öffentliche, vorab authentifizierte URLs für die Bildressourcen auf einer Seite zu erhalten, fügen Sie `preAuthenticated=true` in die Abfragezeichenfolge ein, wenn Sie [die Seiteninhalte abrufen](#page-html-content) (**Beispiel:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="40d0c-193">To get public, pre-authenticated URLs to the image resources on a page, include `preAuthenticated=true` in the query string when you [retrieve the page content](#page-html-content) (**example:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="40d0c-194">Die öffentlichen URLs, die im [Ausgabe-HTML-Code](onenote_input_output_html.md#output-html-examples-for-images) zurückgegeben werden, sind eine Stunde lang gültig.</span><span class="sxs-lookup"><span data-stu-id="40d0c-194">The public URLs that are returned in the [output HTML](onenote_input_output_html.md#output-html-examples-for-images) are valid for one hour.</span></span> <span data-ttu-id="40d0c-195">Ohne dieses Flag können Bilder nicht direkt in einem Browser gerendert werden, da sie wie die restlichen Seiteninhalte privat sind und eine Autorisierung erforderlich ist, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-195">Without this flag, retrieved images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="40d0c-196">**Hinweis:** Das Abrufen einer Sammlung von Ressourcen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40d0c-196">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="40d0c-197">Beim Abrufen einer Dateiressource müssen Sie keinen **Accept**-Inhaltstyp in der Anforderung angeben.</span><span class="sxs-lookup"><span data-stu-id="40d0c-197">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="40d0c-198">Weitere Informationen über GET-Anforderungen finden Sie unter den folgenden Ressourcen in der Referenz zur Microsoft Graph-API:</span><span class="sxs-lookup"><span data-stu-id="40d0c-198">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="40d0c-199">GET Pages</span><span class="sxs-lookup"><span data-stu-id="40d0c-199">GET Pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="40d0c-200">GET Sections</span><span class="sxs-lookup"><span data-stu-id="40d0c-200">GET Sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="40d0c-201">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="40d0c-201">GET SectionGroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="40d0c-202">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="40d0c-202">GET Notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="40d0c-203">Beispiele für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="40d0c-203">Example GET requests</span></span>

<span data-ttu-id="40d0c-204">Sie können Abfragen für OneNote-Entitäten stellen und Seiteninhalte durchsuchen, um genau die gesuchten Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="40d0c-204">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="40d0c-205">Die folgenden Beispiele zeigen einige Verwendungsmöglichkeiten für [unterstützte Abfragezeichenfolgenoptionen](#supported-odata-query-string-options) in GET-Anforderungen für Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="40d0c-205">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="40d0c-206">**Zur Erinnerung:**</span><span class="sxs-lookup"><span data-stu-id="40d0c-206">**Remember:**</span></span>

- <span data-ttu-id="40d0c-207">Alle GET-Anforderungen beginnen mit der [Stamm-URL des Diensts](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="40d0c-207">All GET requests start with the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span> <br/><br/><span data-ttu-id="40d0c-208">**Beispiele**: `https://www.onenote.com/api/v1.0/me/notes` und `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span><span class="sxs-lookup"><span data-stu-id="40d0c-208">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="40d0c-209">Leerzeichen in der URL-Abfragezeichenfolge müssen mit %20 codiert sein.</span><span class="sxs-lookup"><span data-stu-id="40d0c-209">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="40d0c-210">**Beispiel**: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="40d0c-210">Example: </span></span>

- <span data-ttu-id="40d0c-211">Bei Eigenschaftennamen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-211">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="40d0c-212">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="40d0c-212">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="40d0c-213">**Beispiel**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="40d0c-213">Example: </span></span>
 

### <a name="search--filter"></a><span data-ttu-id="40d0c-214">search & filter</span><span class="sxs-lookup"><span data-stu-id="40d0c-214">search & filter</span></span>  

<span data-ttu-id="40d0c-215">Abrufen aller Seiten, die den Begriff *recipe* enthalten und von einer bestimmten App erstellt wurden (`search` ist nur für Heimanwender-Notizbücher verfügbar).</span><span class="sxs-lookup"><span data-stu-id="40d0c-215">Get all pages that contain the term *recipe* that were created by a specific app.</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="40d0c-216">search & select</span><span class="sxs-lookup"><span data-stu-id="40d0c-216">search & select</span></span>  

<span data-ttu-id="40d0c-217">Abrufen des Titels, der OneNote-Clientlinks und des **contentUrl**-Links für alle Seiten, die den Begriff *golgi app* enthalten (`search` ist nur für Heimanwender-Notizbücher verfügbar).</span><span class="sxs-lookup"><span data-stu-id="40d0c-217">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app*.</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="40d0c-218">expand</span><span class="sxs-lookup"><span data-stu-id="40d0c-218">expand</span></span> 

<span data-ttu-id="40d0c-219">Abrufen aller Notizbücher und Erweitern ihrer Abschnitte und Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-219">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="40d0c-220">Abrufen einer bestimmten Abschnittsgruppe und Erweitern ihrer Abschnitte und Abschnittsgruppen:</span><span class="sxs-lookup"><span data-stu-id="40d0c-220">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="40d0c-221">Abrufen einer Seite und Erweitern Ihres übergeordneten Abschnitts und übergeordneten Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="40d0c-221">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="40d0c-222">expand (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="40d0c-222">expand (multiple levels)</span></span>  

<span data-ttu-id="40d0c-223">Abrufen aller Notizbücher und Erweitern ihrer Abschnitte und Abschnittsgruppen sowie aller Abschnitte in jeder Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="40d0c-223">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="40d0c-224">**Hinweis:** Das Erweitern übergeordneter Elemente von untergeordneten Entitäten oder das Erweitern von untergeordneten Elementen von übergeordneten Entitäten erstellt einen Zirkelbezug und wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40d0c-224">Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="40d0c-225">expand & select (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="40d0c-225">expand & select (multiple levels)</span></span>  

<span data-ttu-id="40d0c-226">Abrufen des Namens und des **self**-Links für eine bestimmte Abschnittsgruppe sowie des Namens und **self**-Links für alle enthaltenen Abschnitte.</span><span class="sxs-lookup"><span data-stu-id="40d0c-226">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="40d0c-227">Abrufen des Namens und des **self**-Links für alle Abschnitte sowie des Namens und der Erstellungszeit des übergeordneten Notizbuchs jedes Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="40d0c-227">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="40d0c-228">Abrufen des Titels und der ID für alle Seiten sowie Abrufen des Namens des übergeordneten Abschnitts und des übergeordneten Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="40d0c-228">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="40d0c-229">expand & levels (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="40d0c-229">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="40d0c-230">Abrufen aller Notizbücher, Abschnitte und Abschnittsgruppen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-230">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="40d0c-231">filter</span><span class="sxs-lookup"><span data-stu-id="40d0c-231">filter</span></span>

<span data-ttu-id="40d0c-232">Abrufen aller Abschnitte, die im Oktober 2014 erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-232">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="40d0c-233">Abrufen der Seiten, die von einer bestimmten App seit dem 1. Januar 2015 erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-233">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="40d0c-234">filter & expand</span><span class="sxs-lookup"><span data-stu-id="40d0c-234">filter & expand</span></span>  

<span data-ttu-id="40d0c-235">Rufen Sie alle Seiten in einem bestimmten Notizbuch ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-235">Get all pages in a specific notebook.</span></span> <span data-ttu-id="40d0c-236">Die API gibt standardmäßig 20 Seiten zurück.</span><span class="sxs-lookup"><span data-stu-id="40d0c-236">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="40d0c-237">Rufen Sie den Namens und den **pagesUrl**-Link für alle Abschnitte aus dem Notizbuch *School* ab.</span><span class="sxs-lookup"><span data-stu-id="40d0c-237">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="40d0c-238">In OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet. Verwenden Sie daher am besten die **tolower**-Funktion.</span><span class="sxs-lookup"><span data-stu-id="40d0c-238">OData string comparisons are case sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="40d0c-239">filter & select & orderby</span><span class="sxs-lookup"><span data-stu-id="40d0c-239">filter & select & orderby</span></span>   

<span data-ttu-id="40d0c-240">Abrufen des Namens und des **pagesUrl**-Links für alle Abschnitte, die den Ausdruck *spring* im Abschnittsnamen enthalten.</span><span class="sxs-lookup"><span data-stu-id="40d0c-240">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="40d0c-241">Sortieren der Abschnitte nach dem Datum der letzten Änderung.</span><span class="sxs-lookup"><span data-stu-id="40d0c-241">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="40d0c-242">orderby</span><span class="sxs-lookup"><span data-stu-id="40d0c-242">orderby</span></span>

<span data-ttu-id="40d0c-243">Abrufen der ersten 20 Seiten, sortiert nach der **createdByAppId**-Eigenschaft und dann nach der letzten Erstellungszeit.</span><span class="sxs-lookup"><span data-stu-id="40d0c-243">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="40d0c-244">Die API gibt standardmäßig 20 Seiten zurück.</span><span class="sxs-lookup"><span data-stu-id="40d0c-244">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="40d0c-245">search & filter & top</span><span class="sxs-lookup"><span data-stu-id="40d0c-245">search & filter & top</span></span> 

<span data-ttu-id="40d0c-246">Abrufen der fünf neuesten Seiten, die seit dem 1. Januar 2015 erstellt wurden und die den Ausdruck *cell division* enthalten.</span><span class="sxs-lookup"><span data-stu-id="40d0c-246">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="40d0c-247">Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="40d0c-247">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="40d0c-248">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc` (`search` ist nur für Heimanwender-Notizbücher verfügbar).</span><span class="sxs-lookup"><span data-stu-id="40d0c-248">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="40d0c-249">search & filter & top & skip</span><span class="sxs-lookup"><span data-stu-id="40d0c-249">search & filter & top & skip</span></span>  

<span data-ttu-id="40d0c-250">Rufen Sie die folgenden fünf Seiten im Resultset ab (`search` ist nur für Heimanwender-Notizbücher verfügbar).</span><span class="sxs-lookup"><span data-stu-id="40d0c-250">Get the next five pages in the result set (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="40d0c-251">Und die folgenden fünf (`search` ist nur für Heimanwender-Notizbücher verfügbar)</span><span class="sxs-lookup"><span data-stu-id="40d0c-251">And the next five (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="40d0c-252">**Hinweis:** Wenn **search** und **filter** auf dieselbe Anforderung angewendet werden, enthält das Ergebnis nur die Entitäten, die beide Kriterien erfüllen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-252">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="40d0c-253">select</span><span class="sxs-lookup"><span data-stu-id="40d0c-253">select</span></span>

<span data-ttu-id="40d0c-254">Abrufen von Name, Erstellungszeit und **self**-Link für alle Abschnitte in den Notizbüchern des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="40d0c-254">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="40d0c-255">Abrufen des Titels, der Erstellungszeit und der OneNote-Clientlinks für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="40d0c-255">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="40d0c-256">select & expand & filter (mehrere Ebenen)</span><span class="sxs-lookup"><span data-stu-id="40d0c-256">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="40d0c-257">Abrufen von Name und **pagesUrl**-Link für alle Abschnitte im Standardnotizbuch des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="40d0c-257">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="40d0c-258">top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="40d0c-258">top & select & orderby</span></span> 

<span data-ttu-id="40d0c-259">Abrufen des Titels und des **self**-Links für die ersten 50 Seiten, alphabetisch sortiert nach Titel.</span><span class="sxs-lookup"><span data-stu-id="40d0c-259">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="40d0c-260">Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="40d0c-260">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="40d0c-261">Die Standardsortierreihenfolge für Seiten ist `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="40d0c-261">The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="40d0c-262">skip & top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="40d0c-262">skip & top & select & orderby</span></span>  

<span data-ttu-id="40d0c-p117">Abrufen der Seiten 51 bis 100. Die API gibt standardmäßig 20 und maximal 100 Einträge zurück.</span><span class="sxs-lookup"><span data-stu-id="40d0c-p117">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="40d0c-265">**Hinweis:** GET-Anforderungen für Seiten, die die Standardanzahl von Einträgen abrufen (d. h., sie enthalten keinen **top**-Ausdruck) geben einen **@odata.nextLink**-Link in der Antwort zurück, mit dem Sie die nächsten 20 Einträge abrufen können.</span><span class="sxs-lookup"><span data-stu-id="40d0c-265">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="40d0c-266">Unterstützte Optionen für OData-Abfragezeichenfolgen</span><span class="sxs-lookup"><span data-stu-id="40d0c-266">Supported OData query string options</span></span>

<span data-ttu-id="40d0c-267">Beim Senden von GET-Anforderungen an Microsoft Graph können Sie die Abfrage mit Optionen für OData-Abfragezeichenfolgen anpassen und so genau die gewünschten Informationen erhalten.</span><span class="sxs-lookup"><span data-stu-id="40d0c-267">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="40d0c-268">Sie können auch eine Leistungssteigerung erzielen, indem die Anzahl der Aufrufe an den Dienst und die Größe der Antwortnutzlast reduziert wird.</span><span class="sxs-lookup"><span data-stu-id="40d0c-268">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="40d0c-269">**Hinweis:** Zur besseren Lesbarkeit wird in den Beispielen in diesem Artikel nicht die erforderliche Prozentcodierung %20 für Leerzeichen in der URL-Abfragezeichenfolge verwendet: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="40d0c-269">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="40d0c-270">Abfrageoption</span><span class="sxs-lookup"><span data-stu-id="40d0c-270">Query option</span></span> | <span data-ttu-id="40d0c-271">Beispiel und Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40d0c-271">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="40d0c-272">count</span><span class="sxs-lookup"><span data-stu-id="40d0c-272">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="40d0c-p119">Die Anzahl der Einträge in der Auflistung. Der Wert wird in der Antwort in der **@odata.count**-Eigenschaft zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40d0c-p119">The count of entities in the collection. The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="40d0c-275">expand</span><span class="sxs-lookup"><span data-stu-id="40d0c-275">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="40d0c-276">Die Navigationseigenschaften, die inline in der Antwort zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-276">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="40d0c-277">Die folgenden Eigenschaften werden für **expand**-Ausdrücke unterstützt:</span><span class="sxs-lookup"><span data-stu-id="40d0c-277">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="40d0c-278">– Seiten: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="40d0c-278">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="40d0c-279">– Abschnitte: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="40d0c-279">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="40d0c-280">– Abschnittsgruppen: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="40d0c-280">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="40d0c-281">– Notizbücher: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="40d0c-281">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="40d0c-282">Standardmäßig erweitern GET-Anforderungen für Seiten **parentSection** und wählen die Eigenschaften **id**, **name** und **self** des Abschnitts aus.</span><span class="sxs-lookup"><span data-stu-id="40d0c-282">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties.</span></span> <span data-ttu-id="40d0c-283">Standardmäßig erweitern GET-Anforderungen für Abschnitte und Abschnittsgruppen **parentNotebook** und **parentSectionGroup** und wählen die Eigenschaften **id**, **name** und **self** der übergeordneten Elemente aus.</span><span class="sxs-lookup"><span data-stu-id="40d0c-283">Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties.</span></span> </p><p><span data-ttu-id="40d0c-284">Kann für eine einzelne Entität oder eine Sammlung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-284">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="40d0c-285">Trennen Sie mehrere Eigenschaften durch Kommas.</span><span class="sxs-lookup"><span data-stu-id="40d0c-285">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="40d0c-286">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-286">Property names are not case-sensitive</span></span></p> |   
| <span data-ttu-id="40d0c-287">filter</span><span class="sxs-lookup"><span data-stu-id="40d0c-287">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="40d0c-288">Ein boolescher Ausdruck, der angibt, ob ein Eintrag in das Resultset aufgenommen werden soll.</span><span class="sxs-lookup"><span data-stu-id="40d0c-288">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="40d0c-289">Unterstützt die folgenden OData-Operatoren und -Funktionen:</span><span class="sxs-lookup"><span data-stu-id="40d0c-289">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="40d0c-290">– Vergleichsoperatoren: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span><span class="sxs-lookup"><span data-stu-id="40d0c-290">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="40d0c-291">– Logische Operatoren: **and**, **or**, **not**</span><span class="sxs-lookup"><span data-stu-id="40d0c-291">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="40d0c-292">– Zeichenfolgenfunktionen: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span><span class="sxs-lookup"><span data-stu-id="40d0c-292">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="40d0c-293">Bei [Eigenschaften](#onenote-entity-properties)namen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-293">[Property](#onenote-entity-properties) names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="40d0c-294">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="40d0c-294">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="40d0c-295">**Beispiel**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="40d0c-295">Example: </span></span></p> |  
| <span data-ttu-id="40d0c-296">orderby</span><span class="sxs-lookup"><span data-stu-id="40d0c-296">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="40d0c-p124">Die [Eigenschaften](#onenote-entity-properties), nach denen sortiert werden soll, mit einer optionalen Sortierreihenfolge **asc** (Standard) oder **desc**. Sie können nach jeder beliebigen Eigenschaft der Entität in der angeforderten Auflistung sortieren.</span><span class="sxs-lookup"><span data-stu-id="40d0c-p124">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="40d0c-299">Die Standardsortierreihenfolge für Notizbücher, Abschnittsgruppen und Abschnitte ist `name asc` und für Seiten `lastModifiedTime desc` (zuletzt geänderte Seite zuerst).</span><span class="sxs-lookup"><span data-stu-id="40d0c-299">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="40d0c-300">Trennen Sie mehrere Eigenschaften durch Kommas, und führen Sie sie in der Reihenfolge auf, in der sie angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-300">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="40d0c-301">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-301">Property names are not case-sensitive</span></span></p> |  
| <span data-ttu-id="40d0c-302">search</span><span class="sxs-lookup"><span data-stu-id="40d0c-302">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="40d0c-303">Nur für Heimanwender-Notizbücher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="40d0c-303">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="40d0c-p126">Der zu suchende Begriff oder Ausdruck im Seitentitel, Seitentext, Alternativtext für Bilder und OCR-Text für Bilder. Standardmäßig werden die Ergebnisse von Suchabfragen nach Relevanz sortiert zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40d0c-p126">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="40d0c-306">OneNote verwendet die Bing-Volltextsuche, um die Suche nach Wortgruppen, Wortstammerkennung, Toleranz gegen Rechtschreibfehler, Relevanz und Bewertung, Worttrennung, mehrere Sprachen und andere Volltext-Suchfunktionen zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-306">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="40d0c-307">In Suchzeichenfolgen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-307">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="40d0c-308">Gilt nur für Seiten in Notizbüchern im Besitz des Benutzers (nicht in für den Benutzer freigegebenen).</span><span class="sxs-lookup"><span data-stu-id="40d0c-308">Applies only to pages in notebooks owned by the user (not shared with the user).</span></span> <span data-ttu-id="40d0c-309">Indizierter Inhalt ist privat und nur für den Besitzer zugänglich.</span><span class="sxs-lookup"><span data-stu-id="40d0c-309">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="40d0c-310">Kennwortgeschützte Seiten werden nicht indiziert.</span><span class="sxs-lookup"><span data-stu-id="40d0c-310">Password-protected pages are not indexed.</span></span> <span data-ttu-id="40d0c-311">Gilt nur für den `pages`-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="40d0c-311">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="40d0c-312">select</span><span class="sxs-lookup"><span data-stu-id="40d0c-312">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="40d0c-313">Die [Eigenschaften](#onenote-entity-properties), die zurückgegeben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-313">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="40d0c-314">Kann für eine einzelne Entität oder eine Sammlung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-314">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="40d0c-315">Trennen Sie mehrere Eigenschaften durch Kommas.</span><span class="sxs-lookup"><span data-stu-id="40d0c-315">Separate multiple properties with commas.</span></span> <span data-ttu-id="40d0c-316">Bei Eigenschaftennamen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-316">Property names are not case-sensitive</span></span></p> |  
| <span data-ttu-id="40d0c-317">skip</span><span class="sxs-lookup"><span data-stu-id="40d0c-317">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="40d0c-318">Die Anzahl der Einträge, die im Resultset übersprungen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-318">The number of entries to skip in the result set.</span></span> <span data-ttu-id="40d0c-319">In der Regel für die Seitenverwaltung der Ergebnisse verwendet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-319">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="40d0c-320">Nach oben</span><span class="sxs-lookup"><span data-stu-id="40d0c-320">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="40d0c-321">Die Anzahl der zurückzugebenden Einträge im Resultset, maximal 100.</span><span class="sxs-lookup"><span data-stu-id="40d0c-321">The number of entries to return in the result set, up to a maximum of 100.</span></span> <span data-ttu-id="40d0c-322">Der Standardwert ist 20.</span><span class="sxs-lookup"><span data-stu-id="40d0c-322">The default value is 20.</span></span></p> |  

<span data-ttu-id="40d0c-323">Microsoft Graph bietet außerdem die `pagelevel`-Zeichenfolgenoption, mit der Sie die Ebene und die Reihenfolge der Seiten innerhalb des übergeordneten Abschnitts abrufen können.</span><span class="sxs-lookup"><span data-stu-id="40d0c-323">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="40d0c-324">Gilt nur für Abfragen für Seiten in einem bestimmten Abschnitt oder für Abfragen für eine bestimmte Seite.</span><span class="sxs-lookup"><span data-stu-id="40d0c-324">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="40d0c-325">Beispiele</span><span class="sxs-lookup"><span data-stu-id="40d0c-325">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="40d0c-326">Unterstützte OData-Operatoren und -Funktionen</span><span class="sxs-lookup"><span data-stu-id="40d0c-326">Supported OData operators and functions</span></span>

<span data-ttu-id="40d0c-327">Microsoft Graph unterstützt die folgenden OData-Operatoren und Funktionen in **filter**-Ausdrücken.</span><span class="sxs-lookup"><span data-stu-id="40d0c-327">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="40d0c-328">Beachten Sie bei der Verwendung von OData-Ausdrücken Folgendes:</span><span class="sxs-lookup"><span data-stu-id="40d0c-328">When using OData expressions, remember:</span></span>

- <span data-ttu-id="40d0c-329">Leerzeichen in der URL-Abfagezeichenfolge müssen durch die Codierung `%20` ersetzt werden.</span><span class="sxs-lookup"><span data-stu-id="40d0c-329">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="40d0c-330">**Beispiel:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="40d0c-330">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="40d0c-331">Bei Eigenschaftennamen und OData-Zeichenfolgenvergleichen wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-331">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="40d0c-332">Wir empfehlen die Verwendung der OData-Funktion **tolower** für Zeichenfolgenvergleiche.</span><span class="sxs-lookup"><span data-stu-id="40d0c-332">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="40d0c-333">**Beispiel:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="40d0c-333">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="40d0c-334">Vergleichsoperator</span><span class="sxs-lookup"><span data-stu-id="40d0c-334">Comparison operator</span></span> | <span data-ttu-id="40d0c-335">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-335">Example</span></span> |  
|------|------|  
| <span data-ttu-id="40d0c-336">eq</span><span class="sxs-lookup"><span data-stu-id="40d0c-336">eq</span></span><br /><span data-ttu-id="40d0c-337">(gleich)</span><span class="sxs-lookup"><span data-stu-id="40d0c-337">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="40d0c-338">ne</span><span class="sxs-lookup"><span data-stu-id="40d0c-338">ne</span></span><br /><span data-ttu-id="40d0c-339">(nicht gleich)</span><span class="sxs-lookup"><span data-stu-id="40d0c-339">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="40d0c-340">gt</span><span class="sxs-lookup"><span data-stu-id="40d0c-340">gt</span></span><br /><span data-ttu-id="40d0c-341">(größer als)</span><span class="sxs-lookup"><span data-stu-id="40d0c-341">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="40d0c-342">ge</span><span class="sxs-lookup"><span data-stu-id="40d0c-342">ge</span></span><br /><span data-ttu-id="40d0c-343">(größer als oder gleich)</span><span class="sxs-lookup"><span data-stu-id="40d0c-343">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="40d0c-344">lt</span><span class="sxs-lookup"><span data-stu-id="40d0c-344">lt</span></span><br /><span data-ttu-id="40d0c-345">(kleiner als)</span><span class="sxs-lookup"><span data-stu-id="40d0c-345">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="40d0c-346">le</span><span class="sxs-lookup"><span data-stu-id="40d0c-346">le</span></span><br /><span data-ttu-id="40d0c-347">(kleiner als oder gleich)</span><span class="sxs-lookup"><span data-stu-id="40d0c-347">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="40d0c-348">Logischer Operator</span><span class="sxs-lookup"><span data-stu-id="40d0c-348">Logical operator</span></span> | <span data-ttu-id="40d0c-349">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-349">Example</span></span> |  
|------|------|  
| <span data-ttu-id="40d0c-350">und</span><span class="sxs-lookup"><span data-stu-id="40d0c-350">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="40d0c-351">oder</span><span class="sxs-lookup"><span data-stu-id="40d0c-351">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="40d0c-352">not</span><span class="sxs-lookup"><span data-stu-id="40d0c-352">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="40d0c-353">String-Funktion</span><span class="sxs-lookup"><span data-stu-id="40d0c-353">String function</span></span> | <span data-ttu-id="40d0c-354">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-354">Example</span></span> |  
|------|------|   
| <span data-ttu-id="40d0c-355">contains</span><span class="sxs-lookup"><span data-stu-id="40d0c-355">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="40d0c-356">endswith</span><span class="sxs-lookup"><span data-stu-id="40d0c-356">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="40d0c-357">startswith</span><span class="sxs-lookup"><span data-stu-id="40d0c-357">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="40d0c-358">length</span><span class="sxs-lookup"><span data-stu-id="40d0c-358">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="40d0c-359">indexof</span><span class="sxs-lookup"><span data-stu-id="40d0c-359">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="40d0c-360">substring</span><span class="sxs-lookup"><span data-stu-id="40d0c-360">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="40d0c-361">tolower</span><span class="sxs-lookup"><span data-stu-id="40d0c-361">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="40d0c-362">toupper</span><span class="sxs-lookup"><span data-stu-id="40d0c-362">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="40d0c-363">trim</span><span class="sxs-lookup"><span data-stu-id="40d0c-363">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="40d0c-364">concat</span><span class="sxs-lookup"><span data-stu-id="40d0c-364">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="40d0c-365">OneNote-Entitätseigenschaften</span><span class="sxs-lookup"><span data-stu-id="40d0c-365">OneNote entity properties</span></span>

<span data-ttu-id="40d0c-366">Die Abfrageausdrücke **filter**, **select**, **expand** und **orderby** können Eigenschaften von OneNote-Entitäten enthalten.</span><span class="sxs-lookup"><span data-stu-id="40d0c-366">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="40d0c-367">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40d0c-367">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="40d0c-368">Bei Eigenschaftennamen in Abfrageausdrücken wird die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-368">Property names are case sensitive in query expressions.</span></span>

<span data-ttu-id="40d0c-369">Die Liste der Eigenschaften und Eigenschaftentypen finden Sie unter den folgenden Ressourcen in der Referenz zur Microsoft Graph-API:</span><span class="sxs-lookup"><span data-stu-id="40d0c-369">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="40d0c-370">GET Pages</span><span class="sxs-lookup"><span data-stu-id="40d0c-370">GET Pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="40d0c-371">GET Sections</span><span class="sxs-lookup"><span data-stu-id="40d0c-371">GET Sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="40d0c-372">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="40d0c-372">GET SectionGroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="40d0c-373">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="40d0c-373">GET Notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 



<span data-ttu-id="40d0c-374">Die Abfragezeichenfolgenoption **expand** kann mit folgenden Navigationseigenschaften verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="40d0c-374">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="40d0c-375">Seiten: **parentNotebook**, **parentSection**</span><span class="sxs-lookup"><span data-stu-id="40d0c-375">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="40d0c-376">Abschnitte: **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="40d0c-376">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="40d0c-377">Abschnittsgruppen: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="40d0c-377">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="40d0c-378">Notizbücher: **sections**, **sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="40d0c-378">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="40d0c-379">Anforderungs- and Antwortinformationen für *GET*-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="40d0c-379">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="40d0c-380">Anforderungsdaten</span><span class="sxs-lookup"><span data-stu-id="40d0c-380">Request data</span></span> | <span data-ttu-id="40d0c-381">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40d0c-381">Description</span></span> |  
|------|------|  
| <span data-ttu-id="40d0c-382">Protokoll</span><span class="sxs-lookup"><span data-stu-id="40d0c-382">Protocol</span></span> | <span data-ttu-id="40d0c-383">Alle Anforderungen verwenden das SSL/TLS HTTPS-Protokoll.</span><span class="sxs-lookup"><span data-stu-id="40d0c-383">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="40d0c-384">Header „Authorization“</span><span class="sxs-lookup"><span data-stu-id="40d0c-384">Authorization header</span></span> | <p><span data-ttu-id="40d0c-385">`Bearer {token}`, wobei `{token}` ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</span><span class="sxs-lookup"><span data-stu-id="40d0c-385">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="40d0c-386">Wenn dies fehlt oder ungültig ist, schlägt die Anforderung mit dem Statuscode 401 fehl.</span><span class="sxs-lookup"><span data-stu-id="40d0c-386">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="40d0c-387">Siehe [Authentifizierung und Berechtigungen](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="40d0c-387">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="40d0c-388">Header „Accept“</span><span class="sxs-lookup"><span data-stu-id="40d0c-388">Accept header</span></span> | <p> <span data-ttu-id="40d0c-389">`application/json` für OneNote-Entitäten und -Entitätenmengen</span><span class="sxs-lookup"><span data-stu-id="40d0c-389">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="40d0c-390">`text/html` für Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="40d0c-390">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="40d0c-391">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="40d0c-391">Response data</span></span> | <span data-ttu-id="40d0c-392">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40d0c-392">Description</span></span> |  
|------|------|  
| <span data-ttu-id="40d0c-393">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="40d0c-393">Success code</span></span> | <span data-ttu-id="40d0c-394">HTTP-Statuscode 200.</span><span class="sxs-lookup"><span data-stu-id="40d0c-394">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="40d0c-395">Antworttext</span><span class="sxs-lookup"><span data-stu-id="40d0c-395">Response body</span></span> | <span data-ttu-id="40d0c-396">Eine OData-Darstellung der Entität oder der Entitätenmenge im JSON-Format, der HTML-Code der Seite oder Binärdaten der Dateiressource.</span><span class="sxs-lookup"><span data-stu-id="40d0c-396">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="40d0c-397">Fehler</span><span class="sxs-lookup"><span data-stu-id="40d0c-397">Errors</span></span> | <span data-ttu-id="40d0c-398">Wenn die Anforderung nicht erfüllt wird, gibt die API [Fehler](onenote_error_codes.md) im **@api.diagnostics**-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="40d0c-398">If the request fails, the API returns [errors](onenote_error_codes.md) in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="40d0c-399">Header „X-CorrelationId“</span><span class="sxs-lookup"><span data-stu-id="40d0c-399">X-CorrelationId header</span></span> | <span data-ttu-id="40d0c-400">Ein globaler Bezeichner (GUID), über den die Anforderung eindeutig identifiziert wird.</span><span class="sxs-lookup"><span data-stu-id="40d0c-400">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="40d0c-401">Sie können diesen Wert zusammen mit dem Wert des Date-Headers verwenden, um zusammen mit dem Microsoft Support Probleme zu behandeln.</span><span class="sxs-lookup"><span data-stu-id="40d0c-401">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="40d0c-402">Erstellen der Stamm-URL des Microsoft Graph-Notizendiensts</span><span class="sxs-lookup"><span data-stu-id="40d0c-402">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="40d0c-403">Die Stamm-URL des Microsoft Graph-Notizendienses verwendet das folgende Format für alle Aufrufe von Microsoft Graph-Notizen:</span><span class="sxs-lookup"><span data-stu-id="40d0c-403">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes.</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="40d0c-404">Das Segment `version` in der URL ist die Version von Microsoft Graph, die verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="40d0c-404">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="40d0c-405">Verwenden Sie `v1.0` für stabilen Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="40d0c-405">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="40d0c-406">Verwenden Sie `beta`, um ein Feature zu testen, das sich in der Entwicklung befindet.</span><span class="sxs-lookup"><span data-stu-id="40d0c-406">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="40d0c-407">Features und Funktionen in der Betaversion ändern sich möglicherweise, sodass Sie es nicht in Ihrem Produktionscode verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="40d0c-407">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="40d0c-408">Verwenden Sie `me` für OneNote-Inhalt, auf den der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte).</span><span class="sxs-lookup"><span data-stu-id="40d0c-408">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="40d0c-409">Verwenden Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="40d0c-409">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="40d0c-410">Verwenden Sie [Microsoft Graph](https://graph.microsoft.com/v1.0/users), um Benutzer-IDs abzurufen.</span><span class="sxs-lookup"><span data-stu-id="40d0c-410">Use the [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="40d0c-411">Berechtigungen für GET-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="40d0c-411">Permissions for GET requests</span></span>

<span data-ttu-id="40d0c-412">Um OneNote-Inhalte oder -Strukturen abzurufen, müssen Sie entsprechende Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="40d0c-412">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="40d0c-413">Die folgenden Bereiche lassen GET-Anforderungen für Microsoft Graph zu.</span><span class="sxs-lookup"><span data-stu-id="40d0c-413">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="40d0c-414">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="40d0c-414">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="40d0c-415">Wählen Sie zwischen:</span><span class="sxs-lookup"><span data-stu-id="40d0c-415">Choose from:</span></span>

- <span data-ttu-id="40d0c-416">Notes.Read</span><span class="sxs-lookup"><span data-stu-id="40d0c-416">Notes.read</span></span>
- <span data-ttu-id="40d0c-417">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40d0c-417">Notes.ReadWrite</span></span>
- <span data-ttu-id="40d0c-418">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40d0c-418">Notes.ReadWrite.All</span></span>

<span data-ttu-id="40d0c-419">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="40d0c-419">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="40d0c-420">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="40d0c-420">See also</span></span>

- [<span data-ttu-id="40d0c-421">Eingabe- und Ausgabe-HTML für OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="40d0c-421">Input and output HTML for OneNote pages</span></span>](onenote_input_output_html.md)
- [<span data-ttu-id="40d0c-422">Integrieren in OneNote</span><span class="sxs-lookup"><span data-stu-id="40d0c-422">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="40d0c-423">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="40d0c-423">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="40d0c-424">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="40d0c-424">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="40d0c-425">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="40d0c-425">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

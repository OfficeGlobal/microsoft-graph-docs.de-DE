# <a name="update-onenote-page-content"></a><span data-ttu-id="c4673-101">Aktualisieren der Inhalte von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="c4673-101">Update OneNote page content</span></span>

<span data-ttu-id="c4673-102">*__Gilt für:__ Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365*</span><span class="sxs-lookup"><span data-stu-id="c4673-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>


<span data-ttu-id="c4673-103">Sollen die Inhalte einer OneNote-Seite aktualisiert werden, senden Sie eine PATCH-Anforderung an den Endpunkt *content* der Seite:</span><span class="sxs-lookup"><span data-stu-id="c4673-103">To retrieve the HTML content of a onnvshort page, you send a GET request to  the page's content endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="c4673-104">Im Anforderungstext senden Sie ein JSON-Änderungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="c4673-104">Send a JSON change object in the message body.</span></span> <span data-ttu-id="c4673-105">Wird die Anforderung erfolgreich ausgeführt, gibt Microsoft Graph den HTTP-Statuscode 204 zurück.</span><span class="sxs-lookup"><span data-stu-id="c4673-105">If the create request is successful, the onnvshort API returns a 201 HTTP status code.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="c4673-106">Zusammensetzen des Anforderungs-URI</span><span class="sxs-lookup"><span data-stu-id="c4673-106">Construct the request</span></span>

<span data-ttu-id="c4673-107">Beginnen Sie bei der Zusammensetzung des Anforderungs-URI mit der Stamm-URL des Diensts:</span><span class="sxs-lookup"><span data-stu-id="c4673-107">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="c4673-108">Fügen Sie dann den Endpunkt *content* der Seite an:</span><span class="sxs-lookup"><span data-stu-id="c4673-108">Then append the page's *content* endpoint:</span></span>

<span data-ttu-id="c4673-109">**Abrufen des HTML-Codes der Seite und aller definierten Werte des Typs *data-id***</span><span class="sxs-lookup"><span data-stu-id="c4673-109">**Get the page HTML and all defined *data-id* values**</span></span></p>
`../pages/{id}/content`   

<span data-ttu-id="c4673-110">**Abrufen des HTML-Codes der Seite, aller definierten Werte des Typs *data-id* und aller generierten Werte des Typs *id***</span><span class="sxs-lookup"><span data-stu-id="c4673-110">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span>  
`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="c4673-111">Die Werte des Typs **data-id** und des Typs **id** dienen als Bezeichner für die Elemente mit dem Attribut **target**, also die Elemente, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c4673-111">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="c4673-112">Der vollständige Anforderungs-URI sieht so aus:</span><span class="sxs-lookup"><span data-stu-id="c4673-112">Your full request URI will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="c4673-113">Weitere Informationen zur Stamm-URL des Service finden Sie unter [diesem Link](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="c4673-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>


<a name="message-body"></a>
## <a name="construct-the-message-body"></a><span data-ttu-id="c4673-114">Erstellen des Anforderungstexts</span><span class="sxs-lookup"><span data-stu-id="c4673-114">Construct the message body</span></span>

<span data-ttu-id="c4673-115">Der HTML-Code einer OneNote-Seite enthält Text, Bilder und andere Inhalte, die in Strukturen wie Elementen des Typs **div**, **img** oder **ol** organisiert sind.</span><span class="sxs-lookup"><span data-stu-id="c4673-115">The HTML of a onnvshort page contains text, images, and other content organized into structures such as div, img, and ol elements. To update page HTML, you send a PATCH request to the page's content endpoint:</span></span> <span data-ttu-id="c4673-116">Sollen die Inhalte einer OneNote-Seite aktualisiert werden, fügen Sie der Seite HTML-Elemente hinzu oder ersetzen vorhandene HTML-Elemente.</span><span class="sxs-lookup"><span data-stu-id="c4673-116">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="c4673-117">Ihre Änderungen werden als Array von JSON-Änderungsobjekten im Anforderungstext gesendet.</span><span class="sxs-lookup"><span data-stu-id="c4673-117">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="c4673-118">Jedes Objekt definiert das Zielelement, neue HTML-Inhalte und die auf die Inhalte anzuwendende Aktion.</span><span class="sxs-lookup"><span data-stu-id="c4673-118">Your changes are sent in the request body as an array of JSON objects. Each object specifies the target element,  new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="c4673-p104">Das folgende Array definiert zwei Änderungen. Bei der ersten wird ein Bild über einem Absatz als gleichgeordnetes Element eingefügt, bei der zweiten wird ein Element an eine Liste als letztes untergeordnetes Element angefügt.</span><span class="sxs-lookup"><span data-stu-id="c4673-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

<span data-ttu-id="c4673-121">Weitere Beispiele finden Sie [hier](#example-requests).</span><span class="sxs-lookup"><span data-stu-id="c4673-121">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="c4673-122">Attribute für JSON-Änderungsobjekte</span><span class="sxs-lookup"><span data-stu-id="c4673-122">Attributes for JSON objects</span></span>

<span data-ttu-id="c4673-123">JSON-Objekte für PATCH-Anforderungen werden mithilfe der Attribute **target**, **action**, **position** und **content** definiert.</span><span class="sxs-lookup"><span data-stu-id="c4673-123">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

<span data-ttu-id="c4673-124">**target**</span><span class="sxs-lookup"><span data-stu-id="c4673-124">**target**</span></span>  
<span data-ttu-id="c4673-p105">Das zu aktualisierende Element. Der Wert muss einer der folgenden Bezeichner sein:</span><span class="sxs-lookup"><span data-stu-id="c4673-p105">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="c4673-127">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="c4673-127">Identifier</span></span> | <span data-ttu-id="c4673-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4673-128">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c4673-129">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="c4673-129">data-id</span></span> | <p><span data-ttu-id="c4673-130">Diese ID wird bei der [Erstellung einer Seite](onenote-create-page.md) oder der [Aktualisierung einer Seite](onenote_update_page.md) optional den Elementen im Eingabe-HTML-Code zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="c4673-130">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote_update_page.md).</span></span> <span data-ttu-id="c4673-131">Setzen Sie vor den Wert als Präfix das Symbol #.</span><span class="sxs-lookup"><span data-stu-id="c4673-131">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="c4673-132">Beispiel: `'target':'#intro'` legt das Element `<div data-id="intro" ...>` als Ziel fest.</span><span class="sxs-lookup"><span data-stu-id="c4673-132">Example: `'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="c4673-133">id</span><span class="sxs-lookup"><span data-stu-id="c4673-133">id</span></span> | <p><span data-ttu-id="c4673-134">Hierbei handelt es sich um die von Microsoft Graph [generierte ID](#generated-ids). Sie ist für die meisten Ersetzungsvorgänge erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4673-134">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="c4673-135">Setzen Sie hier kein Symbol # als Präfix.</span><span class="sxs-lookup"><span data-stu-id="c4673-135">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="c4673-136">Beispiel: `'target':'div:{33f8a2...}{37}'` legt das Element `<div id="div:{33f8a2...}{37}" ...>` als Ziel fest.</span><span class="sxs-lookup"><span data-stu-id="c4673-136">Example: `'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="c4673-137">Verwechseln Sie IDs dieses Typs nicht mit den Werten des Typs **id** im [Eingabe-HTML-Code](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="c4673-137">Don't confuse these with any **id** values defined in the [input HTML](onenote_input_output_html.md).</span></span> <span data-ttu-id="c4673-138">Alle im Eingabe-HTML-Code gesendeten Werte des Typs **id** werden verworfen.</span><span class="sxs-lookup"><span data-stu-id="c4673-138">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="c4673-139">body</span><span class="sxs-lookup"><span data-stu-id="c4673-139">body</span></span> | <span data-ttu-id="c4673-140">Das Schlüsselwort, dass als Ziel das erste „div“-Element auf der Seite festlegt.</span><span class="sxs-lookup"><span data-stu-id="c4673-140">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="c4673-141">Setzen Sie hier kein Symbol # als Präfix.</span><span class="sxs-lookup"><span data-stu-id="c4673-141">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="c4673-142">title</span><span class="sxs-lookup"><span data-stu-id="c4673-142">title</span></span> | <span data-ttu-id="c4673-143">Das Schlüsselwort, das als Ziel den Seitentitel festlegt.</span><span class="sxs-lookup"><span data-stu-id="c4673-143">The keyword that targets the page title.</span></span> <span data-ttu-id="c4673-144">Setzen Sie hier kein Symbol # als Präfix.</span><span class="sxs-lookup"><span data-stu-id="c4673-144">Do not prefix with a #.</span></span> |  
 
<span data-ttu-id="c4673-145">**action**</span><span class="sxs-lookup"><span data-stu-id="c4673-145">**action**</span></span>  
<span data-ttu-id="c4673-146">Die auf das Zielelement anzuwendende Aktion.</span><span class="sxs-lookup"><span data-stu-id="c4673-146">The action to perform on the target element. Possible values are: , , , , or .</span></span> <span data-ttu-id="c4673-147">Details finden Sie im Abschnitt [Unterstützte Elemente und Aktionen](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="c4673-147">See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="c4673-148">Aktion</span><span class="sxs-lookup"><span data-stu-id="c4673-148">Action</span></span> | <span data-ttu-id="c4673-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4673-149">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c4673-150">append</span><span class="sxs-lookup"><span data-stu-id="c4673-150">Append</span></span> | <p><span data-ttu-id="c4673-151">Fügt den angegebenen Inhalt als erstes oder letztes untergeordnetes Element zum Ziel hinzu, je nach dem im Attribut **position** festgelegten Wert.</span><span class="sxs-lookup"><span data-stu-id="c4673-151">**append**Adds the supplied content to the target as a first or last child, as determined by the position attribute.Applies only to body, div, ol, and ul elements.</span></span></p><p><span data-ttu-id="c4673-152">Kann nur auf Elemente des Typs **body**, **div**, **ol** oder **ul** angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="c4673-152">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="c4673-153">insert</span><span class="sxs-lookup"><span data-stu-id="c4673-153">insert</span></span> | <span data-ttu-id="c4673-154">Fügt den angegebenen Inhalt als gleichgeordnetes Element vor oder nach dem Ziel hinzu, je nach dem im Attribut **position** festgelegten Wert.</span><span class="sxs-lookup"><span data-stu-id="c4673-154">**insert**Adds the supplied content as a sibling before or after the target, as determined by the position attribute.</span></span> |  
| <span data-ttu-id="c4673-155">prepend</span><span class="sxs-lookup"><span data-stu-id="c4673-155">prepend</span></span> | <p><span data-ttu-id="c4673-156">Fügt den angegebenen Inhalt als erstes untergeordnetes Element zum Ziel hinzu.</span><span class="sxs-lookup"><span data-stu-id="c4673-156">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="c4673-157">Kurzbefehl als Ersatz für **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="c4673-157">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="c4673-158">Kann nur auf Elemente des Typs **body**, **div**, **ol** oder **ul** angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="c4673-158">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="c4673-159">replace</span><span class="sxs-lookup"><span data-stu-id="c4673-159">replace</span></span> | <p><span data-ttu-id="c4673-160">Ersetzt das Ziel durch den angegebenen Inhalt.</span><span class="sxs-lookup"><span data-stu-id="c4673-160">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="c4673-161">Für die meisten Aktionen des Typs **replace** muss das Ziel in Form der [generierten ID](#generated-ids) angegeben werden. (Ausnahme: Elemente des Typs **img** oder **object** innerhalb eines „div“-Elements. Sie können auch per **data-id** angegeben werden.)</span><span class="sxs-lookup"><span data-stu-id="c4673-161">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
<span data-ttu-id="c4673-162">**position**</span><span class="sxs-lookup"><span data-stu-id="c4673-162">**position**</span></span>  
<span data-ttu-id="c4673-163">Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement.</span><span class="sxs-lookup"><span data-stu-id="c4673-163">The location to add the supplied content, relative to the target element. Possible values are:  (default) or .</span></span> <span data-ttu-id="c4673-164">Wird kein Wert angegeben, wird der Standardwert **after** gesetzt.</span><span class="sxs-lookup"><span data-stu-id="c4673-164">Defaults to **render** if omitted.</span></span>

| <span data-ttu-id="c4673-165">Position</span><span class="sxs-lookup"><span data-stu-id="c4673-165">Position</span></span> | <span data-ttu-id="c4673-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4673-166">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c4673-167">after (Standard)</span><span class="sxs-lookup"><span data-stu-id="c4673-167">after (default)</span></span> | <p><span data-ttu-id="c4673-168">- Mit **append**: das letzte untergeordnete Element des Zielelements</span><span class="sxs-lookup"><span data-stu-id="c4673-168">- With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="c4673-169">- Mit **insert**: das nachfolgende gleichgeordnete Element des Zielelements</span><span class="sxs-lookup"><span data-stu-id="c4673-169">**after** (default)- With append: The last child of the target element.- With insert: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="c4673-170">before</span><span class="sxs-lookup"><span data-stu-id="c4673-170">Before.</span></span> | <p><span data-ttu-id="c4673-171">- Mit **append**: das erste untergeordnete Element des Zielelements</span><span class="sxs-lookup"><span data-stu-id="c4673-171">- With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="c4673-172">- Mit **insert**: das vorhergehende gleichgeordnete Element des Zielelements</span><span class="sxs-lookup"><span data-stu-id="c4673-172">**before**- With append: The first child of the target element.- With insert: The preceding sibling of the target element.</span></span></p> |

<span data-ttu-id="c4673-173">**content**</span><span class="sxs-lookup"><span data-stu-id="c4673-173">**content**</span></span>  
<span data-ttu-id="c4673-174">Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten.</span><span class="sxs-lookup"><span data-stu-id="c4673-174">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the  content type with a "Commands" part.</span></span> <span data-ttu-id="c4673-175">Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` in einem Teil „Commands“ gesendet werden (siehe [Beispiel](#multipart-request-with-binary-content)).</span><span class="sxs-lookup"><span data-stu-id="c4673-175">A string of well-formed HTML to add to the page and any image or file binary data. If the content contains binary data, the request must be sent using the multipart/form-data`multipart/form-data` content type with a "Commands" part (see an  [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="c4673-176">Generierte IDs</span><span class="sxs-lookup"><span data-stu-id="c4673-176">Generated IDs</span></span>
<span data-ttu-id="c4673-177">Microsoft Graph generiert Werte des Typs **id** für alle Seitenelemente, die aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="c4673-177">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="c4673-178">Abrufen können Sie die generierten IDs über den Abfragezeichenfolgenausdruck `includeIDs=true` in der GET-Anforderung:</span><span class="sxs-lookup"><span data-stu-id="c4673-178">The onnvshort API generates id`includeIDs=true` values for page elements that can be updated. To get generated IDs, use the includeIDs=true query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="c4673-179">**Hinweis:** Die API verwirft alle Werte des Typs **id**, die im [Eingabe-HTML-Code](onenote_input_output_html.md) von Anforderungen des Typs „create-page“ oder „update-page“ angegeben sind.</span><span class="sxs-lookup"><span data-stu-id="c4673-179">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote_input_output_html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="c4673-180">Das folgende Beispiel zeigt generierte IDs für einen Absatz und ein Bild im [Ausgabe-HTML-Code](onenote_input_output_html.md) einer Seite.</span><span class="sxs-lookup"><span data-stu-id="c4673-180">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote_input_output_html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="c4673-181">Generierte **id**-Werte ändern sich nach dem Aktualisieren einer Seite möglicherweise, Sie sollten daher die aktuellen Werte abrufen, bevor Sie eine PATCH-Anforderung erstellen, die diese verwendet.</span><span class="sxs-lookup"><span data-stu-id="c4673-181">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="c4673-182">Angeben können Sie Zielelemente in Form eines Werts des Typs **data-id** oder eines Werts des Typs **id**. Dabei gilt:</span><span class="sxs-lookup"><span data-stu-id="c4673-182">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="c4673-183">Bei Aktionen des Typs **append** oder des Typs **insert** können Sie beide ID-Typen als Zielwert verwenden.</span><span class="sxs-lookup"><span data-stu-id="c4673-183">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="c4673-184">Bei Aktionen des Typs **replace** müssen Sie für alle Elemente die generierte ID verwenden. Ausgenommen hiervon sind lediglich der Seitentitel sowie Bilder und Objekte innerhalb von „div“-Elementen.</span><span class="sxs-lookup"><span data-stu-id="c4673-184">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div. To replace a title, use the title keyword. To replace images and objects that are within a div, use either data-id or id.</span></span> 
    - <span data-ttu-id="c4673-185">Ersetzen eines Titels: Verwenden Sie das Schlüsselwort **title**.</span><span class="sxs-lookup"><span data-stu-id="c4673-185">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="c4673-186">Ersetzen von Bildern und Objekten in einem „div“-Element: Verwenden Sie entweder **data-id** oder **id**.</span><span class="sxs-lookup"><span data-stu-id="c4673-186">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="c4673-187">Im folgenden Beispiel wird das Ziel in Form eines Werts des Typs **id** angegeben.</span><span class="sxs-lookup"><span data-stu-id="c4673-187">The following example uses the **id** value for the target . Don't use the # prefix with a generated ID.</span></span> <span data-ttu-id="c4673-188">Setzen Sie vor generierten IDs niemals das Präfix #.</span><span class="sxs-lookup"><span data-stu-id="c4673-188">The following example uses the id value for the target . Don't use the # prefix with a generated ID.</span></span>

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a><span data-ttu-id="c4673-189">Unterstützte Elemente und Aktionen</span><span class="sxs-lookup"><span data-stu-id="c4673-189">Supported elements and actions</span></span>
<span data-ttu-id="c4673-190">Viele Elemente auf einer Seite lassen sich aktualisieren, doch unterstützt jeder Elementtyp nur bestimmte Aktionen.</span><span class="sxs-lookup"><span data-stu-id="c4673-190">Many elements on  the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span> <span data-ttu-id="c4673-191">In der folgenden Tabelle sind die unterstützten Zielelemente aufgeführt sowie die Aktualisierungsaktionen, die sie unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c4673-191">Many elements on  the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="c4673-192">Element</span><span class="sxs-lookup"><span data-stu-id="c4673-192">Element</span></span> | <span data-ttu-id="c4673-193">Ersetzen</span><span class="sxs-lookup"><span data-stu-id="c4673-193">Replace</span></span> | <span data-ttu-id="c4673-194">Untergeordnetes Element anfügen</span><span class="sxs-lookup"><span data-stu-id="c4673-194">Append child</span></span> | <span data-ttu-id="c4673-195">Gleichgeordnetes Element einfügen</span><span class="sxs-lookup"><span data-stu-id="c4673-195">Insert sibling</span></span> |  
|------|------|------|------|  
| <span data-ttu-id="c4673-196">body</span><span class="sxs-lookup"><span data-stu-id="c4673-196">body</span></span><br /> <span data-ttu-id="c4673-197">(Ziel: erstes „div“-Element auf der Seite)</span><span class="sxs-lookup"><span data-stu-id="c4673-197">body(targets first div on the page)</span></span> | <span data-ttu-id="c4673-198">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-198">no</span></span> | <span data-ttu-id="c4673-199">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-199">**yes**</span></span> | <span data-ttu-id="c4673-200">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-200">no</span></span> |  
| <span data-ttu-id="c4673-201">div</span><span class="sxs-lookup"><span data-stu-id="c4673-201">div</span></span><br /> <span data-ttu-id="c4673-202">([absolut positioniert](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="c4673-202">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="c4673-203">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-203">no</span></span> | <span data-ttu-id="c4673-204">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-204">**yes**</span></span> | <span data-ttu-id="c4673-205">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-205">no</span></span> |  
| <span data-ttu-id="c4673-206">div</span><span class="sxs-lookup"><span data-stu-id="c4673-206">div</span></span><br /> <span data-ttu-id="c4673-207">(in einem anderen „div“-Element)</span><span class="sxs-lookup"><span data-stu-id="c4673-207">(within a div)</span></span> | <span data-ttu-id="c4673-208">**Ja** (nur per „id“)</span><span class="sxs-lookup"><span data-stu-id="c4673-208">**yes** (id only)</span></span> | <span data-ttu-id="c4673-209">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-209">**Yes**</span></span> | <span data-ttu-id="c4673-210">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-210">**Yes**</span></span> |   
| <span data-ttu-id="c4673-211">img, object</span><span class="sxs-lookup"><span data-stu-id="c4673-211">img, object</span></span><br /> <span data-ttu-id="c4673-212">(in einem anderen „div“-Element)</span><span class="sxs-lookup"><span data-stu-id="c4673-212">(within a div)</span></span> | <span data-ttu-id="c4673-213">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-213">**yes**</span></span> | <span data-ttu-id="c4673-214">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-214">no</span></span> | <span data-ttu-id="c4673-215">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-215">**yes**</span></span> |   
| <span data-ttu-id="c4673-216">ol, ul</span><span class="sxs-lookup"><span data-stu-id="c4673-216">ol, ul</span></span> | <span data-ttu-id="c4673-217">**Ja** (nur per „id“)</span><span class="sxs-lookup"><span data-stu-id="c4673-217">**yes** (id only)</span></span> | <span data-ttu-id="c4673-218">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-218">**Yes**</span></span> | <span data-ttu-id="c4673-219">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-219">**yes**</span></span> |   
| <span data-ttu-id="c4673-220">table</span><span class="sxs-lookup"><span data-stu-id="c4673-220">table</span></span> | <span data-ttu-id="c4673-221">**Ja** (nur per „id“)</span><span class="sxs-lookup"><span data-stu-id="c4673-221">**yes** (id only)</span></span> | <span data-ttu-id="c4673-222">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-222">no</span></span> | <span data-ttu-id="c4673-223">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-223">**yes**</span></span> |   
| <span data-ttu-id="c4673-224">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="c4673-224">p, li, h1-h6</span></span> | <span data-ttu-id="c4673-225">**Ja** (nur per „id“)</span><span class="sxs-lookup"><span data-stu-id="c4673-225">**yes** (id only)</span></span> | <span data-ttu-id="c4673-226">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-226">no</span></span> | <span data-ttu-id="c4673-227">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-227">**yes**</span></span> |   
| <span data-ttu-id="c4673-228">title</span><span class="sxs-lookup"><span data-stu-id="c4673-228">title</span></span> | <span data-ttu-id="c4673-229">**Ja**</span><span class="sxs-lookup"><span data-stu-id="c4673-229">**yes**</span></span> | <span data-ttu-id="c4673-230">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-230">no</span></span> | <span data-ttu-id="c4673-231">Nein</span><span class="sxs-lookup"><span data-stu-id="c4673-231">no</span></span> |  
 

<span data-ttu-id="c4673-232">Die folgenden Elemente unterstützen keinerlei Aktualisierungsaktionen:</span><span class="sxs-lookup"><span data-stu-id="c4673-232">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="c4673-233">img ([absolut positioniert](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="c4673-233">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="c4673-234">object ([absolut positioniert](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="c4673-234">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="c4673-235">tr, td</span><span class="sxs-lookup"><span data-stu-id="c4673-235">tr, td</span></span>
- <span data-ttu-id="c4673-236">meta</span><span class="sxs-lookup"><span data-stu-id="c4673-236">meta</span></span>
- <span data-ttu-id="c4673-237">head</span><span class="sxs-lookup"><span data-stu-id="c4673-237">head</span></span>
- <span data-ttu-id="c4673-238">span</span><span class="sxs-lookup"><span data-stu-id="c4673-238">span</span></span>
- <span data-ttu-id="c4673-239">a</span><span class="sxs-lookup"><span data-stu-id="c4673-239">a</span></span>
- <span data-ttu-id="c4673-240">„style“-Tags</span><span class="sxs-lookup"><span data-stu-id="c4673-240">style tags</span></span>


<a name="examples"></a>
## <a name="example-requests"></a><span data-ttu-id="c4673-241">Beispielanforderungen</span><span class="sxs-lookup"><span data-stu-id="c4673-241">Example requests</span></span>
<span data-ttu-id="c4673-242">Eine Aktualisierungsanforderung enthält eine oder mehrere Änderungen, jeweils dargestellt als JSON-Änderungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="c4673-242">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="c4673-243">Diese Objekte können unterschiedliche Ziele auf der Seite sowie unterschiedliche Aktionen und Inhalte für diese Ziele definieren.</span><span class="sxs-lookup"><span data-stu-id="c4673-243">An update request contains one or more changes represented as JSON objects. These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="c4673-244">Die folgenden Beispiele zeigen JSON-Objekte, die in PATCH-Anforderungen verwendet werden, sowie vollständige PATCH-Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="c4673-244">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

<span data-ttu-id="c4673-245">[Anfügen von untergeordneten Elementen](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Einfügen von gleichgeordneten Elementen](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Ersetzen von Elementen](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Vollständige PATCH-Anforderungen:](#complete-patch-request-examples)</span><span class="sxs-lookup"><span data-stu-id="c4673-245">[Append child elements](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Insert sibling elements](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Replace elements](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Complete PATCH requests](#complete-patch-request-examples)</span></span>


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="c4673-246">Anfügen von untergeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="c4673-246">Append  child elements</span></span>
<span data-ttu-id="c4673-247">Die Aktion **append** fügt einem Element des Typs **body**, **div** (innerhalb eines anderen „div“-Elements), **ol** oder **ul** ein untergeordnetes Element hinzu.</span><span class="sxs-lookup"><span data-stu-id="c4673-247">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element. The position attribute determines whether to append the child before or after the target. The default position is after.</span></span> <span data-ttu-id="c4673-248">Das Attribut **position** legt fest, ob das untergeordnete Element vor oder nach dem Ziel angefügt wird.</span><span class="sxs-lookup"><span data-stu-id="c4673-248">The **position** attribute determines whether to append the child before or after the target.</span></span> <span data-ttu-id="c4673-249">Die Standardposition ist **after**.</span><span class="sxs-lookup"><span data-stu-id="c4673-249">The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="c4673-250">Anfügen an ein „div“-Element</span><span class="sxs-lookup"><span data-stu-id="c4673-250">Append to a  div</span></span>

<span data-ttu-id="c4673-251">Das folgende Beispiel fügt dem Element **div1** zwei untergeordnete Knoten hinzu.</span><span class="sxs-lookup"><span data-stu-id="c4673-251">The following example adds two child nodes  to the **div1** element. It adds an image as the first child and a paragraph as the last child.</span></span> <span data-ttu-id="c4673-252">Als erstes untergeordnetes Element wird ein Bild hinzugefügt, als letztes untergeordnetes Element ein Absatz.</span><span class="sxs-lookup"><span data-stu-id="c4673-252">The following example adds two child nodes  to the div1 element. It adds an image as the first child and a paragraph as the last child.</span></span> 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="c4673-253">Anfügen an das *body*-Element</span><span class="sxs-lookup"><span data-stu-id="c4673-253">Append to the body element</span></span>

<span data-ttu-id="c4673-254">Sie können **body** als schnellen Weg verwenden, um ein untergeordnetes Element im ersten „div“-Element auf der Seite anzufügen.</span><span class="sxs-lookup"><span data-stu-id="c4673-254">You can use the body target as a shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="c4673-255">Im folgenden Beispiel werden dem ersten „div“-Element auf der Seite zwei Absätze hinzugefügt, einer als erstes untergeordnetes Element und einer als letztes untergeordnetes Element.</span><span class="sxs-lookup"><span data-stu-id="c4673-255">The following example adds two paragraphs as the first child and the last child to the first div on the page. Don't use a # with the body target. This example uses the prepend shortcut for append + before.</span></span> <span data-ttu-id="c4673-256">Setzen Sie vor ein Ziel des Typs **body** niemals das Präfix #.</span><span class="sxs-lookup"><span data-stu-id="c4673-256">Don't use a # with the **body** target.</span></span> <span data-ttu-id="c4673-257">In diesem Beispiel verwenden wir die Aktion **prepend** als Kurzversion von **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="c4673-257">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a><span data-ttu-id="c4673-258">Anfügen an eine Liste</span><span class="sxs-lookup"><span data-stu-id="c4673-258">Append to a list</span></span>

<span data-ttu-id="c4673-259">Im folgenden Beispiel wird der Zielliste ein Listenelement als letztes untergeordnetes Element hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c4673-259">The following example adds a list item as a last child to the target list. The list-style-type property is defined because the item uses a non-default list style.</span></span> <span data-ttu-id="c4673-260">Die Eigenschaft **list-style-type** wird angegeben, weil das Element ein anderes Listenformat als das Standardlistenformat verwendet.</span><span class="sxs-lookup"><span data-stu-id="c4673-260">The following example adds a list item as a last child to the target list. The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a><span data-ttu-id="c4673-261">Einfügen von gleichgeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="c4673-261">Insert sibling elements</span></span>
<span data-ttu-id="c4673-262">Die Aktion **insert** fügt dem Zielelement ein gleichgeordnetes Element hinzu.</span><span class="sxs-lookup"><span data-stu-id="c4673-262">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="c4673-263">Das Attribut **position** legt fest, ob das gleichgeordnete Element vor oder nach dem Ziel eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="c4673-263">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="c4673-264">Die Standardposition ist **after**.</span><span class="sxs-lookup"><span data-stu-id="c4673-264">The default position is **after**.</span></span> <span data-ttu-id="c4673-265">In diesem Abschnitt finden Sie alle [Elemente, die **insert** unterstützen](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="c4673-265">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

<span data-ttu-id="c4673-266">**Einfügen von gleichgeordneten Elementen**</span><span class="sxs-lookup"><span data-stu-id="c4673-266">**Insert siblings**</span></span>

<span data-ttu-id="c4673-267">Das folgende Beispiel fügt der Seite zwei gleichgeordnete Knoten hinzu.</span><span class="sxs-lookup"><span data-stu-id="c4673-267">The following example adds two sibling nodes to the page.</span></span> <span data-ttu-id="c4673-268">Es werden ein Bild über dem Element **para1** und ein Absatz unter dem Element **para2** hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="c4673-268">The following example adds two sibling nodes to the page. It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a><span data-ttu-id="c4673-269">Ersetzen von Elementen</span><span class="sxs-lookup"><span data-stu-id="c4673-269">Replace elements</span></span>

<span data-ttu-id="c4673-270">Sie können entweder den Wert **data-id** oder den generierten Wert **id** als Zielwert nutzen, wenn Sie Elemente des Typs **img** oder **object** in einem „div“-Element ersetzen möchten.</span><span class="sxs-lookup"><span data-stu-id="c4673-270">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div. To replace the page title, use the title keyword. For all other elements that support replace, you must use the generated ID.</span></span> <span data-ttu-id="c4673-271">Verwenden Sie das Schlüsselwort **title**, wenn der Seitentitel ersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c4673-271">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="c4673-272">Bei allen anderen [Elementen, die **replace** unterstützen](#supported-elements-and-actions), müssen Sie die generierte ID verwenden.</span><span class="sxs-lookup"><span data-stu-id="c4673-272">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="c4673-273">Ersetzen eines Bilds</span><span class="sxs-lookup"><span data-stu-id="c4673-273">Replace an image</span></span>

<span data-ttu-id="c4673-274">Im folgenden Beispiel wird ein Bild durch ein „div“-Element ersetzt. Als Zielwert wird der Wert **data-id** des Bilds verwendet.</span><span class="sxs-lookup"><span data-stu-id="c4673-274">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="c4673-275">Aktualisieren einer Tabelle</span><span class="sxs-lookup"><span data-stu-id="c4673-275">Update a table</span></span> 

<span data-ttu-id="c4673-276">In diesem Beispiel wird gezeigt, wie eine Tabelle mithilfe ihrer generierten ID aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="c4673-276">This example shows how to update a table by using its generated ID. Replacing tr and td elements is not supported, but you can replace the entire table.</span></span> <span data-ttu-id="c4673-277">Das Ersetzen von Elementen des Typs **tr** und des Typs **td** wird nicht unterstützt. Sie können jedoch die gesamte Tabelle ersetzen.</span><span class="sxs-lookup"><span data-stu-id="c4673-277">This example shows how to update a table by using its generated ID. Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a><span data-ttu-id="c4673-278">Ändern des Titels</span><span class="sxs-lookup"><span data-stu-id="c4673-278">Change the title</span></span> 

<span data-ttu-id="c4673-279">Dieses Beispiel demonstriert, wie Sie den Titel einer Seite ändern.</span><span class="sxs-lookup"><span data-stu-id="c4673-279">This example shows how to change the title of a page.</span></span> <span data-ttu-id="c4673-280">Verwenden Sie zum Ändern des Titels als Zielwert das Schlüsselwort **title**.</span><span class="sxs-lookup"><span data-stu-id="c4673-280">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="c4673-281">Setzen Sie vor ein Ziel des Typs „title“ niemals das Präfix #.</span><span class="sxs-lookup"><span data-stu-id="c4673-281">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="c4673-282">Aktualisieren eines Aufgabenelements</span><span class="sxs-lookup"><span data-stu-id="c4673-282">Update a to-do item</span></span>

<span data-ttu-id="c4673-283">Im folgenden Beispiel wird die Aktion „replace“ verwendet, um das Kontrollkästchen eines Aufgabenelements auf „Abgeschlossen“ zu setzen.</span><span class="sxs-lookup"><span data-stu-id="c4673-283">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="c4673-284">Weitere Informationen zum Verwenden des Attributs **data-tag** finden Sie im Artikel zum Thema [Verwenden von Notiztags](onenote-note-tags.md).</span><span class="sxs-lookup"><span data-stu-id="c4673-284">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="c4673-285">Beispiele für vollständige PATCH-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="c4673-285">Complete PATCH request examples</span></span>

<span data-ttu-id="c4673-286">Die folgenden Beispiele zeigen vollständige PATCH-Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="c4673-286">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="c4673-287">Anforderung ausschließlich mit Textinhalten</span><span class="sxs-lookup"><span data-stu-id="c4673-287">Request with text content only</span></span>  
<span data-ttu-id="c4673-288">Das folgende Beispiel zeigt eine PATCH-Anforderung, die den Inhaltstyp **application/json** verwendet.</span><span class="sxs-lookup"><span data-stu-id="c4673-288">The following example shows a PATCH request that uses the   **application/json** content type. You can use this format when your content doesn't contain binary data.</span></span> <span data-ttu-id="c4673-289">Dieses Format können Sie verwenden, wenn Ihr Inhalt keine Binärdaten enthält.</span><span class="sxs-lookup"><span data-stu-id="c4673-289">The following example shows a PATCH request that uses the   application/json content type. You can use this format when your content doesn't contain binary data.</span></span>

```
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="c4673-290">Mehrteilige Anforderung mit Binärinhalten</span><span class="sxs-lookup"><span data-stu-id="c4673-290">Multipart request with binary content</span></span> 

<span data-ttu-id="c4673-291">Das folgende Beispiel zeigt eine mehrteilige PATCH-Anforderung, die Binärdaten enthält.</span><span class="sxs-lookup"><span data-stu-id="c4673-291">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="c4673-292">Mehrteilige Anforderungen müssen einen Teil „Commands“ enthalten, in dem der Inhaltstyp **application/json** angegeben ist und der das Array von JSON-Änderungsobjekten enthält.</span><span class="sxs-lookup"><span data-stu-id="c4673-292">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="c4673-293">Andere Datenteile dürfen Binärdaten enthalten.</span><span class="sxs-lookup"><span data-stu-id="c4673-293">Other data parts can contain binary data.</span></span> <span data-ttu-id="c4673-294">Die Namen von Teilen sind in der Regel Zeichenfolgen, an die die aktuelle Zeit in Millisekunden oder eine zufällige GUID angefügt ist.</span><span class="sxs-lookup"><span data-stu-id="c4673-294">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="c4673-295">Anforderungs- and Antwortinformationen in PATCH-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="c4673-295">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="c4673-296">Daten in der Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4673-296">Request data</span></span> | <span data-ttu-id="c4673-297">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4673-297">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c4673-298">Protokoll</span><span class="sxs-lookup"><span data-stu-id="c4673-298">Protocol</span></span> | <span data-ttu-id="c4673-299">Alle Anforderungen verwenden das Protokoll SSL/TLS HTTPS.</span><span class="sxs-lookup"><span data-stu-id="c4673-299">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="c4673-300">Header „Authorization“</span><span class="sxs-lookup"><span data-stu-id="c4673-300">Authorization header</span></span> | <p><span data-ttu-id="c4673-301">`Bearer {token}`, wobei *{token}* ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</span><span class="sxs-lookup"><span data-stu-id="c4673-301">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="c4673-302">Fehlt das Token oder ist es ungültig, schlägt die Anforderung mit dem Statuscode 401 fehl.</span><span class="sxs-lookup"><span data-stu-id="c4673-302">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="c4673-303">Siehe [Authentifizierung und Berechtigungen](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4673-303">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="c4673-304">Header „Content-Type“</span><span class="sxs-lookup"><span data-stu-id="c4673-304">content-type header</span></span> | <p><span data-ttu-id="c4673-305">`application/json` für das Array von JSON-Änderungsobjekten, unabhängig davon, ob es direkt im Anforderungstext gesendet wird oder im Pflichtteil „Commands“ einer [mehrteiligen Anforderung](#multipart-request-with-binary-content).</span><span class="sxs-lookup"><span data-stu-id="c4673-305">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="c4673-306">Mehrteilige Anfragen sind erforderlich, wenn Binärdaten gesendet werden sollen. Sie verwenden den Inhaltstyp `multipart/form-data; boundary=part-boundary`, wobei *{part-boundary}* eine Zeichenfolge ist, die den Beginn und das Ende jedes Datenteils signalisiert.</span><span class="sxs-lookup"><span data-stu-id="c4673-306">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where *{part-boundary}* is a string that signals the start and end of each data part.</span></span></p> |  
 

| <span data-ttu-id="c4673-307">Daten in der Antwort</span><span class="sxs-lookup"><span data-stu-id="c4673-307">Response data</span></span> | <span data-ttu-id="c4673-308">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4673-308">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c4673-309">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="c4673-309">Success code</span></span> | <span data-ttu-id="c4673-p131">204 HTTP-Statuscode. Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4673-p131">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="c4673-312">Fehler</span><span class="sxs-lookup"><span data-stu-id="c4673-312">Errors</span></span> | <span data-ttu-id="c4673-313">Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote_error_codes.md).</span><span class="sxs-lookup"><span data-stu-id="c4673-313">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="c4673-314">Zusammensetzen der Stamm-URL des Microsoft Graph-Diensts</span><span class="sxs-lookup"><span data-stu-id="c4673-314">Constructing the Microsoft Graph service root URL</span></span>

<a name="root-url"></a>

## <a name="root-url"></a><span data-ttu-id="c4673-315">Stamm-URL</span><span class="sxs-lookup"><span data-stu-id="c4673-315">URL Root</span></span>
<span data-ttu-id="c4673-316">Die Stamm-URL des OneNote-Diensts verwendet das folgende Format für alle Aufrufe der OneNote-API:</span><span class="sxs-lookup"><span data-stu-id="c4673-316">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="c4673-317">Das Segment `version` in der URL ist die Version von Microsoft Graph, die verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c4673-317">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>
- <span data-ttu-id="c4673-318">Setzen Sie `v1.0` für stabilen Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="c4673-318">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="c4673-319">Setzen Sie `beta`, wenn Sie ein Feature testen möchten, das sich noch in der Entwicklung befindet.</span><span class="sxs-lookup"><span data-stu-id="c4673-319">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="c4673-320">Features und Funktionen in der Betaphase werden möglicherweise noch geändert und sollten daher nicht in Produktionscode verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c4673-320">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>
- <span data-ttu-id="c4673-321">Setzen Sie `me` für OneNote-Inhalte, auf die der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte).</span><span class="sxs-lookup"><span data-stu-id="c4673-321">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="c4673-322">Setzen Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="c4673-322">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="c4673-323">Verwenden Sie dazu die [Azure AD-Graph-API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="c4673-323">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span></span>


> <span data-ttu-id="c4673-324">**Hinweis:** Benutzer-IDs können Sie über eine GET-Anforderung an `https://graph.microsoft.com/v1.0/users` abrufen.</span><span class="sxs-lookup"><span data-stu-id="c4673-324">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="c4673-325">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c4673-325">Permissions</span></span>

<span data-ttu-id="c4673-326">Zum Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="c4673-326">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="c4673-327">Wählen Sie die niedrigste Berechtigungsstufe, die erforderlich ist, damit Ihre App korrekt funktioniert.</span><span class="sxs-lookup"><span data-stu-id="c4673-327">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="c4673-328">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4673-328">Notes.ReadWrite</span></span>
- <span data-ttu-id="c4673-329">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4673-329">Notes.ReadWrite.All</span></span>

<span data-ttu-id="c4673-330">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie unter [OneNote-Berechtigungsbereiche](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4673-330">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="additional-resources"></a><span data-ttu-id="c4673-331">Weitere Ressourcen</span><span class="sxs-lookup"><span data-stu-id="c4673-331">Additional resources</span></span>

- [<span data-ttu-id="c4673-332">Hinzufügen von Bildern und Dateien</span><span class="sxs-lookup"><span data-stu-id="c4673-332">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="c4673-333">Integrieren mit OneNote</span><span class="sxs-lookup"><span data-stu-id="c4673-333">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="c4673-334">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="c4673-334">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="c4673-335">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="c4673-335">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="c4673-336">GitHub-Repositorys für OneNote</span><span class="sxs-lookup"><span data-stu-id="c4673-336">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

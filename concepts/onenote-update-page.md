---
title: Aktualisieren der Inhalte von OneNote-Seiten
description: " Enterprise-Notizbücher in Office 365"
ms.openlocfilehash: 746520c5071dba0cf11d2fde02daa502522c56f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092227"
---
# <a name="update-onenote-page-content"></a><span data-ttu-id="d8d4a-103">Aktualisieren der Inhalte von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="d8d4a-103">Update OneNote page content</span></span>

<span data-ttu-id="d8d4a-104">**Gilt für** Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365</span><span class="sxs-lookup"><span data-stu-id="d8d4a-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>


<span data-ttu-id="d8d4a-105">Sollen die Inhalte einer OneNote-Seite aktualisiert werden, senden Sie eine PATCH-Anforderung an den Endpunkt *content* der Seite:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-105">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="d8d4a-106">Im Anforderungstext senden Sie ein JSON-Änderungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-106">Send a JSON change object in the message body.</span></span> <span data-ttu-id="d8d4a-107">Wenn die Anforderung erfolgreich ist, gibt Microsoft Graph den HTTP-Statuscode 204 zurück.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-107">If the request is successful, Microsoft Graph returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="d8d4a-108">Zusammensetzen des Anforderungs-URI</span><span class="sxs-lookup"><span data-stu-id="d8d4a-108">Construct the request URI</span></span>

<span data-ttu-id="d8d4a-109">Beginnen Sie bei der Zusammensetzung des Anforderungs-URI mit der Stamm-URL des Diensts:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="d8d4a-110">Fügen Sie dann den Endpunkt *content* der Seite an:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-110">Then append the page's *content* endpoint:</span></span>

- <span data-ttu-id="d8d4a-111">**Abrufen des HTML-Codes der Seite und aller definierten Werte des Typs *data-id***</span><span class="sxs-lookup"><span data-stu-id="d8d4a-111">**Get the page HTML and all defined *data-id* values**</span></span><br/><br/>`../pages/{id}/content`   

- <span data-ttu-id="d8d4a-112">**Abrufen des HTML-Codes der Seite, aller definierten Werte des Typs *data-id* und aller generierten Werte des Typs *id***</span><span class="sxs-lookup"><span data-stu-id="d8d4a-112">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span><br/><br/>`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="d8d4a-113">Die Werte des Typs **data-id** und des Typs **id** dienen als Bezeichner für die Elemente mit dem Attribut **target**, also die Elemente, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-113">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="d8d4a-114">Der vollständige Anforderungs-URI sieht so aus:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-114">Your full request URI will look like this:</span></span><br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="d8d4a-115">Weitere Informationen zur Stamm-URL des Service finden Sie unter [diesem Link](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-115">Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="d8d4a-116">Erstellen des Anforderungstexts</span><span class="sxs-lookup"><span data-stu-id="d8d4a-116">Construct the message body</span></span>

<span data-ttu-id="d8d4a-117">Der HTML-Code einer OneNote-Seite enthält Text, Bilder und andere Inhalte, die in Strukturen wie Elementen des Typs **div**, **img** oder **ol** organisiert sind.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-117">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements.</span></span> <span data-ttu-id="d8d4a-118">Sollen die Inhalte einer OneNote-Seite aktualisiert werden, fügen Sie der Seite HTML-Elemente hinzu oder ersetzen vorhandene HTML-Elemente.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-118">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="d8d4a-119">Ihre Änderungen werden als Array von JSON-Änderungsobjekten im Anforderungstext gesendet.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-119">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="d8d4a-120">Jedes Objekt definiert das Zielelement, neue HTML-Inhalte und die auf die Inhalte anzuwendende Aktion.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-120">Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="d8d4a-p104">Das folgende Array definiert zwei Änderungen. Bei der ersten wird ein Bild über einem Absatz als gleichgeordnetes Element eingefügt, bei der zweiten wird ein Element an eine Liste als letztes untergeordnetes Element angefügt.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

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

<span data-ttu-id="d8d4a-123">Weitere Beispiele finden Sie [hier](#example-requests).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-123">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="d8d4a-124">Attribute für JSON-Änderungsobjekte</span><span class="sxs-lookup"><span data-stu-id="d8d4a-124">Attributes for JSON change objects</span></span>

<span data-ttu-id="d8d4a-125">JSON-Objekte für PATCH-Anforderungen werden mithilfe der Attribute **target**, **action**, **position** und **content** definiert.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-125">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

#### <a name="target"></a><span data-ttu-id="d8d4a-126">target</span><span class="sxs-lookup"><span data-stu-id="d8d4a-126">target</span></span>

<span data-ttu-id="d8d4a-p105">Das zu aktualisierende Element. Der Wert muss einer der folgenden Bezeichner sein:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p105">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="d8d4a-129">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="d8d4a-129">Identifier</span></span> | <span data-ttu-id="d8d4a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8d4a-130">Description</span></span> |  
|------|------|  
| <span data-ttu-id="d8d4a-131">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="d8d4a-131">#{data-id}</span></span> | <p><span data-ttu-id="d8d4a-132">Diese ID wird bei der [Erstellung einer Seite](onenote-create-page.md) oder der [Aktualisierung einer Seite](onenote-update-page.md) optional den Elementen im Eingabe-HTML-Code zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-132">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote-update-page.md).</span></span> <span data-ttu-id="d8d4a-133">Setzen Sie vor den Wert als Präfix das Symbol #.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-133">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="d8d4a-134">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-134">Example:</span></span><br/><span data-ttu-id="d8d4a-135">`'target':'#intro'` legt das Element `<div data-id="intro" ...>` als Ziel fest.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-135">`'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="d8d4a-136">id</span><span class="sxs-lookup"><span data-stu-id="d8d4a-136">id</span></span> | <p><span data-ttu-id="d8d4a-137">Hierbei handelt es sich um die von Microsoft Graph [generierte ID](#generated-ids). Sie ist für die meisten Ersetzungsvorgänge erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-137">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="d8d4a-138">Setzen Sie hier kein Symbol # als Präfix.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-138">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="d8d4a-139">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-139">Example:</span></span><br/><span data-ttu-id="d8d4a-140">`'target':'div:{33f8a2...}{37}'` legt das Element `<div id="div:{33f8a2...}{37}" ...>` als Ziel fest.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-140">`'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="d8d4a-141">Verwechseln Sie IDs dieses Typs nicht mit den Werten des Typs **id** im [Eingabe-HTML-Code](onenote-input-output-html.md).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-141">Don't confuse these with any **id** values defined in the [input HTML](onenote-input-output-html.md).</span></span> <span data-ttu-id="d8d4a-142">Alle im Eingabe-HTML-Code gesendeten Werte des Typs **id** werden verworfen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-142">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="d8d4a-143">body</span><span class="sxs-lookup"><span data-stu-id="d8d4a-143">body</span></span> | <span data-ttu-id="d8d4a-144">Das Schlüsselwort, dass als Ziel das erste „div“-Element auf der Seite festlegt.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-144">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="d8d4a-145">Setzen Sie hier kein Symbol # als Präfix.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-145">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="d8d4a-146">title</span><span class="sxs-lookup"><span data-stu-id="d8d4a-146">title</span></span> | <span data-ttu-id="d8d4a-147">Das Schlüsselwort, das als Ziel den Seitentitel festlegt.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-147">The keyword that targets the page title.</span></span> <span data-ttu-id="d8d4a-148">Setzen Sie hier kein Symbol # als Präfix.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-148">Do not prefix with a #.</span></span> |  
 
#### <a name="action"></a><span data-ttu-id="d8d4a-149">Aktion</span><span class="sxs-lookup"><span data-stu-id="d8d4a-149">action</span></span>

<span data-ttu-id="d8d4a-p111">Die für das Zielelement auszuführende Aktion. Siehe [Unterstützte Aktionen für Elemente](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p111">The action to perform on the target element. See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="d8d4a-152">Aktion</span><span class="sxs-lookup"><span data-stu-id="d8d4a-152">Action</span></span> | <span data-ttu-id="d8d4a-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8d4a-153">Description</span></span> |  
|------|------|  
| <span data-ttu-id="d8d4a-154">append</span><span class="sxs-lookup"><span data-stu-id="d8d4a-154">append</span></span> | <p><span data-ttu-id="d8d4a-155">Fügt den angegebenen Inhalt als erstes oder letztes untergeordnetes Element zum Ziel hinzu, je nach dem im Attribut **position** festgelegten Wert.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-155">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="d8d4a-156">Kann nur auf Elemente des Typs **body**, **div**, **ol** oder **ul** angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-156">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="d8d4a-157">insert</span><span class="sxs-lookup"><span data-stu-id="d8d4a-157">insert</span></span> | <span data-ttu-id="d8d4a-158">Fügt den angegebenen Inhalt als gleichgeordnetes Element vor oder nach dem Ziel hinzu, je nach dem im Attribut **position** festgelegten Wert.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-158">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="d8d4a-159">prepend</span><span class="sxs-lookup"><span data-stu-id="d8d4a-159">prepend</span></span> | <p><span data-ttu-id="d8d4a-160">Fügt den angegebenen Inhalt als erstes untergeordnetes Element zum Ziel hinzu.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-160">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="d8d4a-161">Kurzbefehl als Ersatz für **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-161">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="d8d4a-162">Kann nur auf Elemente des Typs **body**, **div**, **ol** oder **ul** angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-162">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="d8d4a-163">replace</span><span class="sxs-lookup"><span data-stu-id="d8d4a-163">replace</span></span> | <p><span data-ttu-id="d8d4a-164">Ersetzt das Ziel durch den angegebenen Inhalt.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-164">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="d8d4a-165">Für die meisten Aktionen des Typs **replace** muss das Ziel in Form der [generierten ID](#generated-ids) angegeben werden. (Ausnahme: Elemente des Typs **img** oder **object** innerhalb eines „div“-Elements. Sie können auch per **data-id** angegeben werden.)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-165">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
#### <a name="position"></a><span data-ttu-id="d8d4a-166">position</span><span class="sxs-lookup"><span data-stu-id="d8d4a-166">position</span></span>

<span data-ttu-id="d8d4a-p113">Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement. Wenn der Wert weggelassen wird, gilt der Standardwert **after**.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p113">The location to add the supplied content, relative to the target element. Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="d8d4a-169">Position</span><span class="sxs-lookup"><span data-stu-id="d8d4a-169">Position</span></span> | <span data-ttu-id="d8d4a-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8d4a-170">Description</span></span> |  
|------|------|  
| <span data-ttu-id="d8d4a-171">after (Standard)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-171">after (default)</span></span> |<p><span data-ttu-id="d8d4a-172">Mit **append**: das letzte untergeordnete Element des Zielelements</span><span class="sxs-lookup"><span data-stu-id="d8d4a-172">With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="d8d4a-173">Mit **insert**: das nachfolgende gleichgeordnete Element des Zielelements</span><span class="sxs-lookup"><span data-stu-id="d8d4a-173">With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="d8d4a-174">before</span><span class="sxs-lookup"><span data-stu-id="d8d4a-174">before</span></span> | <p><span data-ttu-id="d8d4a-175">Mit **append**: das erste untergeordnete Element des Zielelements</span><span class="sxs-lookup"><span data-stu-id="d8d4a-175">With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="d8d4a-176">Mit **insert**: das vorhergehende gleichgeordnete Element des Zielelements</span><span class="sxs-lookup"><span data-stu-id="d8d4a-176">With **insert**: The preceding sibling of the target element.</span></span></p> |

#### <a name="content"></a><span data-ttu-id="d8d4a-177">content</span><span class="sxs-lookup"><span data-stu-id="d8d4a-177">content</span></span>

<span data-ttu-id="d8d4a-178">Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-178">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="d8d4a-179">Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` in einem Teil „Commands“ gesendet werden (siehe [Beispiel](#multipart-request-with-binary-content)).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-179">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part (see an [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="d8d4a-180">Generierte IDs</span><span class="sxs-lookup"><span data-stu-id="d8d4a-180">Generated IDs</span></span>
<span data-ttu-id="d8d4a-181">Microsoft Graph generiert Werte des Typs **id** für alle Seitenelemente, die aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-181">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="d8d4a-182">Abrufen können Sie die generierten IDs über den Abfragezeichenfolgenausdruck `includeIDs=true` in der GET-Anforderung:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-182">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="d8d4a-183">**Hinweis:** Die API verwirft alle Werte des Typs **id**, die im [Eingabe-HTML-Code](onenote-input-output-html.md) von Anforderungen des Typs „create-page“ oder „update-page“ angegeben sind.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-183">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote-input-output-html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="d8d4a-184">Das folgende Beispiel zeigt generierte IDs für einen Absatz und ein Bild im [Ausgabe-HTML-Code](onenote-input-output-html.md) einer Seite.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-184">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote-input-output-html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="d8d4a-185">Generierte **id**-Werte ändern sich nach dem Aktualisieren einer Seite möglicherweise, Sie sollten daher die aktuellen Werte abrufen, bevor Sie eine PATCH-Anforderung erstellen, die diese verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-185">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="d8d4a-186">Angeben können Sie Zielelemente in Form eines Werts des Typs **data-id** oder eines Werts des Typs **id**. Dabei gilt:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-186">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="d8d4a-187">Bei Aktionen des Typs **append** oder des Typs **insert** können Sie beide ID-Typen als Zielwert verwenden.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-187">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="d8d4a-188">Bei Aktionen des Typs **replace** müssen Sie für alle Elemente die generierte ID verwenden. Ausgenommen hiervon sind lediglich der Seitentitel sowie Bilder und Objekte innerhalb von „div“-Elementen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-188">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
    - <span data-ttu-id="d8d4a-189">Ersetzen eines Titels: Verwenden Sie das Schlüsselwort **title**.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-189">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="d8d4a-190">Ersetzen von Bildern und Objekten in einem „div“-Element: Verwenden Sie entweder **data-id** oder **id**.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-190">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="d8d4a-191">Im folgenden Beispiel wird das Ziel in Form eines Werts des Typs **id** angegeben.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-191">The following example uses the **id** value for the target.</span></span> <span data-ttu-id="d8d4a-192">Setzen Sie vor generierten IDs niemals das Präfix #.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-192">Don't use the # prefix with a generated ID.</span></span>

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

## <a name="supported-elements-and-actions"></a><span data-ttu-id="d8d4a-193">Unterstützte Elemente und Aktionen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-193">Supported elements and actions</span></span>

<span data-ttu-id="d8d4a-194">Viele Elemente auf einer Seite lassen sich aktualisieren, doch unterstützt jeder Elementtyp nur bestimmte Aktionen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-194">Many elements on the page can be updated, but each element type supports specific actions.</span></span> <span data-ttu-id="d8d4a-195">In der folgenden Tabelle sind die unterstützten Zielelemente aufgeführt sowie die Aktualisierungsaktionen, die sie unterstützen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-195">The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="d8d4a-196">Element</span><span class="sxs-lookup"><span data-stu-id="d8d4a-196">Element</span></span> | <span data-ttu-id="d8d4a-197">Ersetzen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-197">Replace</span></span> | <span data-ttu-id="d8d4a-198">Untergeordnetes Element anfügen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-198">Append child</span></span> | <span data-ttu-id="d8d4a-199">Gleichgeordnetes Element einfügen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-199">Insert sibling</span></span> |  
|------|:------:|:------:|:------:|  
| <span data-ttu-id="d8d4a-200">body</span><span class="sxs-lookup"><span data-stu-id="d8d4a-200">body</span></span><br /> <span data-ttu-id="d8d4a-201">(Ziel: erstes „div“-Element auf der Seite)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-201">(targets first div on the page)</span></span> | <span data-ttu-id="d8d4a-202">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-202">no</span></span> | <span data-ttu-id="d8d4a-203">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-203">**yes**</span></span> | <span data-ttu-id="d8d4a-204">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-204">no</span></span> |  
| <span data-ttu-id="d8d4a-205">div</span><span class="sxs-lookup"><span data-stu-id="d8d4a-205">div</span></span><br /> <span data-ttu-id="d8d4a-206">([absolut positioniert](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="d8d4a-206">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="d8d4a-207">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-207">no</span></span> | <span data-ttu-id="d8d4a-208">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-208">**yes**</span></span> | <span data-ttu-id="d8d4a-209">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-209">no</span></span> |  
| <span data-ttu-id="d8d4a-210">div</span><span class="sxs-lookup"><span data-stu-id="d8d4a-210">div</span></span><br /> <span data-ttu-id="d8d4a-211">(in einem anderen „div“-Element)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-211">(within a div)</span></span> | <span data-ttu-id="d8d4a-212">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-212">**yes**</span></span><br/><span data-ttu-id="d8d4a-213">(nur per „id“)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-213">(id only)</span></span> | <span data-ttu-id="d8d4a-214">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-214">**yes**</span></span> | <span data-ttu-id="d8d4a-215">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-215">**yes**</span></span> |   
| <span data-ttu-id="d8d4a-216">img, object</span><span class="sxs-lookup"><span data-stu-id="d8d4a-216">img, object</span></span><br /> <span data-ttu-id="d8d4a-217">(in einem anderen „div“-Element)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-217">(within a div)</span></span> | <span data-ttu-id="d8d4a-218">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-218">**yes**</span></span> | <span data-ttu-id="d8d4a-219">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-219">no</span></span> | <span data-ttu-id="d8d4a-220">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-220">**yes**</span></span> |   
| <span data-ttu-id="d8d4a-221">ol, ul</span><span class="sxs-lookup"><span data-stu-id="d8d4a-221">ol, ul</span></span> | <span data-ttu-id="d8d4a-222">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-222">**yes**</span></span><br/><span data-ttu-id="d8d4a-223">(nur per „id“)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-223">(id only)</span></span> | <span data-ttu-id="d8d4a-224">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-224">**yes**</span></span> | <span data-ttu-id="d8d4a-225">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-225">**yes**</span></span> |   
| <span data-ttu-id="d8d4a-226">table</span><span class="sxs-lookup"><span data-stu-id="d8d4a-226">table</span></span> | <span data-ttu-id="d8d4a-227">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-227">**yes**</span></span><br/><span data-ttu-id="d8d4a-228">(nur per „id“)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-228">(id only)</span></span> | <span data-ttu-id="d8d4a-229">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-229">no</span></span> | <span data-ttu-id="d8d4a-230">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-230">**yes**</span></span> |   
| <span data-ttu-id="d8d4a-231">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="d8d4a-231">p, li, h1-h6</span></span> | <span data-ttu-id="d8d4a-232">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-232">**yes**</span></span><br/><span data-ttu-id="d8d4a-233">(nur per „id“)</span><span class="sxs-lookup"><span data-stu-id="d8d4a-233">(id only)</span></span> | <span data-ttu-id="d8d4a-234">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-234">no</span></span> | <span data-ttu-id="d8d4a-235">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-235">**yes**</span></span> |   
| <span data-ttu-id="d8d4a-236">title</span><span class="sxs-lookup"><span data-stu-id="d8d4a-236">title</span></span> | <span data-ttu-id="d8d4a-237">**Ja**</span><span class="sxs-lookup"><span data-stu-id="d8d4a-237">**yes**</span></span> | <span data-ttu-id="d8d4a-238">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-238">no</span></span> | <span data-ttu-id="d8d4a-239">Nein</span><span class="sxs-lookup"><span data-stu-id="d8d4a-239">no</span></span> |  
 
<br/>

<span data-ttu-id="d8d4a-240">Die folgenden Elemente unterstützen keinerlei Aktualisierungsaktionen:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-240">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="d8d4a-241">img ([absolut positioniert](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="d8d4a-241">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="d8d4a-242">object ([absolut positioniert](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="d8d4a-242">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="d8d4a-243">tr, td</span><span class="sxs-lookup"><span data-stu-id="d8d4a-243">tr, td</span></span>
- <span data-ttu-id="d8d4a-244">meta</span><span class="sxs-lookup"><span data-stu-id="d8d4a-244">meta</span></span>
- <span data-ttu-id="d8d4a-245">head</span><span class="sxs-lookup"><span data-stu-id="d8d4a-245">head</span></span>
- <span data-ttu-id="d8d4a-246">span</span><span class="sxs-lookup"><span data-stu-id="d8d4a-246">span</span></span>
- <span data-ttu-id="d8d4a-247">a</span><span class="sxs-lookup"><span data-stu-id="d8d4a-247">a</span></span>
- <span data-ttu-id="d8d4a-248">„style“-Tags</span><span class="sxs-lookup"><span data-stu-id="d8d4a-248">style tags</span></span>


<a name="examples"></a>

## <a name="example-requests"></a><span data-ttu-id="d8d4a-249">Beispielanforderungen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-249">Example requests</span></span>

<span data-ttu-id="d8d4a-250">Eine Aktualisierungsanforderung enthält eine oder mehrere Änderungen, jeweils dargestellt als JSON-Änderungsobjekt.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-250">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="d8d4a-251">Diese Objekte können unterschiedliche Ziele auf der Seite sowie unterschiedliche Aktionen und Inhalte für diese Ziele definieren.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-251">These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="d8d4a-252">Die folgenden Beispiele zeigen JSON-Objekte, die in PATCH-Anforderungen verwendet werden, sowie vollständige PATCH-Anforderungen:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-252">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

- [<span data-ttu-id="d8d4a-253">Anfügen von untergeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-253">Append child elements</span></span>](#append-child-elements)
- [<span data-ttu-id="d8d4a-254">Einfügen von gleichgeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-254">Insert sibling elements</span></span>](#insert-sibling-elements)
- [<span data-ttu-id="d8d4a-255">Ersetzen von Elementen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-255">Replace elements</span></span>](#replace-elements)
- [<span data-ttu-id="d8d4a-256">Vollständige PATCH-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-256">Complete PATCH requests</span></span>](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="d8d4a-257">Anfügen von untergeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-257">Append child elements</span></span>

<span data-ttu-id="d8d4a-p119">Die **append**-Aktion fügt ein untergeordnetes Element zu einem **body**-, **div**- (innerhalb eines div-Elements), **ol**- oder **ul**-Element hinzu. Das **position**-Attribut bestimmt, ob das untergeordnete Element vor oder nach dem Tag angefügt wird. Die Standardposition ist **after**.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p119">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element. The **position** attribute determines whether to append the child before or after the target. The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="d8d4a-261">Anfügen an ein „div“-Element</span><span class="sxs-lookup"><span data-stu-id="d8d4a-261">Append to a div</span></span>

<span data-ttu-id="d8d4a-262">Das folgende Beispiel fügt dem Element **div1** zwei untergeordnete Knoten hinzu.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-262">The following example adds two child nodes to the **div1** element.</span></span> <span data-ttu-id="d8d4a-263">Als erstes untergeordnetes Element wird ein Bild hinzugefügt, als letztes untergeordnetes Element ein Absatz.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-263">It adds an image as the first child and a paragraph as the last child.</span></span> 

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
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="d8d4a-264">Anfügen an das *body*-Element</span><span class="sxs-lookup"><span data-stu-id="d8d4a-264">Append to the *body* element</span></span>

<span data-ttu-id="d8d4a-265">Sie können **body** als schnellen Weg verwenden, um ein untergeordnetes Element im ersten „div“-Element auf der Seite anzufügen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-265">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="d8d4a-266">Im folgenden Beispiel werden dem ersten „div“-Element auf der Seite zwei Absätze hinzugefügt, einer als erstes untergeordnetes Element und einer als letztes untergeordnetes Element.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-266">The following example adds two paragraphs as the first child and the last child to the first div on the page.</span></span> <span data-ttu-id="d8d4a-267">Setzen Sie vor ein Ziel des Typs **body** niemals das Präfix #.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-267">Don't use a # with the **body** target.</span></span> <span data-ttu-id="d8d4a-268">In diesem Beispiel verwenden wir die Aktion **prepend** als Kurzversion von **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-268">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

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
 

#### <a name="append-to-a-list"></a><span data-ttu-id="d8d4a-269">Anfügen an eine Liste</span><span class="sxs-lookup"><span data-stu-id="d8d4a-269">Append to a list</span></span>

<span data-ttu-id="d8d4a-p122">Im folgenden Beispiel wird ein Listenelement als letztes untergeordnetes Element zur Zielliste hinzugefügt. Die **list-style-type**-Eigenschaft ist definiert, da das Element einen nicht standardmäßigen Listenstil verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p122">The following example adds a list item as a last child to the target list. The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

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

### <a name="insert-sibling-elements"></a><span data-ttu-id="d8d4a-272">Einfügen von gleichgeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-272">Insert sibling elements</span></span>

<span data-ttu-id="d8d4a-273">Die Aktion **insert** fügt dem Zielelement ein gleichgeordnetes Element hinzu.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-273">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="d8d4a-274">Das Attribut **position** legt fest, ob das gleichgeordnete Element vor oder nach dem Ziel eingefügt wird.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-274">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="d8d4a-275">Die Standardposition ist **after**.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-275">The default position is **after**.</span></span> <span data-ttu-id="d8d4a-276">In diesem Abschnitt finden Sie alle [Elemente, die **insert** unterstützen](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-276">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

#### <a name="insert-siblings"></a><span data-ttu-id="d8d4a-277">Einfügen von gleichgeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-277">Insert siblings</span></span>

<span data-ttu-id="d8d4a-p124">Im folgenden Beispiel werden zwei gleichgeordnete Knoten zu der Seite hinzugefügt. Über dem **para1**-Element wird ein Bild und über dem **para2**-Element wird ein Absatz hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p124">The following example adds two sibling nodes to the page. It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

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

### <a name="replace-elements"></a><span data-ttu-id="d8d4a-280">Ersetzen von Elementen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-280">Replace elements</span></span>

<span data-ttu-id="d8d4a-281">Sie können entweder den Wert **data-id** oder den generierten Wert **id** als Zielwert nutzen, wenn Sie Elemente des Typs **img** oder **object** in einem „div“-Element ersetzen möchten.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-281">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div.</span></span> <span data-ttu-id="d8d4a-282">Verwenden Sie das Schlüsselwort **title**, wenn der Seitentitel ersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-282">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="d8d4a-283">Bei allen anderen [Elementen, die **replace** unterstützen](#supported-elements-and-actions), müssen Sie die generierte ID verwenden.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-283">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="d8d4a-284">Ersetzen eines Bilds</span><span class="sxs-lookup"><span data-stu-id="d8d4a-284">Replace an image</span></span>

<span data-ttu-id="d8d4a-285">Im folgenden Beispiel wird ein Bild durch ein „div“-Element ersetzt. Als Zielwert wird der Wert **data-id** des Bilds verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-285">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="d8d4a-286">Aktualisieren einer Tabelle</span><span class="sxs-lookup"><span data-stu-id="d8d4a-286">Update a table</span></span> 

<span data-ttu-id="d8d4a-p126">In diesem Beispiel wird gezeigt, wie eine Tabelle mithilfe ihrer generierten ID aktualisiert wird. Das Ersetzen von **tr**- und **td**-Elementen wird nicht unterstützt, Sie können jedoch die gesamte Tabelle ersetzen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p126">This example shows how to update a table by using its generated ID. Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

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
 

#### <a name="change-the-title"></a><span data-ttu-id="d8d4a-289">Ändern des Titels</span><span class="sxs-lookup"><span data-stu-id="d8d4a-289">Change the title</span></span> 

<span data-ttu-id="d8d4a-290">Dieses Beispiel demonstriert, wie Sie den Titel einer Seite ändern.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-290">This example shows how to change the title of a page.</span></span> <span data-ttu-id="d8d4a-291">Verwenden Sie zum Ändern des Titels als Zielwert das Schlüsselwort **title**.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-291">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="d8d4a-292">Setzen Sie vor ein Ziel des Typs „title“ niemals das Präfix #.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-292">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="d8d4a-293">Aktualisieren eines Aufgabenelements</span><span class="sxs-lookup"><span data-stu-id="d8d4a-293">Update a to-do item</span></span>

<span data-ttu-id="d8d4a-294">Im folgenden Beispiel wird die Aktion „replace“ verwendet, um das Kontrollkästchen eines Aufgabenelements auf „Abgeschlossen“ zu setzen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-294">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="d8d4a-295">Weitere Informationen zum Verwenden des Attributs **data-tag** finden Sie im Artikel zum Thema [Verwenden von Notiztags](onenote-note-tags.md).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-295">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="d8d4a-296">Beispiele für vollständige PATCH-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-296">Complete PATCH request examples</span></span>

<span data-ttu-id="d8d4a-297">Die folgenden Beispiele zeigen vollständige PATCH-Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-297">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="d8d4a-298">Anforderung ausschließlich mit Textinhalten</span><span class="sxs-lookup"><span data-stu-id="d8d4a-298">Request with text content only</span></span>

<span data-ttu-id="d8d4a-299">Das folgende Beispiel zeigt eine PATCH-Anforderung, die den Inhaltstyp **application/json** verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-299">The following example shows a PATCH request that uses the **application/json** content type.</span></span> <span data-ttu-id="d8d4a-300">Dieses Format können Sie verwenden, wenn Ihr Inhalt keine Binärdaten enthält.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-300">You can use this format when your content doesn't contain binary data.</span></span>

```json
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

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="d8d4a-301">Mehrteilige Anforderung mit Binärinhalten</span><span class="sxs-lookup"><span data-stu-id="d8d4a-301">Multipart request with binary content</span></span> 

<span data-ttu-id="d8d4a-302">Das folgende Beispiel zeigt eine mehrteilige PATCH-Anforderung, die Binärdaten enthält.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-302">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="d8d4a-303">Mehrteilige Anforderungen müssen einen Teil „Commands“ enthalten, in dem der Inhaltstyp **application/json** angegeben ist und der das Array von JSON-Änderungsobjekten enthält.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-303">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="d8d4a-304">Andere Datenteile dürfen Binärdaten enthalten.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-304">Other data parts can contain binary data.</span></span> <span data-ttu-id="d8d4a-305">Die Namen von Teilen sind in der Regel Zeichenfolgen, an die die aktuelle Zeit in Millisekunden oder eine zufällige GUID angefügt ist.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-305">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```json
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

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="d8d4a-306">Anforderungs- and Antwortinformationen in PATCH-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-306">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="d8d4a-307">Daten in der Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8d4a-307">Request data</span></span> | <span data-ttu-id="d8d4a-308">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8d4a-308">Description</span></span> |  
|------|------|  
| <span data-ttu-id="d8d4a-309">Protokoll</span><span class="sxs-lookup"><span data-stu-id="d8d4a-309">Protocol</span></span> | <span data-ttu-id="d8d4a-310">Alle Anforderungen verwenden das SSL/TLS HTTPS-Protokoll.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-310">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="d8d4a-311">Header „Authorization“</span><span class="sxs-lookup"><span data-stu-id="d8d4a-311">Authorization header</span></span> | <p><span data-ttu-id="d8d4a-312">`Bearer {token}`, wobei `{token}` ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-312">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="d8d4a-313">Wenn dies fehlt oder ungültig ist, schlägt die Anforderung mit dem Statuscode 401 fehl.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-313">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="d8d4a-314">Siehe [Authentifizierung und Berechtigungen](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-314">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="d8d4a-315">Header „Content-Type“</span><span class="sxs-lookup"><span data-stu-id="d8d4a-315">Content-Type header</span></span> | <p><span data-ttu-id="d8d4a-316">`application/json` für das Array von JSON-Änderungsobjekten, unabhängig davon, ob es direkt im Anforderungstext gesendet wird oder im Pflichtteil „Commands“ einer [mehrteiligen Anforderung](#multipart-request-with-binary-content).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-316">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="d8d4a-317">Mehrteilige Anfragen sind erforderlich, wenn Binärdaten gesendet werden sollen. Sie verwenden den Inhaltstyp `multipart/form-data; boundary=part-boundary`, wobei `{part-boundary}` eine Zeichenfolge ist, die den Beginn und das Ende jedes Datenteils signalisiert.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-317">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  

<br/> 

| <span data-ttu-id="d8d4a-318">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="d8d4a-318">Response data</span></span> | <span data-ttu-id="d8d4a-319">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8d4a-319">Description</span></span> |  
|------|------|  
| <span data-ttu-id="d8d4a-320">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="d8d4a-320">Success code</span></span> | <span data-ttu-id="d8d4a-p131">204 HTTP-Statuscode. Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-p131">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="d8d4a-323">Fehler</span><span class="sxs-lookup"><span data-stu-id="d8d4a-323">Errors</span></span> | <span data-ttu-id="d8d4a-324">Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-324">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="d8d4a-325">Zusammensetzen der Stamm-URL des Microsoft Graph-Diensts</span><span class="sxs-lookup"><span data-stu-id="d8d4a-325">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="d8d4a-326">Die Stamm-URL des OneNote-Diensts verwendet das folgende Format für alle Aufrufe der OneNote-API:</span><span class="sxs-lookup"><span data-stu-id="d8d4a-326">The OneNote service root URL uses the following format for all calls to the OneNote API:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="d8d4a-327">Das Segment `version` in der URL ist die Version von Microsoft Graph, die verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-327">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="d8d4a-328">Setzen Sie `v1.0` für stabilen Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-328">`v1.0` is for stable production code.</span></span> <span data-ttu-id="d8d4a-329">Setzen Sie `beta`, wenn Sie ein Feature testen möchten, das sich noch in der Entwicklung befindet.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-329">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="d8d4a-330">Features und Funktionen in der Betaphase werden möglicherweise noch geändert und sollten daher nicht in Produktionscode verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-330">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>

<span data-ttu-id="d8d4a-331">Setzen Sie `me` für OneNote-Inhalte, auf die der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-331">`me` is for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="d8d4a-332">Setzen Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-332">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="d8d4a-333">Verwenden Sie dazu die [Azure AD-Graph-API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-333">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog).</span></span>


> <span data-ttu-id="d8d4a-334">**Hinweis:** Benutzer-IDs können Sie über eine GET-Anforderung an `https://graph.microsoft.com/v1.0/users` abrufen.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-334">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="d8d4a-335">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d8d4a-335">Permissions</span></span>

<span data-ttu-id="d8d4a-336">Zum Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-336">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="d8d4a-337">Wählen Sie die niedrigste Berechtigungsstufe, die erforderlich ist, damit Ihre App korrekt funktioniert.</span><span class="sxs-lookup"><span data-stu-id="d8d4a-337">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="d8d4a-338">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8d4a-338">Notes.ReadWrite</span></span>
- <span data-ttu-id="d8d4a-339">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8d4a-339">Notes.ReadWrite.All</span></span>

<span data-ttu-id="d8d4a-340">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie unter [OneNote-Berechtigungsbereiche](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8d4a-340">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="d8d4a-341">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d8d4a-341">See also</span></span>

- [<span data-ttu-id="d8d4a-342">Hinzufügen von Bildern und Dateien</span><span class="sxs-lookup"><span data-stu-id="d8d4a-342">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="d8d4a-343">Integrieren mit OneNote</span><span class="sxs-lookup"><span data-stu-id="d8d4a-343">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="d8d4a-344">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="d8d4a-344">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="d8d4a-345">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="d8d4a-345">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="d8d4a-346">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="d8d4a-346">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="e23f7-101">Eingabe- und Ausgabe-HTML auf OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="e23f7-101">Input and output HTML for OneNote pages</span></span>

<span data-ttu-id="e23f7-102">Der HTML-Code, der den Seiteninhalt und die Seitenstruktur definiert, wenn Sie eine OneNote-Seite [erstellen](../api-reference/v1.0/api/section_post_pages.md) oder [aktualisieren](../api-reference/v1.0/api/page_update.md), wird *Eingabe-HTML* genannt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-102">The HTML that defines the page content and structure when you [create](../api-reference/v1.0/api/section_post_pages.md) or [update](../api-reference/v1.0/api/page_update.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="e23f7-103">Der HTML-Code, der beim [Abrufen von Seiteninhalt](../api-reference/v1.0/api/page_get.md) zurückgegeben wird, heißt *Ausgabe-HTML*.</span><span class="sxs-lookup"><span data-stu-id="e23f7-103">The HTML that's returned when you [get page content](../api-reference/v1.0/api/page_get.md) is called *output HTML*.</span></span> <span data-ttu-id="e23f7-104">Der Ausgabe-HTML-Code entspricht nicht dem Eingabe-HTML-Code.</span><span class="sxs-lookup"><span data-stu-id="e23f7-104">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="e23f7-105">Die OneNote-APIs in Microsoft Graph behalten den semantischen Inhalt und die grundlegende Struktur des Eingabe-HTML-Codes bei, konvertieren diese jedoch in [unterstützte HTML-Elemente und CSS-Eigenschaften](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html).</span><span class="sxs-lookup"><span data-stu-id="e23f7-105">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html).</span></span> <span data-ttu-id="e23f7-106">Die APIs fügen zudem benutzerdefinierte Attribute hinzu, die OneNote-Funktionen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-106">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="e23f7-107">Dieser Artikel beschreibt die wichtigsten Elemente und Attribute von Eingabe- und Ausgabe-HTML-Codes.</span><span class="sxs-lookup"><span data-stu-id="e23f7-107">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="e23f7-108">Es kann hilfreich sein, Eingabe-HTML-Codes zu verstehen, wenn Sie Seiteninhalte erstellen oder aktualisieren. Mit Ausgabe- HTML-Codes sollten Sie sich auskennen, wenn Sie zurückgegebene Seiteninhalte analysieren möchten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-108">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="e23f7-109">Textkörperelement</span><span class="sxs-lookup"><span data-stu-id="e23f7-109">Body element</span></span>
<span data-ttu-id="e23f7-110">Der HTML-Inhalt im Textkörper der Seite repräsentiert den Seiteninhalt und die Seitenstruktur, einschließlich der Bild- und Dateiressourcen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-110">The HTML content in the page body represents  the page content and structure, including image and file resources. The body element can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="e23f7-111">Das **body**-Element kann die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-111">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="e23f7-112">**Eingabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-112">**Input attributes**</span></span>

|<span data-ttu-id="e23f7-113">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-113">Input attribute</span></span>|<span data-ttu-id="e23f7-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-114">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-115">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="e23f7-115">data-absolute-enabled</span></span> | <span data-ttu-id="e23f7-116">Gibt an, ob der Eingabe-Textkörper [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)-Elemente unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-116">Indicates whether the input body supports [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) elements.</span></span> |
| <span data-ttu-id="e23f7-117">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-117">style</span></span> | <p><span data-ttu-id="e23f7-118">Die CSS-[style](#styles)-Eigenschaften des Textkörpers.</span><span class="sxs-lookup"><span data-stu-id="e23f7-118">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="e23f7-119">In der Ausgabe-HTML können Eingabeeinstellungen eingebettet in die entsprechenden untergeordneten Elemente zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e23f7-119">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="e23f7-120">Hintergrundfarbe wird derzeit nicht für das **body**-Element unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-120">Background color is not currently supported for the **body** element.</span></span></p> |
 

<span data-ttu-id="e23f7-121">**Ausgabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-121">**Output attributes**</span></span>

|<span data-ttu-id="e23f7-122">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-122">Output attribute</span></span>|<span data-ttu-id="e23f7-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-123">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-124">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="e23f7-124">data-absolute-enabled</span></span> | <span data-ttu-id="e23f7-125">Gibt an, ob der Textkörper [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)-Elemente unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-125">Indicates whether the body supports absolutely positioned elements. Always true in output HTML.</span></span> <span data-ttu-id="e23f7-126">Immer **true** in der HTML-Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="e23f7-126">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="e23f7-127">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-127">style</span></span> | <span data-ttu-id="e23f7-128">Die Eigenschaften **font-family** und **font-size** des Textkörpers.</span><span class="sxs-lookup"><span data-stu-id="e23f7-128">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="e23f7-129">Div-Elemente</span><span class="sxs-lookup"><span data-stu-id="e23f7-129">Div elements</span></span>
<span data-ttu-id="e23f7-130">**Div**-Elemente enthalten Text, Bilder und andere Inhalte.</span><span class="sxs-lookup"><span data-stu-id="e23f7-130">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="e23f7-131">Das **div**-Element kann die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-131">Divs contain text, images, and other content. A **div** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="e23f7-132">**Eingabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-132">**Input attributes**</span></span>

|<span data-ttu-id="e23f7-133">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-133">Input attribute</span></span>|<span data-ttu-id="e23f7-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-134">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-135">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-135">data-id</span></span> | <span data-ttu-id="e23f7-136">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-136">A reference for the element.</span></span> <span data-ttu-id="e23f7-137">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-137">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-138">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="e23f7-138">data-render-fallback</span></span> | <span data-ttu-id="e23f7-139">Die Ausweichaktion bei einem Fehler der [Extraktion](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data): **render** (Standard) oder **none**.</span><span class="sxs-lookup"><span data-stu-id="e23f7-139">The fallback action if the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="e23f7-140">data-render-method</span><span class="sxs-lookup"><span data-stu-id="e23f7-140">data-render-method</span></span> | <span data-ttu-id="e23f7-141">Die auszuführende [Extraktionsmethode](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data), z. B.: `extract.businesscard` oder `extract.recipe`.</span><span class="sxs-lookup"><span data-stu-id="e23f7-141">The [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) method to perform, for example: `extract.businesscard`extract.businesscard`extract.recipe`

or extract.recipe.</span></span> |
| <span data-ttu-id="e23f7-142">data-render-src</span><span class="sxs-lookup"><span data-stu-id="e23f7-142">data-render-src</span></span> | <span data-ttu-id="e23f7-143">Die Inhaltsquelle für die [Extraktion](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span><span class="sxs-lookup"><span data-stu-id="e23f7-143">The content source for the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span></span> |
| <span data-ttu-id="e23f7-144">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-144">style</span></span> | <p><span data-ttu-id="e23f7-145">Die Position, Größe, Schriftart und Farbe von Eigenschaften für div:</span><span class="sxs-lookup"><span data-stu-id="e23f7-145">The position, size, font, and color properties for the div:</span></span></p><p> <span data-ttu-id="e23f7-146">- **Position** (nur **absolut**), **links**, **oben** und **Breite**.</span><span class="sxs-lookup"><span data-stu-id="e23f7-146">- **position** (**absolute** only), **left**, **top**, and **width**.</span></span> <span data-ttu-id="e23f7-147">(Die Höhe wird für divs automatisch konfiguriert .)</span><span class="sxs-lookup"><span data-stu-id="e23f7-147">(Height is auto-configured for divs.)</span></span><br /><span data-ttu-id="e23f7-148">Wird verwendet, um ein [absolut positioniertes](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)-Div-Element zu erstellen, wenn das Div-Element ein direktes untergeordnetes Element des Textkörpers und für den Textkörper `data-absolute-enabled="true"` angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="e23f7-148">Used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="e23f7-149">Beispiel: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="e23f7-149">Example`<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></p><p> <span data-ttu-id="e23f7-150">Die CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="e23f7-150">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="e23f7-151">In der Ausgabe-HTML werden diese Werte eingebettet in die entsprechenden untergeordneten Elemente zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e23f7-151">The CSS style properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></p> |
 

<span data-ttu-id="e23f7-152">Die OneNote-APIs in Microsoft Graph umschließen alle Textkörper mit mindestens einem Div.</span><span class="sxs-lookup"><span data-stu-id="e23f7-152">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="e23f7-153">Die API erstellt ein standardmäßiges Div (mit `data-id="_default"`-Attributen), die den Textkörper enthalten, wenn:</span><span class="sxs-lookup"><span data-stu-id="e23f7-153">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="e23f7-154">Das **data-absolute-enabled**-Attribut des Eingabe-Textkörper-Elements ausgelassen oder auf **false** gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="e23f7-154">The input body element's data-absolute-enabled attribute is omitted or set to false. In this case, all body content is put in the default div.</span></span> <span data-ttu-id="e23f7-155">In diesem Fall werden alle Inhalte des Textkörpers im standardmäßigen Div abgelegt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-155">The input body element's data-absolute-enabled attribute is omitted or set to false. In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="e23f7-156">Das **data-absolute-enabled**-Attribut des Eingabe-Textkörper-Elements auf **true** gesetzt wird, die Eingabe HTML jedoch direkt untergeordnete Elemente enthält, die [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img** oder **object**-Elemente sind.</span><span class="sxs-lookup"><span data-stu-id="e23f7-156">The input body element's data-absolute-enabled attribute is true, but the input HTML  contains direct children that aren't absolutely positioned div, img, or object elements. In this case, direct children that aren't absolutely positioned div, img, or object elements are put in the default div.</span></span> <span data-ttu-id="e23f7-157">In diesem Fall werden untergeordnete Elemente, die keine [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img** oder **object**-Elemente sind, im standardmäßigen Div abgelegt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-157">In this case, direct children that aren't [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


<span data-ttu-id="e23f7-158">**Ausgabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-158">**Output attributes**</span></span>

|<span data-ttu-id="e23f7-159">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-159">Output attribute</span></span>|<span data-ttu-id="e23f7-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-160">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-161">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-161">data-id</span></span> | <span data-ttu-id="e23f7-162">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-162">A reference for the element.</span></span> <span data-ttu-id="e23f7-163">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-163">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-164">id</span><span class="sxs-lookup"><span data-stu-id="e23f7-164">id</span></span> | <span data-ttu-id="e23f7-165">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-165">A unique ID for the group.</span></span> <span data-ttu-id="e23f7-166">Zurückgegeben von einem [GET requests to a page's*-content*-Endpunkt ](../api-reference/v1.0/api/page_get.md), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e23f7-166">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="e23f7-167">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-167">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-168">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-168">style</span></span> | <span data-ttu-id="e23f7-169">Die Positions- und Größeneigenschaften des div-Elements.</span><span class="sxs-lookup"><span data-stu-id="e23f7-169">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="e23f7-170">Nicht beitragende Divs</span><span class="sxs-lookup"><span data-stu-id="e23f7-170">Non-contributing divs</span></span>
<span data-ttu-id="e23f7-171">Wenn ein **div**-Element in der Eingabe-HTML nichts zur Seitenstruktur beiträgt und keine von OneNote verwendeten Informationen enthält,  verschiebt die API den Inhalt des div-Elements in das übergeordnete oder standardmäßige div-Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-171">When a div element in the input HTML does not contribute to the page structure or carry information that onnvshort uses,  the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="e23f7-172">Dieser Vorgang wird in den folgenden Beispielen dargestellt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-172">This is illustrated in the following examples.</span></span>

<span data-ttu-id="e23f7-173">**Eingabe-HTML** mit einem nicht beitragenden, geschachtelten div-Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-173">**Input HTML**  that contains a non-contributing, nested div.</span></span>

```html
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <div>
            <p>Some text</p>
            <div>
                <p>More text inside a div that doesn't define page structure</p>
            </div>
        </div>
    </body>
</html>
```

<span data-ttu-id="e23f7-174">**Ausgabe-HTML-Code**</span><span class="sxs-lookup"><span data-stu-id="e23f7-174">**Output HTML**</span></span>

><span data-ttu-id="e23f7-175">**Hinweis:** Der DIV-Inhalt wurde in die übergeordnete Div verschoben, und die geschachtelten `<div>`-Tags wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-175">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="e23f7-176">Die Div wäre erhalten geblieben, wenn sie semantische Informationen definiert hätte, z. B. eine **Daten-Id** (Beispiel: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="e23f7-176">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11px">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <p>Some text</p>
            <p>More text inside a nested div</p>
        </div>
    </body>
</html>
```


## <a name="img-elements"></a><span data-ttu-id="e23f7-177">Img-Elemente</span><span class="sxs-lookup"><span data-stu-id="e23f7-177">Img elements</span></span>
<span data-ttu-id="e23f7-178">Bilder auf OneNote-Seiten werden durch **img**-Elemente dargestellt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-178">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="e23f7-179">Das **img**-Element kann die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-179">Images on onnvshort pages are represented by **img** elements. An img element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="e23f7-180">**Eingabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-180">**Input attributes**</span></span>

|<span data-ttu-id="e23f7-181">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-181">Input attribute</span></span>|<span data-ttu-id="e23f7-182">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-182">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-183">alt</span><span class="sxs-lookup"><span data-stu-id="e23f7-183">alt</span></span> | <span data-ttu-id="e23f7-184">Der angegebene Alternativtext für das Bild.</span><span class="sxs-lookup"><span data-stu-id="e23f7-184">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="e23f7-185">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-185">data-id</span></span> | <span data-ttu-id="e23f7-186">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-186">A reference for the element.</span></span> <span data-ttu-id="e23f7-187">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-187">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-188">data-render-src</span><span class="sxs-lookup"><span data-stu-id="e23f7-188">data-render-src</span></span> |<span data-ttu-id="e23f7-189">Es ist entweder **data-render-src** oder **src** erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e23f7-189">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="e23f7-190">Die Webseite, die als Bitmapbild auf der OneNote-Seite gerendert werden soll:</span><span class="sxs-lookup"><span data-stu-id="e23f7-190">The webpage to render as a bit-mapped image on the onnvshort page:</span></span><br /> <span data-ttu-id="e23f7-191">- `data-render-src="http://..."` für eine öffentliche URL.</span><span class="sxs-lookup"><span data-stu-id="e23f7-191">- `data-render-src="http://..."` for a public URL.</span></span><br /> <span data-ttu-id="e23f7-192">- `data-render-src="name:BlockName"` für ein Bild-Bestandteil im Block "Präsentation" einer [mehrteiligen Anforderung](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="e23f7-192">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span><br/><br/><span data-ttu-id="e23f7-193">Diese Methode ist nützlich, wenn die Webseite so komplex ist, dass sie nicht zuverlässig von OneNote analysiert werden kann, oder wenn für die Seite eine Anmeldung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e23f7-193">data-render-src="name:BlockName" for an image part in the Presentation block of a multi-part request. This method is useful when the webpage is more complex than the onnvshort page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="e23f7-194">data-tag</span><span class="sxs-lookup"><span data-stu-id="e23f7-194">data-tag</span></span> | <span data-ttu-id="e23f7-195">Ein [Notiztag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-195">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="e23f7-196">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-196">style</span></span> |<span data-ttu-id="e23f7-197">Die Position- und Größen-Eigenschaften für das Bild: **Position** (nur **absolute**), **links**, **oben**, **Breite** und **Höhe**.</span><span class="sxs-lookup"><span data-stu-id="e23f7-197">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="e23f7-198">Die Größe kann für jedes Bild festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="e23f7-198">Size can be set on any image.</span></span> <span data-ttu-id="e23f7-199">Positionseigenschaften werden verwendet, um ein [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)-Bild zu erstellen, wenn das Bild ein direktes untergeordnetes Element des Textkörpers und für den Textkörper `data-absolute-enabled="true"` angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="e23f7-199">Position properties are used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="e23f7-200">Beispiel: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="e23f7-200">Example`<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="e23f7-201">In der Ausgabe-HTML wird die Bildgröße separat in **width**- und **height**-Attributen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e23f7-201">In the output HTML, the image size is returned separately in  **width** and **height** attributes.</span></span> |
| <span data-ttu-id="e23f7-202">src</span><span class="sxs-lookup"><span data-stu-id="e23f7-202">src</span></span> |<span data-ttu-id="e23f7-203">Es ist entweder **src** oder **data-render-src** erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e23f7-203">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="e23f7-204">Das Bild, das auf der OneNote-Seite gerendert werden soll:</span><span class="sxs-lookup"><span data-stu-id="e23f7-204">The image to render on the onnvshort page:</span></span><br /> <span data-ttu-id="e23f7-205">- `src="http://..."` für eine URL zu einem öffentlich verfügbaren Bild im Internet.</span><span class="sxs-lookup"><span data-stu-id="e23f7-205">src="http://..." for a URL to a publicly available image on the internet.</span></span><br /> <span data-ttu-id="e23f7-206">- `src="name:BlockName"` für einen benannten Teil in einer mehrteiligen Anforderung, die das Bild darstellt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-206">src="name:BlockName" for a named part in a multi-part request that represents the image.</span></span>|
| <span data-ttu-id="e23f7-207">Breite, Höhe</span><span class="sxs-lookup"><span data-stu-id="e23f7-207">width, height</span></span> | <span data-ttu-id="e23f7-208">Die Breite oder Höhe des Bilds, in Pixel, aber ohne px.</span><span class="sxs-lookup"><span data-stu-id="e23f7-208">The width or height of the image, in pixels but without the px. Example: width="400"</span></span> <span data-ttu-id="e23f7-209">Beispiel: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="e23f7-209">Example`width="400"`</span></span> |
 
><span data-ttu-id="e23f7-210">**Hinweis:** Die OneNote-APIs erkennt automatisch den Eingabe-Bildtyp und gibt ihn als **data-fullres-src-type** an die Ausgabe-HTML zurück.</span><span class="sxs-lookup"><span data-stu-id="e23f7-210">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="e23f7-211">Die API gibt auch den Bildtyp des optimierten Bilds in **data-src-type** zurück.</span><span class="sxs-lookup"><span data-stu-id="e23f7-211">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

<span data-ttu-id="e23f7-212">**Ausgabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-212">**Output attributes**</span></span>

|<span data-ttu-id="e23f7-213">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-213">Output attribute</span></span>|<span data-ttu-id="e23f7-214">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-214">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-215">alt</span><span class="sxs-lookup"><span data-stu-id="e23f7-215">alt</span></span> | <span data-ttu-id="e23f7-216">Der angegebene Alternativtext für das Bild.</span><span class="sxs-lookup"><span data-stu-id="e23f7-216">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="e23f7-217">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-217">data-id</span></span> | <span data-ttu-id="e23f7-218">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-218">A reference for the element.</span></span> <span data-ttu-id="e23f7-219">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-219">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-220">data-index</span><span class="sxs-lookup"><span data-stu-id="e23f7-220">data-index</span></span> | <span data-ttu-id="e23f7-221">Die Ausrichtung des Bildes.</span><span class="sxs-lookup"><span data-stu-id="e23f7-221">The position properties of the image.</span></span> <span data-ttu-id="e23f7-222">Für die Unterstützung von [geteilten Bildern](#split-images).</span><span class="sxs-lookup"><span data-stu-id="e23f7-222">For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="e23f7-223">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="e23f7-223">data-fullres-src</span></span> | <span data-ttu-id="e23f7-224">Der Endpunkt für die Version der Bildressource, die ursprünglich in die Seite eingebettet war.</span><span class="sxs-lookup"><span data-stu-id="e23f7-224">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="e23f7-225">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="e23f7-225">data-fullres-src-type</span></span> | <span data-ttu-id="e23f7-226">Der Medientyp der **data-fullres-src**-Ressource. Beispiel: `image/png` oder `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="e23f7-226">The MIME type of the **data-fullres-src** resource, for example: image/png`image/png` or image/jpeg`image/jpeg`.</span></span> |
| <span data-ttu-id="e23f7-227">data-options</span><span class="sxs-lookup"><span data-stu-id="e23f7-227">data-options</span></span> | <span data-ttu-id="e23f7-228">Der Typ der Datenquelle: **printout** für PDF-Dateien oder **splitimage** für alle anderen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-228">The source type: **printout** for PDF files or **splitimage** for all others. Applies only to split images created with the data-render-src attribute.</span></span> <span data-ttu-id="e23f7-229">Gilt nur für [geteilte Bilder](#split-images), die mit dem **data-render-src**-Attribut erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="e23f7-229">The source type: **printout** for PDF files or splitimage for all others. Applies only to [split images](#split-images) created with the data-render-src attribute.</span></span> |
| <span data-ttu-id="e23f7-230">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="e23f7-230">data-render-original-src</span></span> | <span data-ttu-id="e23f7-231">Die ursprüngliche URL des Bilds, wenn das Quellbild aus dem öffentlichen Internet stammt und mit dem **data-render-src**-Attribut erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e23f7-231">The original source URL of the image, if the source image  is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="e23f7-232">data-src-type</span><span class="sxs-lookup"><span data-stu-id="e23f7-232">data-src-type</span></span> | <span data-ttu-id="e23f7-233">Der Medientyp der **src**-Ressource. Beispiel: `image/png` oder `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="e23f7-233">The MIME type of the **src** resource, for example: image/png`image/png` or image/jpeg`image/jpeg`.</span></span> |
| <span data-ttu-id="e23f7-234">data-tag</span><span class="sxs-lookup"><span data-stu-id="e23f7-234">data-tag</span></span> | <span data-ttu-id="e23f7-235">Ein [Notiztag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-235">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="e23f7-236">id</span><span class="sxs-lookup"><span data-stu-id="e23f7-236">id</span></span> | <span data-ttu-id="e23f7-237">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-237">A unique ID for the group.</span></span> <span data-ttu-id="e23f7-238">Zurückgegeben von einem [GET requests to a page's*-content*-Endpunkt ](../api-reference/v1.0/api/page_get.md), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e23f7-238">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="e23f7-239">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-239">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-240">src</span><span class="sxs-lookup"><span data-stu-id="e23f7-240">src</span></span> | <span data-ttu-id="e23f7-241">Der Endpunkt für die Version der Bildressource, die für Webbrowser sowie mobile Geräte und Tablets optimiert wurde.</span><span class="sxs-lookup"><span data-stu-id="e23f7-241">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="e23f7-242">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-242">style</span></span> | <span data-ttu-id="e23f7-243">Die Positionseigenschaften des Bilds.</span><span class="sxs-lookup"><span data-stu-id="e23f7-243">The position properties of the image.</span></span> |
| <span data-ttu-id="e23f7-244">width, height</span><span class="sxs-lookup"><span data-stu-id="e23f7-244">width, height</span></span> | <span data-ttu-id="e23f7-245">Die Breite oder Höhe des Bilds in Pixel.</span><span class="sxs-lookup"><span data-stu-id="e23f7-245">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="e23f7-246">Beispiele für die Ausgabe-HTML für Bilder</span><span class="sxs-lookup"><span data-stu-id="e23f7-246">Output HTML examples for images</span></span>
<span data-ttu-id="e23f7-247">Ausgabe-**img**-Elemente enthalten die Endpunkte für Bilddateiressourcen und den Bildtyp (siehe  unten).</span><span class="sxs-lookup"><span data-stu-id="e23f7-247">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="e23f7-248">Sie können separate [GET-Anforderung zu Bildressourcen-Endpunkten](../api-reference/v1.0/api/resource_get.md) durchführen, um die binäre Inhalt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-248">Output object elements  contain  endpoints that link to the file resources in the page. You can make separate GET requests to these resource endpoints to retrieve their binary contents.</span></span>

```http
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="e23f7-249">Standardmäßig können Bilder nicht direkt in einem Browser gerendert werden, da sie wie die restlichen Seiteninhalte privat sind und eine Autorisierung erforderlich ist, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-249">Images won’t render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="e23f7-250">Um Öffentliche URLs für die Bildressourcen auf einer Seite zu erhalten, fügen Sie **preAuthenticated=true** in die Abfragezeichenfolge ein, wenn Sie die Seiteninhalte abrufen (Beispiel: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="e23f7-250">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="e23f7-251">Die öffentlichen URLs, die zurückgegeben werden, sind eine Stunde lang gültig.</span><span class="sxs-lookup"><span data-stu-id="e23f7-251">The public URLs that are returned are valid for one hour.</span></span> 

<span data-ttu-id="e23f7-252">**Bild mit öffentlichen URL, wenn _vorauthentifiziert = True_ in der Anfrage enthalten ist**</span><span class="sxs-lookup"><span data-stu-id="e23f7-252">**Image with public URL when _preAuthenticated=true_ is included in the request**</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}" />
```

<span data-ttu-id="e23f7-253">Die folgenden Beispiele zeigen, welche Informationen ein **img**-Element in der Ausgabe-HTML enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="e23f7-253">The following examples show the information an **img** element might contain in the output HTML.</span></span>

<span data-ttu-id="e23f7-254">**Bild mit webfähigen Ressourcen in hoher Auflösung**</span><span class="sxs-lookup"><span data-stu-id="e23f7-254">**Image with web-ready and high resolution resources**</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    [data-render-original-src="{original-source-url-or-named-part}"]
    [data-id="{image-id}"]
    [alt="supplied alt text"]
    [width="345"] [height="180"]
    [style="..."] />
```

<span data-ttu-id="e23f7-255">**Mit dem *data-render-src*-Attribut erstelltes Bild**</span><span class="sxs-lookup"><span data-stu-id="e23f7-255">**Image created by using the *data-render-src* attribute**</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    data-render-original-src="{original-source-url-or-named-part}"
    [data-id="{image-id}"]
    [data-index="{index-of-split-image}"]
    [data-options="{printout-or-splitimage}"]
    [alt="supplied alt text"]
    [width="1024"] [height="1900"]
    [style="..."] />
```

### <a name="split-images"></a><span data-ttu-id="e23f7-256">Aufteilen von Bildern</span><span class="sxs-lookup"><span data-stu-id="e23f7-256">Split images</span></span>

<span data-ttu-id="e23f7-257">Bilder, die mit dem **data-render-src**-Attribut (aus einer Webseiten-URL oder einem benannten Teil) erstellt werden, werden für eine bessere Leistung und ein besseres Rendering möglicherweise in aus mehreren Komponenten bestehende Bilder aufgeteilt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-257">Images that are created using the **data-render-src** attribute from a webpage URL or a named part might be split into multiple component images for performance and rendering reasons. Component images are all assigned the same data-id value.  Each component image has a zero-based data-index attribute that defines the  original vertical layout.</span></span> <span data-ttu-id="e23f7-258">Komponenten-Bildern wird allen der gleiche **data-id**-Wert zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-258">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="e23f7-259">Jedes Komponenten-Bild verfügt über ein nullbasiertes data-index-Attribut, welches das ursprüngliche vertikale Layout definiert.</span><span class="sxs-lookup"><span data-stu-id="e23f7-259">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

<span data-ttu-id="e23f7-260">**Aufgeteiltes Bild mit drei Komponentenbildern**</span><span class="sxs-lookup"><span data-stu-id="e23f7-260">**Split image with three component images**</span></span>

```html
<div data-id="multi-component-image" style="position:absolute;left:48px;top:120px;width:624px">
    <img
        src="{image-resource0-url}/$value"
        data-src-type="image/{type}"
        data-fullres-src="{image-resource0-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="0" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource1-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource1-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="1" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource2-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource2-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="2" 
        data-render-original-src=""{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
</div>
```

<span data-ttu-id="e23f7-261">Da Benutzer die Bilder auf der Seite verschieben können, werden die Indizes möglicherweise in falscher Reihenfolge zurückgegebenen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-261">Because users can move the images on the page, the returned indexes might be out of order.
Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span> <span data-ttu-id="e23f7-262">Die Sortierung erfolgt normalerweise von oben nach unten auf der Y-Achse und von links nach rechts auf der X-Achse, wenn es Konflikte mit der Y-Sortierung gibt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-262">Because users can move the images on the page, the returned indexes might be out of order.
Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="e23f7-263">iframe-Elemente</span><span class="sxs-lookup"><span data-stu-id="e23f7-263">iframe elements</span></span>
<span data-ttu-id="e23f7-264">OneNote-Seiten können eingebettete Videos enthalten, die durch **iframe**-Elemente dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="e23f7-264">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

><span data-ttu-id="e23f7-265">**Hinweis:** Sie können auch [eine Videodatei mithilfe eines **object**-Elements](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files) anfügen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-265">**Note:** You can also [attach a video file using an **object** element](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files).</span></span>

<span data-ttu-id="e23f7-266">**Eingabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-266">**Input attributes**</span></span>

|<span data-ttu-id="e23f7-267">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-267">Input attribute</span></span>|<span data-ttu-id="e23f7-268">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-268">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-269">data-original-src</span><span class="sxs-lookup"><span data-stu-id="e23f7-269">data-original-src</span></span> | <span data-ttu-id="e23f7-270">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e23f7-270">Required.</span></span> <span data-ttu-id="e23f7-271">Die URL der Videoquelle.</span><span class="sxs-lookup"><span data-stu-id="e23f7-271">The URL of the video source.</span></span> <span data-ttu-id="e23f7-272">Siehe [Liste der unterstützten Videoquellen](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span><span class="sxs-lookup"><span data-stu-id="e23f7-272">See the [list of supported video sources](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span></span> <span data-ttu-id="e23f7-273">Beispiel: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="e23f7-273">Example`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="e23f7-274">Breite, Höhe</span><span class="sxs-lookup"><span data-stu-id="e23f7-274">width, height</span></span> | <span data-ttu-id="e23f7-275">Die Breite oder Höhe des iframe in Pixel.</span><span class="sxs-lookup"><span data-stu-id="e23f7-275">The width or height of the image, in pixels.</span></span> <span data-ttu-id="e23f7-276">Beispiel: `width=300`</span><span class="sxs-lookup"><span data-stu-id="e23f7-276">Example`width=300`</span></span> |

<span data-ttu-id="e23f7-277">**Ausgabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-277">**Output attributes**</span></span>

|<span data-ttu-id="e23f7-278">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-278">Output attribute</span></span>|<span data-ttu-id="e23f7-279">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-279">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-280">data-original-src</span><span class="sxs-lookup"><span data-stu-id="e23f7-280">data-original-src</span></span> | <span data-ttu-id="e23f7-281">Die URL der Videoquelle.</span><span class="sxs-lookup"><span data-stu-id="e23f7-281">The URL of the video source.</span></span> |
| <span data-ttu-id="e23f7-282">src</span><span class="sxs-lookup"><span data-stu-id="e23f7-282">src</span></span> | <span data-ttu-id="e23f7-283">Ein Link zu dem Video, das in die OneNote-Seite eingebettet ist.</span><span class="sxs-lookup"><span data-stu-id="e23f7-283">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="e23f7-284">Breite, Höhe</span><span class="sxs-lookup"><span data-stu-id="e23f7-284">width, height</span></span> | <span data-ttu-id="e23f7-285">Die Breite oder Höhe des iframe in Pixel.</span><span class="sxs-lookup"><span data-stu-id="e23f7-285">The width or height of the image, in pixels.</span></span> <span data-ttu-id="e23f7-286">Beispiel: `width=300`</span><span class="sxs-lookup"><span data-stu-id="e23f7-286">Example`width=300`</span></span> |
 
<span data-ttu-id="e23f7-287">Beispiel für eine **Ausgabe-HTML** eines Videos</span><span class="sxs-lookup"><span data-stu-id="e23f7-287">Output HTML example for objects</span></span>

<span data-ttu-id="e23f7-288">Ausgabe-**iframe**-Elemente enthalten Endpunkte, die wie dargestellt auf die Quellseite und das Video verweisen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-288">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="e23f7-289">Object-Elemente</span><span class="sxs-lookup"><span data-stu-id="e23f7-289">Object elements</span></span>
<span data-ttu-id="e23f7-290">OneNote-Seiten können Dateianlagen enthalten, die durch **object**-Elemente dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="e23f7-290">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="e23f7-291">Das **object**-Element kann die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-291">onnvshort pages can contain file attachments  represented by **object** elements. An object element can contain the following attributes in the input and output HTML.</span></span>

><span data-ttu-id="e23f7-292">**Hinweis:** OneNote-APIs können auch Dateiinhalte als Bilder auf einer Seite rendern, wenn die Datei als Bild gesendet und das Attribut **data-render-src** verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e23f7-292">The onnvshort API can also render file content as images in a page when the file is sent as an image and uses the data-render-src attribute.  Example: <img data-render-src="name:BlockName" ... /></span></span> <span data-ttu-id="e23f7-293">Beispiel: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="e23f7-293">Example`<img data-render-src="name:part-name" ... />`</span></span>
 

<span data-ttu-id="e23f7-294">**Eingabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-294">**Input attributes**</span></span>

|<span data-ttu-id="e23f7-295">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-295">Input attribute</span></span>|<span data-ttu-id="e23f7-296">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-296">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-297">data</span><span class="sxs-lookup"><span data-stu-id="e23f7-297">data</span></span> | <span data-ttu-id="e23f7-298">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e23f7-298">Required.</span></span> <span data-ttu-id="e23f7-299">Der Name des Teils, der die Datei in der [mehrteiligen Anforderung](../api-reference/v1.0/api/section_post_pages.md#example) darstellt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-299">Required. The name of the part that represents the file in the multi-part request.</span></span> |
| <span data-ttu-id="e23f7-300">data-attachment</span><span class="sxs-lookup"><span data-stu-id="e23f7-300">data-attachment</span></span> | <span data-ttu-id="e23f7-p137">Erforderlich. Der Dateiname.</span><span class="sxs-lookup"><span data-stu-id="e23f7-p137">Required. The file name.</span></span> |
| <span data-ttu-id="e23f7-303">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-303">data-id</span></span> | <span data-ttu-id="e23f7-304">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-304">A reference for the element.</span></span> <span data-ttu-id="e23f7-305">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-305">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-306">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-306">style</span></span> | <p><span data-ttu-id="e23f7-307">Die Position- und Größen-Eigenschaften für das Objekt: **Position** (nur **absolute**), **links**, **oben** und **Breite**.</span><span class="sxs-lookup"><span data-stu-id="e23f7-307">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span></p><p><span data-ttu-id="e23f7-308">Wird verwendet, um ein [absolut positioniertes](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)-Object-Element zu erstellen, wenn das Object-Element ein direktes untergeordnetes Element des Textkörpers und für den Textkörper `data-absolute-enabled="true"` angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="e23f7-308">position (absolute only), left, top, and width properties. Used to create an absolutely positioned object, only if the object is a direct child of the body when the  body sets data-absolute-enabled="true". Learn more about absolutely positioned elements. Example: <object style="position:absolute;top:350px;left:300px" ... /></span></span><br /><span data-ttu-id="e23f7-309">Beispiel: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="e23f7-309">Example`<object style="position:absolute;top:350px;left:300px" ... />`</span></span></p> |
| <span data-ttu-id="e23f7-310">type</span><span class="sxs-lookup"><span data-stu-id="e23f7-310">type</span></span> | <span data-ttu-id="e23f7-311">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e23f7-311">Required.</span></span> <span data-ttu-id="e23f7-312">Der standardmäßige Mediendateityp.</span><span class="sxs-lookup"><span data-stu-id="e23f7-312">The standard MIME file type.</span></span> <span data-ttu-id="e23f7-313">Bei bekannten Dateitypen wird das dem Dateityp zugeordnete Symbol auf der OneNote-Seite angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-313">Required. The standard MIME file type.  Known file types display the icon associated with the file type on the onnvshort page. Unknown file types display a generic file icon.</span></span> <span data-ttu-id="e23f7-314">Bei unbekannten Dateitypen wird ein generisches Symbol angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-314">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

<span data-ttu-id="e23f7-315">**Ausgabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-315">**Output attributes**</span></span>

|<span data-ttu-id="e23f7-316">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-316">Output attribute</span></span>|<span data-ttu-id="e23f7-317">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-317">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-318">data</span><span class="sxs-lookup"><span data-stu-id="e23f7-318">data</span></span> | <span data-ttu-id="e23f7-319">Der Endpunkt für die Dateiressource.</span><span class="sxs-lookup"><span data-stu-id="e23f7-319">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="e23f7-320">data-attachment</span><span class="sxs-lookup"><span data-stu-id="e23f7-320">data-attachment</span></span> | <span data-ttu-id="e23f7-321">Der Dateiname.</span><span class="sxs-lookup"><span data-stu-id="e23f7-321">The file name.</span></span> |
| <span data-ttu-id="e23f7-322">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-322">data-id</span></span> | <span data-ttu-id="e23f7-323">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-323">A reference for the element.</span></span> <span data-ttu-id="e23f7-324">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-324">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-325">id</span><span class="sxs-lookup"><span data-stu-id="e23f7-325">id</span></span> | <span data-ttu-id="e23f7-326">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-326">A unique ID for the group.</span></span> <span data-ttu-id="e23f7-327">Zurückgegeben von einem [GET requests to a page's*-content*-Endpunkt ](../api-reference/v1.0/api/page_get.md), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e23f7-327">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="e23f7-328">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-328">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-329">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-329">style</span></span> | <span data-ttu-id="e23f7-330">Die Positionseigenschaften des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e23f7-330">The position properties of the object.</span></span> |
| <span data-ttu-id="e23f7-331">type</span><span class="sxs-lookup"><span data-stu-id="e23f7-331">type</span></span> | <span data-ttu-id="e23f7-332">Der standardmäßige Mediendateityp.</span><span class="sxs-lookup"><span data-stu-id="e23f7-332">The standard MIME file type.</span></span> |
 

<span data-ttu-id="e23f7-333">Beispiele für die **Ausgabe-HTML** bei Objekten</span><span class="sxs-lookup"><span data-stu-id="e23f7-333">Output HTML example for objects</span></span>

<span data-ttu-id="e23f7-334">Ausgabe-**object**-Elemente enthalten Endpunkte, die wie dargestellt auf Dateiressourcen auf der Seite verweisen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-334">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="e23f7-335">Sie können separate [GET-Anforderung zu Dateiressourcen-Endpunkten](../api-reference/v1.0/api/resource_get.md) durchführen, um die binäre Inhalt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-335">Output object elements  contain  endpoints that link to the file resources in the page. You can make separate GET requests to these resource endpoints to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="e23f7-336">Absätze und Überschriften</span><span class="sxs-lookup"><span data-stu-id="e23f7-336">Paragraphs and headings</span></span>

<span data-ttu-id="e23f7-337">Absätze, Überschriften und andere Textcontainer können die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-337">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="e23f7-338">**Eingabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-338">**Input attributes**</span></span>

|<span data-ttu-id="e23f7-339">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-339">Input attribute</span></span>|<span data-ttu-id="e23f7-340">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-340">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-341">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-341">data-id</span></span> | <span data-ttu-id="e23f7-342">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-342">A reference for the element.</span></span> <span data-ttu-id="e23f7-343">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-343">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-344">data-tag</span><span class="sxs-lookup"><span data-stu-id="e23f7-344">data-tag</span></span> | <span data-ttu-id="e23f7-345">Ein  [Notiztag ](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) für ein **p**- oder **h1** - **h6**-Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-345">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="e23f7-346">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-346">style</span></span> | <span data-ttu-id="e23f7-347">Die CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="e23f7-347">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="e23f7-348">**Ausgabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-348">**Output attributes**</span></span>

|<span data-ttu-id="e23f7-349">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-349">Output attribute</span></span>|<span data-ttu-id="e23f7-350">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-350">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-351">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-351">data-id</span></span> | <span data-ttu-id="e23f7-352">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-352">A reference for the element.</span></span> <span data-ttu-id="e23f7-353">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-353">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-354">data-tag</span><span class="sxs-lookup"><span data-stu-id="e23f7-354">data-tag</span></span> | <span data-ttu-id="e23f7-355">Ein  [Notiztag ](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) für ein **p**- oder **h1** - **h6**-Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-355">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="e23f7-356">id</span><span class="sxs-lookup"><span data-stu-id="e23f7-356">id</span></span> | <span data-ttu-id="e23f7-357">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-357">A unique ID for the group.</span></span> <span data-ttu-id="e23f7-358">Zurückgegeben von einem [GET requests to a page's*-content*-Endpunkt ](../api-reference/v1.0/api/page_get.md), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e23f7-358">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="e23f7-359">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-359">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-360">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-360">style</span></span> | <span data-ttu-id="e23f7-361">Die CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="e23f7-361">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="e23f7-362">In der Ausgabe-HTML können diese Werte eingebettet in die entsprechenden untergeordneten Elemente oder in **span**-Elementen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e23f7-362">The CSS style properties of the element. In the output HTML, these values may be returned on inline on appropriate child elements or span elements.</span></span> |
 

<span data-ttu-id="e23f7-363">Die folgenden Beispiele zeigen Eingabe-HTML, die verschiedene Möglichkeiten zum Definieren von Formatvorlagen für Textcontainer verwendet, und die zurückgegebene Ausgabe-HTML.</span><span class="sxs-lookup"><span data-stu-id="e23f7-363">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

<span data-ttu-id="e23f7-364">**Eingabe-HTML**, in der Formatvorlagen mit Inlinezeichenformaten, im Starttag und in einem **span**-Element definiert sind.</span><span class="sxs-lookup"><span data-stu-id="e23f7-364">**Input HTML** with styles defined using inline character styles, in the start tag,  and within a **span** element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

<span data-ttu-id="e23f7-365">**Ausgabe-HTML**, in der das `<i>`-Zeichenformat und die Schriftarteinstellungen im `<p>`-Starttag als Inline-CSS-Formate in **span**-Elementen zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e23f7-365">**Output HTML** with the **<i>`<i>` character style and the font settings in the <p>`<p>` start tag returned as inline CSS styles on span** elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="e23f7-366">Listen</span><span class="sxs-lookup"><span data-stu-id="e23f7-366">Lists</span></span>
<span data-ttu-id="e23f7-367">Listen werden als **ol**- oder **ul**-Elemente dargestellt, die **li**-Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-367">
 


Lists are represented as ol or ul elements that can contain li elements.</span></span>

<span data-ttu-id="e23f7-368">Listen und Listenelemente können die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-368">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="e23f7-369">**Eingabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-369">**Input attributes**</span></span>

|<span data-ttu-id="e23f7-370">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-370">Input attribute</span></span>|<span data-ttu-id="e23f7-371">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-371">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-372">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-372">data-id</span></span> | <span data-ttu-id="e23f7-373">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-373">A reference for the element.</span></span> <span data-ttu-id="e23f7-374">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-374">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-375">data-tag</span><span class="sxs-lookup"><span data-stu-id="e23f7-375">data-tag</span></span> | <span data-ttu-id="e23f7-376">Ein [Notiztag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) für ein **ul**-, **ol**- oder **li**-Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-376">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="e23f7-377">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-377">style</span></span> | <span data-ttu-id="e23f7-378">Die **list-style-type**- und die CSS-[style](#styles)-Eigenschaften für die Liste oder das Listenelement.</span><span class="sxs-lookup"><span data-stu-id="e23f7-378">The **list-style-type** and the  CSS [style](#styles) properties for the list or list item.</span></span> |
 

<span data-ttu-id="e23f7-379">**Ausgabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-379">**Output attributes**</span></span>

|<span data-ttu-id="e23f7-380">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-380">Output attribute</span></span>|<span data-ttu-id="e23f7-381">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-381">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-382">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-382">data-id</span></span> | <span data-ttu-id="e23f7-383">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-383">A reference for the element.</span></span> <span data-ttu-id="e23f7-384">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-384">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-385">data-tag</span><span class="sxs-lookup"><span data-stu-id="e23f7-385">data-tag</span></span> |  <span data-ttu-id="e23f7-386">Ein [Notiztag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) in einem **li**-Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-386">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **span** in a li element.</span></span> |
| <span data-ttu-id="e23f7-387">id</span><span class="sxs-lookup"><span data-stu-id="e23f7-387">id</span></span> | <span data-ttu-id="e23f7-388">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-388">A unique ID for the group.</span></span> <span data-ttu-id="e23f7-389">Zurückgegeben von einem [GET requests to a page's*-content*-Endpunkt ](../api-reference/v1.0/api/page_get.md), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e23f7-389">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="e23f7-390">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-390">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-391">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-391">style</span></span> | <span data-ttu-id="e23f7-392">Die **list-style-type**- und CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="e23f7-392">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="e23f7-393">In der Ausgabe HTML werden die Listenebene-Einstellungen an die  Listenelemente zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e23f7-393">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="e23f7-394">Standard-Eigenschaften werden nicht zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="e23f7-394">The following properties are not returned:</span></span> |
 

<span data-ttu-id="e23f7-395">Die OneNote-APIs in Microsoft Graph unterstützen die folgenden Listentypen:</span><span class="sxs-lookup"><span data-stu-id="e23f7-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="e23f7-396">Sortierte Liste</span><span class="sxs-lookup"><span data-stu-id="e23f7-396">Ordered list</span></span>|<span data-ttu-id="e23f7-397">Unsortierte Liste</span><span class="sxs-lookup"><span data-stu-id="e23f7-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-398">keine</span><span class="sxs-lookup"><span data-stu-id="e23f7-398">none</span></span> | <span data-ttu-id="e23f7-399">Keine</span><span class="sxs-lookup"><span data-stu-id="e23f7-399">none</span></span> |
| <span data-ttu-id="e23f7-400">
decimal (Standard)</span><span class="sxs-lookup"><span data-stu-id="e23f7-400">decimal (default)</span></span> | <span data-ttu-id="e23f7-401">
disc (Standard)</span><span class="sxs-lookup"><span data-stu-id="e23f7-401">disc (default)</span></span> |
| <span data-ttu-id="e23f7-402">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="e23f7-402">lower-alpha</span></span> | <span data-ttu-id="e23f7-403">circle</span><span class="sxs-lookup"><span data-stu-id="e23f7-403">Circle</span></span> |
| <span data-ttu-id="e23f7-404">lower-roman</span><span class="sxs-lookup"><span data-stu-id="e23f7-404">lower-roman</span></span> | <span data-ttu-id="e23f7-405">

square</span><span class="sxs-lookup"><span data-stu-id="e23f7-405">square</span></span> |
| <span data-ttu-id="e23f7-406">
upper-alpha</span><span class="sxs-lookup"><span data-stu-id="e23f7-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="e23f7-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="e23f7-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="e23f7-408">Sie können globale Formatvorlagen für eine Liste im **ol**- oder **ul**-Element in der Eingabe-HTML anwenden, aber Formatvorlagen werden in den **li**-Elementen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e23f7-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

<span data-ttu-id="e23f7-409">**Homogene Listenformatvorlage**</span><span class="sxs-lookup"><span data-stu-id="e23f7-409">**Homogenous list style**</span></span>

<span data-ttu-id="e23f7-410">Dieses Beispiel zeigt Eingabe-HTML, die den Listenformattyp im **ol**-Element und CSS-Formatvorlagen in einzelnen Listenelementen festlegt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="e23f7-411">Dies ist die Ausgabe-HTML.</span><span class="sxs-lookup"><span data-stu-id="e23f7-411">This is the output HTML.</span></span> <span data-ttu-id="e23f7-412">Beachten Sie, dass Formatvorlagen inline in den einzelnen **li**- oder **span**-Elementen zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e23f7-412">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

<span data-ttu-id="e23f7-413">**Variable Listenelementvorlagen**</span><span class="sxs-lookup"><span data-stu-id="e23f7-413">**Variable list styles**</span></span>

<span data-ttu-id="e23f7-414">Dieses Beispiel zeigt Eingabe-HTML, die verschiedene Listenformattypen in den **li**-Elementen festlegt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="e23f7-415">Dies ist die Ausgabe-HTML.</span><span class="sxs-lookup"><span data-stu-id="e23f7-415">This is the output HTML.</span></span> <span data-ttu-id="e23f7-416">Beachten Sie, dass Formatvorlagen inline in den einzelnen **li**- oder **span**-Elementen zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e23f7-416">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="e23f7-417">Tabellen</span><span class="sxs-lookup"><span data-stu-id="e23f7-417">Tables</span></span>
<span data-ttu-id="e23f7-418">Tabellen werden als **table**-Elemente dargestellt, die **tr**- und **td**-Elemente enthalten können.</span><span class="sxs-lookup"><span data-stu-id="e23f7-418">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span> <span data-ttu-id="e23f7-419">Verschachtelte Tabellen werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-419">Nested tables are supported.</span></span>

<span data-ttu-id="e23f7-420">Tabellen können die folgenden Attribute in der Eingabe- und Ausgabe-HTML enthalten.</span><span class="sxs-lookup"><span data-stu-id="e23f7-420">Lists and list items can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="e23f7-421">Die OneNote-APIs unterstützen keine **rowspan**- oder **colspan**-Attribute.</span><span class="sxs-lookup"><span data-stu-id="e23f7-421">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

<span data-ttu-id="e23f7-422">**Eingabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-422">**Input attributes**</span></span>

|<span data-ttu-id="e23f7-423">Eingabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-423">Input attribute</span></span>|<span data-ttu-id="e23f7-424">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-425">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-425">data-id</span></span> | <span data-ttu-id="e23f7-426">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-426">A reference for the element.</span></span> <span data-ttu-id="e23f7-427">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-427">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-428">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-428">style</span></span> | <span data-ttu-id="e23f7-429">Die CSS-[style](#styles)-Eigenschaften des Elements und:</span><span class="sxs-lookup"><span data-stu-id="e23f7-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="e23f7-430">- **border**.</span><span class="sxs-lookup"><span data-stu-id="e23f7-430">Border</span></span> <span data-ttu-id="e23f7-431">Kann entweder 0px oder 1px sein.</span><span class="sxs-lookup"><span data-stu-id="e23f7-431">border. Can be either 0px or 1px.</span></span><br /> <span data-ttu-id="e23f7-432">- **width**.</span><span class="sxs-lookup"><span data-stu-id="e23f7-432">width</span></span> <span data-ttu-id="e23f7-433">**width**. Unterstützt von **table** und td als Pixel oder Prozentsatz der Seitenbreite.</span><span class="sxs-lookup"><span data-stu-id="e23f7-433">**width**. Supported by **table** and td as pixels or percentage of page width. Example: width="100px" or width="60%"</span></span><br /><span data-ttu-id="e23f7-434">Beispiele: `width="100px"` oder `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="e23f7-434">Example: `width="100px"` or `width="60%"`</span></span> |
 

<span data-ttu-id="e23f7-435">**Ausgabeattribute**</span><span class="sxs-lookup"><span data-stu-id="e23f7-435">**Output attributes**</span></span>

|<span data-ttu-id="e23f7-436">Ausgabeattribut</span><span class="sxs-lookup"><span data-stu-id="e23f7-436">Output attribute</span></span>|<span data-ttu-id="e23f7-437">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e23f7-437">Description</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-438">data-id</span><span class="sxs-lookup"><span data-stu-id="e23f7-438">data-id</span></span> | <span data-ttu-id="e23f7-439">Ein Verweis für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-439">A reference for the element.</span></span> <span data-ttu-id="e23f7-440">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-440">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-441">id</span><span class="sxs-lookup"><span data-stu-id="e23f7-441">id</span></span> | <span data-ttu-id="e23f7-442">Eine eindeutige generierte ID für das Element.</span><span class="sxs-lookup"><span data-stu-id="e23f7-442">A unique ID for the group.</span></span> <span data-ttu-id="e23f7-443">Zurückgegeben von einem [GET requests to a page's*-content*-Endpunkt ](../api-reference/v1.0/api/page_get.md), wenn die `includeIDs=true`-Abfrageoption verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e23f7-443">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="e23f7-444">Wird verwendet, um [Seiteninhalt zu aktualisieren](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-444">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="e23f7-445">Formatvorlage</span><span class="sxs-lookup"><span data-stu-id="e23f7-445">style</span></span> | <span data-ttu-id="e23f7-446">Die CSS-[style](#styles)-Eigenschaften des Elements.</span><span class="sxs-lookup"><span data-stu-id="e23f7-446">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="e23f7-447">Die folgenden Beispiele zeigen Eingabe-HTML, die verschiedene Möglichkeiten zum Definieren von Formatvorlagen für Tabellen verwendet, und die zurückgegebene Ausgabe-HTML.</span><span class="sxs-lookup"><span data-stu-id="e23f7-447">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

<span data-ttu-id="e23f7-448">**Eingabe HTML** mit optionalen Einstellungen auf verschiedenen Ebenen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-448">**Input HTML** with optional settings at different levels.</span></span>

```html
<table style="border:0px;width:500px;background-color:green">
    <tr> 
        <td>Cell 1</td> 
        <td>Cell 2</td> 
        <td>Cell 3</td> 
    </tr> 
    <tr style="background-color:blue"> 
        <td style="text-align:right;background-color:red">Left</td> 
        <td style="text-align:center">Middle</td> 
        <td>Right</td> 
    </tr> 
</table>
```
 
<span data-ttu-id="e23f7-449">**Ausgabe-HTML** mit inline in **td**-Elementen zurückgegebenen CSS-Formatvorlagen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-449">**Output HTML** with CSS styles returned inline on the **td** elements.</span></span>

```html
<table style="border:0px">
    <tr>
        <td style="background-color:green;width:166;border:0px">Cell 1</td>
        <td style="background-color:green;width:166;border:0px">Cell 2</td>
        <td style="background-color:green;width:166;border:0px">Cell 3</td>
    </tr>
    <tr>
        <td style="background-color:red;width:166;border:0px;text-align:right">Left</td>
        <td style="background-color:blue;width:166;border:0px;text-align:center">Middle</td>
        <td style="background-color:blue;width:166;border:0px">Right</td>
    </tr>
</table>
``` 


## <a name="styles"></a><span data-ttu-id="e23f7-450">Formatvorlagen</span><span class="sxs-lookup"><span data-stu-id="e23f7-450">Styles</span></span>
<span data-ttu-id="e23f7-451">OneNote APIs in Microsoft Graph unterstützt die folgenden Inline-CSS-**style**-Eigenschaften für Elemente im Seitentextkörper, wie **body**, **div**, **p**, **li** und **span**.</span><span class="sxs-lookup"><span data-stu-id="e23f7-451">The onnvshort API supports the following inline CSS style properties for elements in the page body, such as body, div, p, li, and span.</span></span>

|<span data-ttu-id="e23f7-452">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e23f7-452">Property</span></span>|<span data-ttu-id="e23f7-453">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e23f7-453">Example</span></span>|
|:------|:------|
| <span data-ttu-id="e23f7-454">background-color</span><span class="sxs-lookup"><span data-stu-id="e23f7-454">background-color</span></span> | <span data-ttu-id="e23f7-455">`style="background-color:#66cc66"` (Standardwert ist Weiß)</span><span class="sxs-lookup"><span data-stu-id="e23f7-455">style="background-color:#66cc66"`style="background-color:#66cc66"` (defaults to  white)</span></span><br /><span data-ttu-id="e23f7-456">Das hexadezimale Format und benannte Farben werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e23f7-456">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="e23f7-457">color</span><span class="sxs-lookup"><span data-stu-id="e23f7-457">color</span></span> | <span data-ttu-id="e23f7-458">`style="color:#ffffff"` (Standardwert ist Schwarz)</span><span class="sxs-lookup"><span data-stu-id="e23f7-458">style="color:#ffffff"`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="e23f7-459">font-family</span><span class="sxs-lookup"><span data-stu-id="e23f7-459">font-family</span></span> | <span data-ttu-id="e23f7-460">`style="font-family:Courier"` (Standardwert ist Calibri)</span><span class="sxs-lookup"><span data-stu-id="e23f7-460">style="font-family:Courier"`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="e23f7-461">font-size</span><span class="sxs-lookup"><span data-stu-id="e23f7-461">font-size</span></span> | <span data-ttu-id="e23f7-462">`style="font-size:10pt"` (Standardwert ist 11pt)</span><span class="sxs-lookup"><span data-stu-id="e23f7-462">style="font-size:10pt"`style="font-size:10pt"` (defaults to 11pt)</span></span><br /><span data-ttu-id="e23f7-463">Die APIs akzeptieren den Schriftgrad in *pt* oder *px*, *px* wird jedoch zu *pt* konvertiert.</span><span class="sxs-lookup"><span data-stu-id="e23f7-463">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="e23f7-464">Dezimalwerte werden auf die nächste n.0pt oder n.5pt gerundet.</span><span class="sxs-lookup"><span data-stu-id="e23f7-464">The onnvshort API accepts font size in pt or px, but converts px to pt. Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="e23f7-465">font-style</span><span class="sxs-lookup"><span data-stu-id="e23f7-465">font-style</span></span> | <span data-ttu-id="e23f7-466">`style="font-style:italic"`(nur normal oder kursiv)</span><span class="sxs-lookup"><span data-stu-id="e23f7-466">style="font-style:italic"`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="e23f7-467">font-weight</span><span class="sxs-lookup"><span data-stu-id="e23f7-467">font-weight</span></span> | <span data-ttu-id="e23f7-468">`style="font-weight:bold"`(nur normal oder fett)</span><span class="sxs-lookup"><span data-stu-id="e23f7-468">style="font-weight:bold"`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="e23f7-469">strike-through</span><span class="sxs-lookup"><span data-stu-id="e23f7-469">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="e23f7-470">text-align</span><span class="sxs-lookup"><span data-stu-id="e23f7-470">text-align</span></span> | <span data-ttu-id="e23f7-471">`style="text-align:center"`(nur für Blockelementen)</span><span class="sxs-lookup"><span data-stu-id="e23f7-471">style="text-align:center"`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="e23f7-472">text-decoration</span><span class="sxs-lookup"><span data-stu-id="e23f7-472">text-decoration</span></span> | <span data-ttu-id="e23f7-473">`style="text-decoration:underline"`(nur keine oder unterstrichen)</span><span class="sxs-lookup"><span data-stu-id="e23f7-473">style="text-decoration:underline"`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="e23f7-474">Die folgenden Inlinezeichenformate werden ebenfalls unterstützt:</span><span class="sxs-lookup"><span data-stu-id="e23f7-474">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="e23f7-475">&lt;b&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-475">&lt;B</span></span></td>
<td id="simplecell"><span data-ttu-id="e23f7-476">&lt;i&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-476">&lt;I</span></span></td>
<td id="simplecell"><span data-ttu-id="e23f7-477">&lt;u&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-477">&lt;U</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="e23f7-478">&lt;em&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-478">EM</span></span></td>
<td id="simplecell"><span data-ttu-id="e23f7-479">&lt;strong&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-479">Strong.</span></span></td>
<td id="simplecell"><span data-ttu-id="e23f7-480">&lt;strike&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-480">&lt;strike&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="e23f7-481">&lt;sup&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-481">Scr sup.</span></span></td>
<td id="simplecell"><span data-ttu-id="e23f7-482">&lt;sub&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-482">&lt;Sub&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="e23f7-483">&lt;del&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-483">&lt;del&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="e23f7-484">&lt;cite&gt;</span><span class="sxs-lookup"><span data-stu-id="e23f7-484">&lt;cite&gt;</span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="e23f7-485">Beispiel für Eingabe- und Ausgabe-HTML</span><span class="sxs-lookup"><span data-stu-id="e23f7-485">Input and output HTML example</span></span>
<span data-ttu-id="e23f7-486">Die folgende Abbildung zeigt eine einfache Seite, die mit der Microsoft Graph erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e23f7-486">The following image shows a simple page that was created with the onnvshort API.</span></span>

![Bild einer OneNote-Seite mit Lernnotizen aus Inhalten von Wikipedia](images/onenote-sample-image.png)

<span data-ttu-id="e23f7-488">Dabei handelt es sich um die Eingabe-HTML, die im Nachrichtentextkörper gesendet wurde, um die Seite zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e23f7-488">This is the input HTML that was sent in the request body to create the page.</span></span>

```html
<html lang="en-US">
    <head>
        <title>Sample Study Notes</title>
        <meta name="created" content="2015-01-01T01:01"/>
    </head>
    <body>
        <h1>Aurora Borealis</h1>
        <p>Dancing lights in the sky. Also called <i>Northern Lights</i>. Caused by solar radiation.</p>
        <br />
        <p><b>Intersting facts</b></p>
        <table>
            <tr>
                <td>Neil Armstrong</td>
                <td>Commander</td>
            </tr>
            <tr>
                <td>Buzz Aldrin</td>
                <td>LM Pilot</td>
            </tr>
            <tr>
                <td>Michael Collins</td>
                <td>Command Module Pilot</td>
            </tr>
        </table>
        <img alt="Apollo 11 commemorative stamp." src="http://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<span data-ttu-id="e23f7-489">Im Folgenden sehen Sie die Ausgabe-HTML, die die Microsoft Graph zurückgibt, wenn Sie [den Seiteninhalt abrufen](../api-reference/v1.0/api/page_get.md).</span><span class="sxs-lookup"><span data-stu-id="e23f7-489">This is the output HTML that the onnvshort API returns when you get the page content.</span></span>

><span data-ttu-id="e23f7-490">**Hinweis:** Wenn Sie [eine Seite erstellen](../api-reference/v1.0/api/section_post_pages.md) oder [die Metadaten einer Seite abrufen](../api-reference/v1.0/api/page_get.md), gibt die API die *Inhalte*-Endpunkt-URL der Seite in der **contentUrl**Eigenschaft zurück.</span><span class="sxs-lookup"><span data-stu-id="e23f7-490">**Note:** When you [create a page](../api-reference/v1.0/api/section_post_pages.md) or [get page metadata](../api-reference/v1.0/api/page_get.md), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Sample Study Notes</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">American History 101: Moon Landing</h1>
            <p>First moon landing - July 20, 1969 with Apollo 11 (Eagle)</p>
            <br />
            <p><span style="font-weight:bold">Apollo 11 Astronauts</span></p>
            <table style="border:0px">
                <tr>
                    <td style="border:0px">Neil Armstrong</td>
                    <td style="border:0px">Commander</td>
                </tr>
                <tr>
                    <td style="border:0px">Buzz Aldrin</td>
                    <td style="border:0px">LM Pilot</td>
                </tr>
                <tr>
                    <td style="border:0px">Michael Collins</td>
                    <td style="border:0px">Command Module Pilot</td>
                </tr>
            </table>
            <br />
            <img alt="Apollo 11 commemorative stamp." width="400" height="248" src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value"
                 data-src-type="image/jpeg" data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value" data-fullres-src-type="image/jpeg" />
            <p>References:</p>
            <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="e23f7-491">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e23f7-491">See also</span></span>

- [<span data-ttu-id="e23f7-492">Abrufen von OneNote-Inhalt und -Struktur</span><span class="sxs-lookup"><span data-stu-id="e23f7-492">Get OneNote content and structure</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="e23f7-493">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="e23f7-493">Create OneNote pages</span></span>](../api-reference/v1.0/api/section_post_pages.md)
- [<span data-ttu-id="e23f7-494">Aktualisieren mit OneNote-Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="e23f7-494">Update page content</span></span>](../api-reference/v1.0/api/page_update.md)
- [<span data-ttu-id="e23f7-495">Hinzufügen von Bildern und Dateien</span><span class="sxs-lookup"><span data-stu-id="e23f7-495">Add images and files</span></span>](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)

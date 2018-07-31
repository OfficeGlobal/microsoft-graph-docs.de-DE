
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="048d8-101">Erstellen von absolut positionierten Elementen auf OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="048d8-101">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="048d8-102">Das „body“-Element einer OneNote-Seite kann mehrere direkt untergeordnete Elemente des Typs `div`, `img` oder `object` enthalten, die unabhängig voneinander auf der Seite positioniert werden können.</span><span class="sxs-lookup"><span data-stu-id="048d8-102">The body of a OneNote page can contain multiple direct `div`, `img`, and `object` child elements that can be positioned independently on the page.</span></span>

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="048d8-103">Attribute und Positionierungsverhalten</span><span class="sxs-lookup"><span data-stu-id="048d8-103">Attributes and positioning behavior</span></span>

<span data-ttu-id="048d8-104">Mithilfe der Attribute `data-absolute-enabled` und [`style`](#supported-css-style-attributes) können Sie absolut positionierte Elemente auf einer Seite erstellen. Dabei gilt:</span><span class="sxs-lookup"><span data-stu-id="048d8-104">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="048d8-105">Das „body“-Element muss `data-absolute-enabled="true"` enthalten.</span><span class="sxs-lookup"><span data-stu-id="048d8-105">The body element must specify `data-absolute-enabled="true"`.</span></span> <span data-ttu-id="048d8-106">Fehlt diese Eigenschaft oder ist sie auf `false` gesetzt, werden alle „body“-Inhalte in einem absolut positionierten „div“-Element `_default` gerendert, das von der API erstellt wird. Dabei werden alle Positionseinstellungen ignoriert.</span><span class="sxs-lookup"><span data-stu-id="048d8-106">If omitted or set to `false`, all body content is rendered inside a `_default` absolute positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="048d8-107">Nur Elemente des Typs `div`, `img` oder `object` können absolut positionierte Elemente sein.</span><span class="sxs-lookup"><span data-stu-id="048d8-107">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="048d8-108">Absolut positionierte Elemente müssen `style="position:absolute"` enthalten.</span><span class="sxs-lookup"><span data-stu-id="048d8-108">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="048d8-109">Absolut positionierte Elemente müssen direkt untergeordnete Elemente des Elements `body` sein.</span><span class="sxs-lookup"><span data-stu-id="048d8-109">Absolute positioned elements must be direct children of the `body` element.</span></span> <span data-ttu-id="048d8-110">Alle direkt untergeordneten Elemente des „body“-Elements, die keine absolut positionierten Elemente des Typs `div`, `img` oder `object` sind, werden als statische Inhalte innerhalb des absolut positionierten „div“-Elements `_default` gerendert.</span><span class="sxs-lookup"><span data-stu-id="048d8-110">Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="048d8-111">Absolut positionierte Elemente werden an den festgelegten oberen und linken Koordinaten relativ zur Startposition 0:0 in der linken oberen Ecke der Seite positioniert, über dem Titelbereich.</span><span class="sxs-lookup"><span data-stu-id="048d8-111">Absolute positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the top, left corner of the page above the title area.</span></span>

- <span data-ttu-id="048d8-112">Wenn für ein absolut positioniertes Element die obere Koordinate oder die linke Koordinate nicht angegeben ist, wird die fehlende Koordinate auf ihren jeweiligen Standardwert gesetzt: `top:120px` oder `left:48px`.</span><span class="sxs-lookup"><span data-stu-id="048d8-112">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`.</span></span> <span data-ttu-id="048d8-113">Diese Standardkoordinaten legen eine Position direkt unter dem Titelbereich fest.</span><span class="sxs-lookup"><span data-stu-id="048d8-113">These default coordinates specify a position just below the title area.</span></span> <span data-ttu-id="048d8-114">Das Weglassen von Koordinaten kann dazu führen, dass Elemente übereinander gestapelt werden.</span><span class="sxs-lookup"><span data-stu-id="048d8-114">Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="048d8-115">Absolut positionierte Elemente können weder geschachtelt werden noch positionierte Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="048d8-115">Absolute positioned elements cannot be nested or contain positioned elements.</span></span> <span data-ttu-id="048d8-116">Die API ignoriert alle für geschachtelte Elemente innerhalb eines absolut positionierten „div“-Elements angegebenen Positionseinstellungen, rendert die geschachtelten Inhalte innerhalb des absolut positionierten übergeordneten „div“-Elements und gibt eine Warnung in der Eigenschaft **api.diagnostics** in der Antwort zurück.</span><span class="sxs-lookup"><span data-stu-id="048d8-116">The API ignores any position settings specified on nested elements inside an absolute positioned div, renders the nested content inside the absolute positioned parent div, and returns a warning in the **api.diagnostics** property in the response.</span></span>


### <a name="example"></a><span data-ttu-id="048d8-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="048d8-117">Example</span></span>

<span data-ttu-id="048d8-118">Das folgende Beispiel enthält ein direkt untergeordnetes Element des Typs `p`, ein absolut positioniertes „div“-Element und ein nicht absolut positioniertes „div“-Element.</span><span class="sxs-lookup"><span data-stu-id="048d8-118">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

#### <a name="input-html"></a><span data-ttu-id="048d8-119">Eingabe-HTML</span><span class="sxs-lookup"><span data-stu-id="048d8-119">Input HTML</span></span>  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

<span data-ttu-id="048d8-120">Die API rendert das nicht absolut positionierte „div“-Element im „div“-Element „default“.</span><span class="sxs-lookup"><span data-stu-id="048d8-120">The API renders the non-absolute positioned div in the default div.</span></span> <span data-ttu-id="048d8-121">Beachten Sie: Die geschachtelten Tags des Typs `<div>` werden verworfen, da sie keine semantischen Informationen definieren (z. B. `data-id`).</span><span class="sxs-lookup"><span data-stu-id="048d8-121">Note that the nested  `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

#### <a name="output-html"></a><span data-ttu-id="048d8-122">Ausgabe-HTML</span><span class="sxs-lookup"><span data-stu-id="048d8-122">Output HTML</span></span> 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

### <a name="example"></a><span data-ttu-id="048d8-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="048d8-123">Example</span></span>

<span data-ttu-id="048d8-124">Das folgende Beispiel erstellt eine Seite, die ein einziges absolut positioniertes „div“-Element und ein einziges absolut positioniertes Bild enthält.</span><span class="sxs-lookup"><span data-stu-id="048d8-124">The following example creates a page that contains one absolute positioned div and one absolute positioned image.</span></span>


#### <a name="input-html"></a><span data-ttu-id="048d8-125">Eingabe-HTML</span><span class="sxs-lookup"><span data-stu-id="048d8-125">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="http://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="http://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="048d8-126">Die OneNote-API wertet den Eingabe-HTML-Code aus und behält alle semantischen Inhalte sowie alle strukturellen Informationen bei, die von OneNote unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="048d8-126">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote.</span></span> <span data-ttu-id="048d8-127">Die daraus resultierende Seite wird wie in der Abbildung unten gerendert (ohne die sichtbaren Rahmen um das „div“-Element und das Bild).</span><span class="sxs-lookup"><span data-stu-id="048d8-127">The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![Resultierende Seite mit absolut positioniertem „div“-Element und absolut positioniertem Bild](images/abs-pos.PNG)

<span data-ttu-id="048d8-129">Beachten Sie die Änderungen am nicht berücksichtigten, geschachtelten „div“-Element aus dem Eingabe-HTML-Code.</span><span class="sxs-lookup"><span data-stu-id="048d8-129">Notice the changes to the non-contributing, nested div from the input HTML.</span></span> <span data-ttu-id="048d8-130">Die API behält die Inhalte des „div“-Elements bei, verwirft jedoch die Tags des Typs `<div>`, weil das „div“-Element keine semantischen Informationen definiert (z. B. `data-id`).</span><span class="sxs-lookup"><span data-stu-id="048d8-130">The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="048d8-131">Weitere Informationen dazu, wie die OneNote-API Eingabe-HTML und Ausgabe-HTML verarbeitet, finden Sie unter [Eingabe- und Ausgabe-HTML auf OneNote-Seiten](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="048d8-131">For more information about how the OneNote API handles input and output HTML, see [Input and output HTML for OneNote pages](onenote_input_output_html.md).</span></span>

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a><span data-ttu-id="048d8-132">Unterstützte CSS-Formatattribute</span><span class="sxs-lookup"><span data-stu-id="048d8-132">Supported CSS style attributes</span></span>

<span data-ttu-id="048d8-133">Für alle absolut positionierten Elemente können eine obere Position und eine linke Position angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="048d8-133">All absolute positioned elements can specify top and left positions.</span></span> <span data-ttu-id="048d8-134">Für „div“-Elemente und Bilder lässt sich die Breite, für Bilder zusätzlich auch die Höhe festlegen.</span><span class="sxs-lookup"><span data-stu-id="048d8-134">Divs and images can specify width, and images can also specify height.</span></span> <span data-ttu-id="048d8-135">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="048d8-135">For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="048d8-136">Attribut</span><span class="sxs-lookup"><span data-stu-id="048d8-136">Attribute</span></span> | <span data-ttu-id="048d8-137">Unterstütztes Element</span><span class="sxs-lookup"><span data-stu-id="048d8-137">Supported element</span></span> | <span data-ttu-id="048d8-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="048d8-138">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="048d8-139">top</span><span class="sxs-lookup"><span data-stu-id="048d8-139">top</span></span> | <span data-ttu-id="048d8-140">div, img, object</span><span class="sxs-lookup"><span data-stu-id="048d8-140">div, img, object</span></span> | <span data-ttu-id="048d8-141">Y-Koordinate des oberen Rands des Elements, anzugeben ausschließlich in Pixel.</span><span class="sxs-lookup"><span data-stu-id="048d8-141">The y-axis coordinate of the element's top border, in pixels only.</span></span> <span data-ttu-id="048d8-142">Der Standardwert ist 120 Pixel.</span><span class="sxs-lookup"><span data-stu-id="048d8-142">Default is 120 pixels.</span></span><br/><br/><span data-ttu-id="048d8-143">Beispiel: `top:140px`</span><span class="sxs-lookup"><span data-stu-id="048d8-143">Example: `top:140px`</span></span> |  
| <span data-ttu-id="048d8-144">left</span><span class="sxs-lookup"><span data-stu-id="048d8-144">left</span></span> |  <span data-ttu-id="048d8-145">div, img, object</span><span class="sxs-lookup"><span data-stu-id="048d8-145">div, img, object</span></span>  | <span data-ttu-id="048d8-146">X-Koordinate des linken Rands des Elements, anzugeben ausschließlich in Pixel</span><span class="sxs-lookup"><span data-stu-id="048d8-146">The x-axis coordinate of the element's left border, in pixels only.</span></span> <span data-ttu-id="048d8-147">Der Standardwert ist 48 Pixel.</span><span class="sxs-lookup"><span data-stu-id="048d8-147">Default is 48 pixels.</span></span><br/><br/><span data-ttu-id="048d8-148">Beispiel: `left:95px`</span><span class="sxs-lookup"><span data-stu-id="048d8-148">Example: `left:95px`</span></span> |  
| <span data-ttu-id="048d8-149">width</span><span class="sxs-lookup"><span data-stu-id="048d8-149">width</span></span> |  <span data-ttu-id="048d8-150">div, img</span><span class="sxs-lookup"><span data-stu-id="048d8-150">div, img</span></span>  | <span data-ttu-id="048d8-151">Die Breite des Elements, anzugeben ausschließlich in Pixel.</span><span class="sxs-lookup"><span data-stu-id="048d8-151">The width of the element, in pixels only.</span></span><br/><br/><span data-ttu-id="048d8-152">Beispiel: `width:480px`</span><span class="sxs-lookup"><span data-stu-id="048d8-152">Example: `width:480px`</span></span> |  
| <span data-ttu-id="048d8-153">height</span><span class="sxs-lookup"><span data-stu-id="048d8-153">height</span></span> | <span data-ttu-id="048d8-154">img</span><span class="sxs-lookup"><span data-stu-id="048d8-154">img</span></span> | <span data-ttu-id="048d8-155">Die Höhe des Elements, anzugeben ausschließlich in Pixel.</span><span class="sxs-lookup"><span data-stu-id="048d8-155">The height of the element, in pixels only.</span></span> <span data-ttu-id="048d8-156">Die Höhe von „div“-Elementen wird zur Laufzeit berechnet; angegebene Höhenwerte werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="048d8-156">For divs, height is calculated at runtime and any specified height value is ignored.</span></span><br/><br/><span data-ttu-id="048d8-157">Beispiel: `height:665px`</span><span class="sxs-lookup"><span data-stu-id="048d8-157">Example: `height:665px`</span></span> |  
 
<span data-ttu-id="048d8-158">Andere Positionsattribute, beispielsweise `z-index`, werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="048d8-158">Other position attributes, such as `z-index`, are ignored.</span></span> <span data-ttu-id="048d8-159">Für absolut positionierte Bilder können Sie entweder das Attribut `data-render-src` oder das Attribut `src` verwenden.</span><span class="sxs-lookup"><span data-stu-id="048d8-159">Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="048d8-160">Informationen in der Antwort</span><span class="sxs-lookup"><span data-stu-id="048d8-160">Response information</span></span>

<span data-ttu-id="048d8-161">Die OneNote-API gibt in der Antwort die nachfolgenden Informationen zurück.</span><span class="sxs-lookup"><span data-stu-id="048d8-161">The OneNote API returns the following information in the response.</span></span>

| <span data-ttu-id="048d8-162">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="048d8-162">Response data</span></span> | <span data-ttu-id="048d8-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="048d8-163">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="048d8-164">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="048d8-164">Success code</span></span> | <span data-ttu-id="048d8-165">HTTP-Statuscode 201 bei erfolgreich ausgeführter POST-Anforderung, HTTP-Statuscode 204 bei erfolgreich ausgeführter PATCH-Anforderung</span><span class="sxs-lookup"><span data-stu-id="048d8-165">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="048d8-166">Fehler</span><span class="sxs-lookup"><span data-stu-id="048d8-166">Errors</span></span> | <span data-ttu-id="048d8-167">Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote_error_codes.md).</span><span class="sxs-lookup"><span data-stu-id="048d8-167">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="048d8-168">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="048d8-168">Permissions</span></span>

<span data-ttu-id="048d8-169">Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="048d8-169">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="048d8-170">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="048d8-170">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="048d8-171">Berechtigungen für BEITRAG-Seiten</span><span class="sxs-lookup"><span data-stu-id="048d8-171">Permissions for POST pages</span></span> 

- <span data-ttu-id="048d8-172">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="048d8-172">Notes.Create</span></span>
- <span data-ttu-id="048d8-173">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="048d8-173">Notes.ReadWrite</span></span>
- <span data-ttu-id="048d8-174">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="048d8-174">Notes.ReadWrite.All</span></span>  


#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="048d8-175">Berechtigungen für PATCH-Seiten</span><span class="sxs-lookup"><span data-stu-id="048d8-175">Permissions for PATCH pages</span></span> 

- <span data-ttu-id="048d8-176">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="048d8-176">Notes.ReadWrite</span></span>
- <span data-ttu-id="048d8-177">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="048d8-177">Notes.ReadWrite.All</span></span>

<span data-ttu-id="048d8-178">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie im Artikel zum Thema [OneNote-Berechtigungsbereiche](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="048d8-178">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="048d8-179">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="048d8-179">See also</span></span>

- [<span data-ttu-id="048d8-180">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="048d8-180">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="048d8-181">Aktualisieren der Inhalte von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="048d8-181">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="048d8-182">Integrieren mit OneNote</span><span class="sxs-lookup"><span data-stu-id="048d8-182">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="048d8-183">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="048d8-183">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="048d8-184">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="048d8-184">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="048d8-185">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="048d8-185">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  


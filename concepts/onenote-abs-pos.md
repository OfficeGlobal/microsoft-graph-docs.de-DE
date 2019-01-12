---
title: Erstellen von absolut positionierten Elementen auf OneNote-Seiten
description: Das „body“-Element einer OneNote-Seite kann mehrere direkt untergeordnete Elemente des Typs `div`, `img` oder `object` enthalten, die unabhängig voneinander auf der Seite positioniert werden können.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 9630741091be52de8791f560a13b225ccce2e218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981168"
---
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="c1e7d-103">Erstellen von absolut positionierten Elementen auf OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="c1e7d-103">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="c1e7d-104">Das „body“-Element einer OneNote-Seite kann mehrere direkt untergeordnete Elemente des Typs `div`, `img` oder `object` enthalten, die unabhängig voneinander auf der Seite positioniert werden können.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-104">The body of a OneNote page can contain multiple direct `div`, `img`, and `object` child elements that can be positioned independently on the page.</span></span>

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="c1e7d-105">Attribute und Positionierungsverhalten</span><span class="sxs-lookup"><span data-stu-id="c1e7d-105">Attributes and positioning behavior</span></span>

<span data-ttu-id="c1e7d-106">Mithilfe der Attribute `data-absolute-enabled` und [`style`](#supported-css-style-attributes) können Sie absolut positionierte Elemente auf einer Seite erstellen. Dabei gilt:</span><span class="sxs-lookup"><span data-stu-id="c1e7d-106">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="c1e7d-107">Das „body“-Element muss `data-absolute-enabled="true"` enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-107">The body element must specify `data-absolute-enabled="true"`.</span></span> <span data-ttu-id="c1e7d-108">Fehlt diese Eigenschaft oder ist sie auf `false` gesetzt, werden alle „body“-Inhalte in einem absolut positionierten „div“-Element `_default` gerendert, das von der API erstellt wird. Dabei werden alle Positionseinstellungen ignoriert.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-108">If omitted or set to `false`, all body content is rendered inside a `_default` absolute positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="c1e7d-109">Nur Elemente des Typs `div`, `img` oder `object` können absolut positionierte Elemente sein.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-109">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="c1e7d-110">Absolut positionierte Elemente müssen `style="position:absolute"` enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-110">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="c1e7d-111">Absolut positionierte Elemente müssen direkt untergeordnete Elemente des Elements `body` sein.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-111">Absolute positioned elements must be direct children of the `body` element.</span></span> <span data-ttu-id="c1e7d-112">Alle direkt untergeordneten Elemente des „body“-Elements, die keine absolut positionierten Elemente des Typs `div`, `img` oder `object` sind, werden als statische Inhalte innerhalb des absolut positionierten „div“-Elements `_default` gerendert.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-112">Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="c1e7d-113">Absolut positionierte Elemente werden an den festgelegten oberen und linken Koordinaten relativ zur Startposition 0:0 in der linken oberen Ecke der Seite positioniert, über dem Titelbereich.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-113">Absolute positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the top, left corner of the page above the title area.</span></span>

- <span data-ttu-id="c1e7d-114">Wenn für ein absolut positioniertes Element die obere Koordinate oder die linke Koordinate nicht angegeben ist, wird die fehlende Koordinate auf ihren jeweiligen Standardwert gesetzt: `top:120px` oder `left:48px`.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-114">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`.</span></span> <span data-ttu-id="c1e7d-115">Diese Standardkoordinaten legen eine Position direkt unter dem Titelbereich fest.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-115">These default coordinates specify a position just below the title area.</span></span> <span data-ttu-id="c1e7d-116">Das Weglassen von Koordinaten kann dazu führen, dass Elemente übereinander gestapelt werden.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-116">Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="c1e7d-117">Absolut positionierte Elemente können weder geschachtelt werden noch positionierte Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-117">Absolute positioned elements cannot be nested or contain positioned elements.</span></span> <span data-ttu-id="c1e7d-118">Die API ignoriert alle für geschachtelte Elemente innerhalb eines absolut positionierten „div“-Elements angegebenen Positionseinstellungen, rendert die geschachtelten Inhalte innerhalb des absolut positionierten übergeordneten „div“-Elements und gibt eine Warnung in der Eigenschaft **api.diagnostics** in der Antwort zurück.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-118">The API ignores any position settings specified on nested elements inside an absolute positioned div, renders the nested content inside the absolute positioned parent div, and returns a warning in the **api.diagnostics** property in the response.</span></span>


### <a name="example"></a><span data-ttu-id="c1e7d-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1e7d-119">Example</span></span>

<span data-ttu-id="c1e7d-120">Das folgende Beispiel enthält ein direkt untergeordnetes Element des Typs `p`, ein absolut positioniertes „div“-Element und ein nicht absolut positioniertes „div“-Element.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-120">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

#### <a name="input-html"></a><span data-ttu-id="c1e7d-121">Eingabe-HTML</span><span class="sxs-lookup"><span data-stu-id="c1e7d-121">Input HTML</span></span>  

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

<span data-ttu-id="c1e7d-122">Die API rendert das nicht absolut positionierte „div“-Element im „div“-Element „default“.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-122">The API renders the non-absolute positioned div in the default div.</span></span> <span data-ttu-id="c1e7d-123">Beachten Sie: Die geschachtelten Tags des Typs `<div>` werden verworfen, da sie keine semantischen Informationen definieren (z. B. `data-id`).</span><span class="sxs-lookup"><span data-stu-id="c1e7d-123">Note that the nested `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

#### <a name="output-html"></a><span data-ttu-id="c1e7d-124">Ausgabe-HTML</span><span class="sxs-lookup"><span data-stu-id="c1e7d-124">Output HTML</span></span> 

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

### <a name="example"></a><span data-ttu-id="c1e7d-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1e7d-125">Example</span></span>

<span data-ttu-id="c1e7d-126">Das folgende Beispiel erstellt eine Seite, die ein einziges absolut positioniertes „div“-Element und ein einziges absolut positioniertes Bild enthält.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-126">The following example creates a page that contains one absolute positioned div and one absolute positioned image.</span></span>


#### <a name="input-html"></a><span data-ttu-id="c1e7d-127">Eingabe-HTML</span><span class="sxs-lookup"><span data-stu-id="c1e7d-127">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="c1e7d-128">Die OneNote-API wertet den Eingabe-HTML-Code aus und behält alle semantischen Inhalte sowie alle strukturellen Informationen bei, die von OneNote unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-128">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote.</span></span> <span data-ttu-id="c1e7d-129">Die daraus resultierende Seite wird wie in der Abbildung unten gerendert (ohne die sichtbaren Rahmen um das „div“-Element und das Bild).</span><span class="sxs-lookup"><span data-stu-id="c1e7d-129">The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![Resultierende Seite mit absolut positioniertem „div“-Element und absolut positioniertem Bild](images/abs-pos.png)

<span data-ttu-id="c1e7d-131">Beachten Sie die Änderungen am nicht berücksichtigten, geschachtelten „div“-Element aus dem Eingabe-HTML-Code.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-131">Notice the changes to the non-contributing, nested div from the input HTML.</span></span> <span data-ttu-id="c1e7d-132">Die API behält die Inhalte des „div“-Elements bei, verwirft jedoch die Tags des Typs `<div>`, weil das „div“-Element keine semantischen Informationen definiert (z. B. `data-id`).</span><span class="sxs-lookup"><span data-stu-id="c1e7d-132">The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="c1e7d-133">Weitere Informationen dazu, wie die OneNote-API Eingabe-HTML und Ausgabe-HTML verarbeitet, finden Sie unter [Eingabe- und Ausgabe-HTML auf OneNote-Seiten](onenote-input-output-html.md).</span><span class="sxs-lookup"><span data-stu-id="c1e7d-133">For more information about how the OneNote API handles input and output HTML, see [Input and output HTML for OneNote pages](onenote-input-output-html.md).</span></span>

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a><span data-ttu-id="c1e7d-134">Unterstützte CSS-Formatattribute</span><span class="sxs-lookup"><span data-stu-id="c1e7d-134">Supported CSS style attributes</span></span>

<span data-ttu-id="c1e7d-135">Für alle absolut positionierten Elemente können eine obere Position und eine linke Position angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-135">All absolute positioned elements can specify top and left positions.</span></span> <span data-ttu-id="c1e7d-136">Für „div“-Elemente und Bilder lässt sich die Breite, für Bilder zusätzlich auch die Höhe festlegen.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-136">Divs and images can specify width, and images can also specify height.</span></span> <span data-ttu-id="c1e7d-137">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c1e7d-137">For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="c1e7d-138">Attribut</span><span class="sxs-lookup"><span data-stu-id="c1e7d-138">Attribute</span></span> | <span data-ttu-id="c1e7d-139">Unterstütztes Element</span><span class="sxs-lookup"><span data-stu-id="c1e7d-139">Supported element</span></span> | <span data-ttu-id="c1e7d-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1e7d-140">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="c1e7d-141">top</span><span class="sxs-lookup"><span data-stu-id="c1e7d-141">top</span></span> | <span data-ttu-id="c1e7d-142">div, img, object</span><span class="sxs-lookup"><span data-stu-id="c1e7d-142">div, img, object</span></span> | <span data-ttu-id="c1e7d-143">Y-Koordinate des oberen Rands des Elements, anzugeben ausschließlich in Pixel.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-143">The y-axis coordinate of the element's top border, in pixels only.</span></span> <span data-ttu-id="c1e7d-144">Der Standardwert ist 120 Pixel.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-144">Default is 120 pixels.</span></span><br/><br/><span data-ttu-id="c1e7d-145">Beispiel: `top:140px`</span><span class="sxs-lookup"><span data-stu-id="c1e7d-145">Example: `top:140px`</span></span> |  
| <span data-ttu-id="c1e7d-146">left</span><span class="sxs-lookup"><span data-stu-id="c1e7d-146">left</span></span> |  <span data-ttu-id="c1e7d-147">div, img, object</span><span class="sxs-lookup"><span data-stu-id="c1e7d-147">div, img, object</span></span>  | <span data-ttu-id="c1e7d-148">X-Koordinate des linken Rands des Elements, anzugeben ausschließlich in Pixel</span><span class="sxs-lookup"><span data-stu-id="c1e7d-148">The x-axis coordinate of the element's left border, in pixels only.</span></span> <span data-ttu-id="c1e7d-149">Der Standardwert ist 48 Pixel.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-149">Default is 48 pixels.</span></span><br/><br/><span data-ttu-id="c1e7d-150">Beispiel: `left:95px`</span><span class="sxs-lookup"><span data-stu-id="c1e7d-150">Example: `left:95px`</span></span> |  
| <span data-ttu-id="c1e7d-151">width</span><span class="sxs-lookup"><span data-stu-id="c1e7d-151">width</span></span> |  <span data-ttu-id="c1e7d-152">div, img</span><span class="sxs-lookup"><span data-stu-id="c1e7d-152">div, img</span></span>  | <span data-ttu-id="c1e7d-153">Die Breite des Elements, anzugeben ausschließlich in Pixel.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-153">The width of the element, in pixels only.</span></span><br/><br/><span data-ttu-id="c1e7d-154">Beispiel: `width:480px`</span><span class="sxs-lookup"><span data-stu-id="c1e7d-154">Example: `width:480px`</span></span> |  
| <span data-ttu-id="c1e7d-155">height</span><span class="sxs-lookup"><span data-stu-id="c1e7d-155">height</span></span> | <span data-ttu-id="c1e7d-156">img</span><span class="sxs-lookup"><span data-stu-id="c1e7d-156">img</span></span> | <span data-ttu-id="c1e7d-157">Die Höhe des Elements, anzugeben ausschließlich in Pixel.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-157">The height of the element, in pixels only.</span></span> <span data-ttu-id="c1e7d-158">Die Höhe von „div“-Elementen wird zur Laufzeit berechnet; angegebene Höhenwerte werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-158">For divs, height is calculated at runtime and any specified height value is ignored.</span></span><br/><br/><span data-ttu-id="c1e7d-159">Beispiel: `height:665px`</span><span class="sxs-lookup"><span data-stu-id="c1e7d-159">Example: `height:665px`</span></span> |  
 
<span data-ttu-id="c1e7d-160">Andere Positionsattribute, beispielsweise `z-index`, werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-160">Other position attributes, such as `z-index`, are ignored.</span></span> <span data-ttu-id="c1e7d-161">Für absolut positionierte Bilder können Sie entweder das Attribut `data-render-src` oder das Attribut `src` verwenden.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-161">Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="c1e7d-162">Informationen in der Antwort</span><span class="sxs-lookup"><span data-stu-id="c1e7d-162">Response information</span></span>

<span data-ttu-id="c1e7d-163">Die OneNote-API gibt in der Antwort die nachfolgenden Informationen zurück.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-163">The OneNote API returns the following information in the response.</span></span>

| <span data-ttu-id="c1e7d-164">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="c1e7d-164">Response data</span></span> | <span data-ttu-id="c1e7d-165">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1e7d-165">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="c1e7d-166">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="c1e7d-166">Success code</span></span> | <span data-ttu-id="c1e7d-167">HTTP-Statuscode 201 bei erfolgreich ausgeführter POST-Anforderung, HTTP-Statuscode 204 bei erfolgreich ausgeführter PATCH-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1e7d-167">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="c1e7d-168">Fehler</span><span class="sxs-lookup"><span data-stu-id="c1e7d-168">Errors</span></span> | <span data-ttu-id="c1e7d-169">Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="c1e7d-169">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="c1e7d-170">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1e7d-170">Permissions</span></span>

<span data-ttu-id="c1e7d-171">Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-171">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="c1e7d-172">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="c1e7d-172">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="c1e7d-173">Berechtigungen für BEITRAG-Seiten</span><span class="sxs-lookup"><span data-stu-id="c1e7d-173">Permissions for POST pages</span></span> 

- <span data-ttu-id="c1e7d-174">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="c1e7d-174">Notes.Create</span></span>
- <span data-ttu-id="c1e7d-175">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1e7d-175">Notes.ReadWrite</span></span>
- <span data-ttu-id="c1e7d-176">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1e7d-176">Notes.ReadWrite.All</span></span>  


#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="c1e7d-177">Berechtigungen für PATCH-Seiten</span><span class="sxs-lookup"><span data-stu-id="c1e7d-177">Permissions for PATCH pages</span></span> 

- <span data-ttu-id="c1e7d-178">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1e7d-178">Notes.ReadWrite</span></span>
- <span data-ttu-id="c1e7d-179">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1e7d-179">Notes.ReadWrite.All</span></span>

<span data-ttu-id="c1e7d-180">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie unter [OneNote-Berechtigungsbereiche](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="c1e7d-180">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="c1e7d-181">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="c1e7d-181">See also</span></span>

- [<span data-ttu-id="c1e7d-182">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="c1e7d-182">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="c1e7d-183">Aktualisieren der Inhalte von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="c1e7d-183">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="c1e7d-184">Integrieren mit OneNote</span><span class="sxs-lookup"><span data-stu-id="c1e7d-184">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="c1e7d-185">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="c1e7d-185">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="c1e7d-186">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="c1e7d-186">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="c1e7d-187">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="c1e7d-187">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  


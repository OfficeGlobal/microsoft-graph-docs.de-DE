# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a><span data-ttu-id="789aa-101">Verwenden von div-Tags der OneNote-API zum Extrahieren von Daten aus Erfassungen</span><span class="sxs-lookup"><span data-stu-id="789aa-101">Use OneNote API div tags to extract data from captures</span></span> 

<span data-ttu-id="789aa-102">*__Gilt für:__ Privatanwender-Notizbücher auf OneDrive | Enterprise-Notizbücher auf Office 365*</span><span class="sxs-lookup"><span data-stu-id="789aa-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="789aa-103">Verwenden Sie die OneNote-API zum Extrahieren von Visitenkartendaten aus einem Bild oder von Rezept- und Produktdaten von einer URL.</span><span class="sxs-lookup"><span data-stu-id="789aa-103">Use the OneNote API to extract business card data from an image, or recipe and product data from a URL.</span></span>

<a name="attributes"></a>
## <a name="extraction-attributes"></a><span data-ttu-id="789aa-104">Extraktionsattribute</span><span class="sxs-lookup"><span data-stu-id="789aa-104">Extraction attributes</span></span>

<span data-ttu-id="789aa-105">Zum Extrahieren und Transformieren von Daten schließen Sie einfach ein div-Tag in die [create-page](onenote-create-page.md)- oder [update-page](onenote_update_page.md)-Anforderung ein, das den Quellinhalt, die Extraktionsmethode sowie ein Ausweichverhalten angibt.</span><span class="sxs-lookup"><span data-stu-id="789aa-105">To extract and transform data, simply include a div that specifies the source content, extraction method, and fallback behavior in your [create-page](onenote-create-page.md) or [update-page](onenote_update_page.md) request.</span></span> <span data-ttu-id="789aa-106">Die API rendert extrahierte Daten auf der Seite in einem einfach zu lesenden Format.</span><span class="sxs-lookup"><span data-stu-id="789aa-106">The API renders extracted data on the page in an easy-to-read format.</span></span> 

```
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

<span data-ttu-id="789aa-107">**data-render-src**</span><span class="sxs-lookup"><span data-stu-id="789aa-107">**data-render-src**</span></span>

<span data-ttu-id="789aa-108">Die Inhaltsquelle.</span><span class="sxs-lookup"><span data-stu-id="789aa-108">The content source.</span></span> <span data-ttu-id="789aa-109">Dies kann ein Bild einer Visitenkarte oder eine absolute URL von zahlreichen beliebten Rezept- oder Produktwebsites sein.</span><span class="sxs-lookup"><span data-stu-id="789aa-109">This can be an image of a business card or an absolute URL from many popular recipe or product websites.</span></span> <span data-ttu-id="789aa-110">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="789aa-110">Required.</span></span>

<span data-ttu-id="789aa-111">Verwenden Sie für optimale Ergebnisse beim Angeben einer URL die kanonische URL, die ggf. im HTML-Code der Quellwebseite definiert ist.</span><span class="sxs-lookup"><span data-stu-id="789aa-111">For best results when sending a URL, use the canonical URL defined in the  HTML of the source webpage, if one is defined. Example: <link rel="canonical" href="www.domainname.com/page/123/size12/type987" />.</span></span> <span data-ttu-id="789aa-112">Eine kanonische URL kann beispielsweise folgendermaßen in der Quellwebseite definiert werden:</span><span class="sxs-lookup"><span data-stu-id="789aa-112">For example, a canonical URL might be defined in the source webpage like this:</span></span>

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


<span data-ttu-id="789aa-113">**data-render-method**</span><span class="sxs-lookup"><span data-stu-id="789aa-113">**data-render-method**</span></span>

<span data-ttu-id="789aa-114">Die auszuführende Extraktionsmethode.</span><span class="sxs-lookup"><span data-stu-id="789aa-114">The extraction method to run:</span></span> <span data-ttu-id="789aa-115">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="789aa-115">Required.</span></span>

| <span data-ttu-id="789aa-116">Wert</span><span class="sxs-lookup"><span data-stu-id="789aa-116">Value</span></span> | <span data-ttu-id="789aa-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="789aa-117">Description</span></span> |
|:------|:------|
| <span data-ttu-id="789aa-118">extract.businesscard</span><span class="sxs-lookup"><span data-stu-id="789aa-118">extract.businesscard</span></span> | <span data-ttu-id="789aa-119">Extraktionen von Visitenkarten.</span><span class="sxs-lookup"><span data-stu-id="789aa-119">A business card extraction.</span></span> |
| <span data-ttu-id="789aa-120">extract.recipe</span><span class="sxs-lookup"><span data-stu-id="789aa-120">extract.recipe</span></span> | <span data-ttu-id="789aa-121">Extraktionen von Rezepten.</span><span class="sxs-lookup"><span data-stu-id="789aa-121">A recipe extraction.</span></span> |
| <span data-ttu-id="789aa-122">extract.product</span><span class="sxs-lookup"><span data-stu-id="789aa-122">extract.product</span></span> | <span data-ttu-id="789aa-123">Extraktionen von Produktlisten.</span><span class="sxs-lookup"><span data-stu-id="789aa-123">A product listing extraction.</span></span> |
| <span data-ttu-id="789aa-124">extract</span><span class="sxs-lookup"><span data-stu-id="789aa-124">Extract</span></span> | <span data-ttu-id="789aa-125">Ein unbekannter Datenextraktionstyp.</span><span class="sxs-lookup"><span data-stu-id="789aa-125">An unknown extraction type.</span></span> |

<span data-ttu-id="789aa-126">Für optimale Ergebnisse geben Sie den Inhaltstyp (`extract.businesscard`, `extract.recipe` oder `extract.product`) an, falls bekannt.</span><span class="sxs-lookup"><span data-stu-id="789aa-126">For best results, specify the content type (`extract.businesscard`, `extract.recipe`, or `extract.product`) if you know it.</span></span> <span data-ttu-id="789aa-127">Wenn der Typ nicht bekannt ist, verwenden Sie die `extract`-Methode; die OneNote-API versucht daraufhin, den Typ automatisch zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="789aa-127">For best results, specify the content type (business card, recipe, or product) if you know it. If  the type is unknown, you can use the extract method and the onnvshort API will try to auto-detect the type.</span></span>

<span data-ttu-id="789aa-128">**data-render-fallback**</span><span class="sxs-lookup"><span data-stu-id="789aa-128">**data-render-fallback**</span></span>

<span data-ttu-id="789aa-129">Das Ausweichverhalten, wenn die Extraktion fehlschlägt.</span><span class="sxs-lookup"><span data-stu-id="789aa-129">The fallback behavior if the extraction fails:</span></span> <span data-ttu-id="789aa-130">Wenn der Wert weggelassen wird, gilt der Standardwert **render**.</span><span class="sxs-lookup"><span data-stu-id="789aa-130">Defaults to **render** if omitted.</span></span> 

| <span data-ttu-id="789aa-131">Wert</span><span class="sxs-lookup"><span data-stu-id="789aa-131">Value</span></span> | <span data-ttu-id="789aa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="789aa-132">Description</span></span> |
|:------|:------|
| <span data-ttu-id="789aa-133">render()</span><span class="sxs-lookup"><span data-stu-id="789aa-133">render()</span></span> | <span data-ttu-id="789aa-134">Rendert das Quellbild oder eine Momentaufnahme der Rezept- oder Produktwebseite.</span><span class="sxs-lookup"><span data-stu-id="789aa-134">Renders the source image or a snapshot of the recipe or product webpage.</span></span> |
| <span data-ttu-id="789aa-135">n/v</span><span class="sxs-lookup"><span data-stu-id="789aa-135">none</span></span> | <span data-ttu-id="789aa-136">Hat keine Wirkung. </span><span class="sxs-lookup"><span data-stu-id="789aa-136">Does nothing.</span></span><br /><span data-ttu-id="789aa-137">Die Option ist nützlich, wenn Sie zusätzlich zum extrahierten Inhalt immer eine Momentaufnahme der Visitenkarte oder Webseite auf der Seite einschließen möchten.</span><span class="sxs-lookup"><span data-stu-id="789aa-137">Does nothing. This option is useful if you want to always include a snapshot of the business card or webpage on  the page in addition to any extracted content. Be sure to send a separate img element in the request.</span></span> <span data-ttu-id="789aa-138">Achten Sie darauf, ein separates `img`-Element in der Anforderung zu senden, wie in den Beispielen dargestellt.</span><span class="sxs-lookup"><span data-stu-id="789aa-138">Be sure to send a separate `img` element in the request, as shown in the examples.</span></span> |

<a name="biz-card"></a>
## <a name="business-card-extractions"></a><span data-ttu-id="789aa-139">Extraktionen von Visitenkarten</span><span class="sxs-lookup"><span data-stu-id="789aa-139">Business card extractions</span></span>

<span data-ttu-id="789aa-140">Die OneNote-API sucht und rendert die folgenden Kontaktinformationen basierend auf dem Bild einer Visitenkarte einer Person oder eines Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="789aa-140">The onnvshort API tries to find and  render the following contact information  based on an image of a person's or company's business card.</span></span>


- <span data-ttu-id="789aa-141">Name</span><span class="sxs-lookup"><span data-stu-id="789aa-141">Name</span></span>
- <span data-ttu-id="789aa-142">Titel</span><span class="sxs-lookup"><span data-stu-id="789aa-142">Title</span></span>
- <span data-ttu-id="789aa-143">Organisation</span><span class="sxs-lookup"><span data-stu-id="789aa-143">Organization</span></span>
- <span data-ttu-id="789aa-144">Telefon- und Faxnummer</span><span class="sxs-lookup"><span data-stu-id="789aa-144">Phone and fax numbers</span></span>
- <span data-ttu-id="789aa-145">Postanschrift und physische Adressen</span><span class="sxs-lookup"><span data-stu-id="789aa-145">Mailing and physical addresses</span></span>
- <span data-ttu-id="789aa-146">E-Mail-Adressen</span><span class="sxs-lookup"><span data-stu-id="789aa-146">Email addresses</span></span>
- <span data-ttu-id="789aa-147">Websites</span><span class="sxs-lookup"><span data-stu-id="789aa-147">Websites</span></span>
   
  ![Ein Beispiel für die Extraktion einer Visitenkarte.](images/biz-card-extraction.png)

<span data-ttu-id="789aa-149">Eine vCard (VCF-Datei) mit den extrahierten Kontaktdaten wird auch in die Seite eingebettet.</span><span class="sxs-lookup"><span data-stu-id="789aa-149">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span> <span data-ttu-id="789aa-150">Die vCard ist eine bequeme Möglichkeit, um die Kontaktinformationen beim Abrufen des HTML-Inhalts der Seite abzurufen.</span><span class="sxs-lookup"><span data-stu-id="789aa-150">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span>

### <a name="common-scenarios-for-business-card-extractions"></a><span data-ttu-id="789aa-151">Häufige Szenarien für Visitenkartenextraktionen</span><span class="sxs-lookup"><span data-stu-id="789aa-151">Common scenarios for business card extractions</span></span>

<span data-ttu-id="789aa-152">**Abbildung zum Extrahieren von Visitenkarteninformationen und Rendern der Visitenkarte**</span><span class="sxs-lookup"><span data-stu-id="789aa-152">**Extract business card information, and also render the business card image**</span></span>

<span data-ttu-id="789aa-153">Geben Sie die `extract.businesscard`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="789aa-153">Specify the `extract.businesscard` method and the `none` fallback.</span></span> <span data-ttu-id="789aa-154">Senden Sie auch ein `img`-Element mit dem `src`-Attribut, das auch auf das Bild verweist.</span><span class="sxs-lookup"><span data-stu-id="789aa-154">Also send an `img` element with the `src` attribute that also references the image.</span></span> <span data-ttu-id="789aa-155">Wenn die API keinen Inhalt extrahieren kann, wird nur das Bild der Visitenkarte gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-155">If the API is unable to extract any content, it renders the business card image only.</span></span>

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


<span data-ttu-id="789aa-156">**Abbildung zum Extrahieren von Visitenkarteninformationen und Rendern des Bilds der Visitenkarte, wenn die Extraktion fehlschlägt**</span><span class="sxs-lookup"><span data-stu-id="789aa-156">**Extract business card information, and render the business card image only if the extraction fails**</span></span>

<span data-ttu-id="789aa-157">Geben Sie die `extract.businesscard`-Methode an, und verwenden Sie das standardmäßige `render`-Ausweichverhalten.</span><span class="sxs-lookup"><span data-stu-id="789aa-157">Specify the `extract.businesscard` method and use the default `render` fallback.</span></span> <span data-ttu-id="789aa-158">Wenn die API keinen Inhalt extrahieren kann, wird stattdessen das Bild der Visitenkarte gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-158">If the API is unable to extract any content, it renders the business card image instead.</span></span>

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
<span data-ttu-id="789aa-159">Bei Visitenkartenextraktionen wird das Bild als benannten Teil in einer mehrteiligen Anforderung gesendet.</span><span class="sxs-lookup"><span data-stu-id="789aa-159">For business card extractions, the image is sent as a named part in a multipart request.</span></span> <span data-ttu-id="789aa-160">Unter [Hinzufügen von Bildern und Dateien](onenote_images_files.md) finden Sie Beispiele, in denen gezeigt wird, wie ein Bild in einer Anforderung gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="789aa-160">See Capture photos and images  for examples that show how to send an image in a create-page request.</span></span>


<a name="recipe"></a>
## <a name="recipe-extractions"></a><span data-ttu-id="789aa-161">Extraktionen von Rezepten</span><span class="sxs-lookup"><span data-stu-id="789aa-161">Recipe extractions</span></span>

<span data-ttu-id="789aa-162">Die OneNote-API sucht und rendert die folgenden Informationen auf der Grundlage einer Rezeptkarten-URL.</span><span class="sxs-lookup"><span data-stu-id="789aa-162">The onnvshort API tries to find and  render the following information based on a recipe's URL.</span></span>

- <span data-ttu-id="789aa-163">Großformatiges Hintergrundbild</span><span class="sxs-lookup"><span data-stu-id="789aa-163">Hero image</span></span>
- <span data-ttu-id="789aa-164">Bewertung</span><span class="sxs-lookup"><span data-stu-id="789aa-164">Rating</span></span>
- <span data-ttu-id="789aa-165">Zutaten</span><span class="sxs-lookup"><span data-stu-id="789aa-165">Ingredients</span></span>
- <span data-ttu-id="789aa-166">Anweisungen</span><span class="sxs-lookup"><span data-stu-id="789aa-166">Instructions</span></span>
- <span data-ttu-id="789aa-167">Vorbereitungs-, Koch- und Gesamtzeiten</span><span class="sxs-lookup"><span data-stu-id="789aa-167">Prep, cook, and total times</span></span>
- <span data-ttu-id="789aa-168">Portionen</span><span class="sxs-lookup"><span data-stu-id="789aa-168">Servings</span></span>

   ![Ein Beispiel für die Extraktion von Rezepten](images/recipe-extraction.png)

<span data-ttu-id="789aa-170">Die API ist für Rezepte von vielen beliebten Websites wie *Allrecipes.com*, *FoodNetwork.com* und *SeriousEats.com* optimiert.</span><span class="sxs-lookup"><span data-stu-id="789aa-170">The API is optimized for recipes from many popular sites such as Allrecipes.com, FoodNetwork.com, and SeriousEats.com.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="789aa-171">Häufige Szenarien für Rezeptextraktionen</span><span class="sxs-lookup"><span data-stu-id="789aa-171">Common scenarios for recipe extractions</span></span>

<span data-ttu-id="789aa-172">**Extrahieren von Rezeptinformationen und Rendern eines Snapshots der Rezeptwebseite**</span><span class="sxs-lookup"><span data-stu-id="789aa-172">**Extract recipe information, and also render a snapshot of the recipe webpage**</span></span>

<span data-ttu-id="789aa-173">Geben Sie die `extract.recipe`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="789aa-173">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="789aa-174">Senden Sie auch ein `img`-Element, wobei das `data-render-src`-Attribut auf die Rezept-URL festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="789aa-174">Also send an `img` element with the `data-render-src` attribute set to the recipe URL.</span></span> <span data-ttu-id="789aa-175">Wenn die API keinen Inhalt extrahieren kann, wird nur ein Snapshot der Rezeptwebseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-175">If the API is unable to extract any content, it renders a snapshot of the recipe webpage only.</span></span>

<span data-ttu-id="789aa-176">Dieses Szenario bietet möglicherweise die meisten Informationen, da die Webseite weitere Informationen, wie z. B. Kundenbewertungen und Vorschläge, enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="789aa-176">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="http://allrecipes.com/recipe/guacamole/" />
```
 

<span data-ttu-id="789aa-177">**Extrahieren von Rezeptinformationen und Rendern eines Snapshots der Rezeptwebseite, wenn die Extraktion fehlschlägt**</span><span class="sxs-lookup"><span data-stu-id="789aa-177">**Extract recipe information, and render a snapshot of the recipe webpage only if the extraction fails**</span></span>

<span data-ttu-id="789aa-178">Geben Sie die `extract.recipe`-Methode an, und verwenden Sie das standardmäßige Render-Ausweichverhalten.</span><span class="sxs-lookup"><span data-stu-id="789aa-178">Specify the `extract.recipe` method and use the default render fallback.</span></span> <span data-ttu-id="789aa-179">Wenn die API keinen Inhalt extrahieren kann, wird stattdessen ein Snapshot der Rezeptwebseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-179">If the API is unable to extract any content, it renders a snapshot of the recipe webpage instead.</span></span>

```html  
<div
    data-render-src="http://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


<span data-ttu-id="789aa-180">**Extrahieren von Rezeptinformationen und Rendern eines Links zum Rezept**</span><span class="sxs-lookup"><span data-stu-id="789aa-180">**Extract recipe information, and also render a link to the recipe**</span></span>

<span data-ttu-id="789aa-181">Geben Sie die `extract.recipe`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="789aa-181">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="789aa-182">Senden Sie auch ein `a`-Element, wobei das `src`-Attribut auf die Rezept-URL festgelegt ist (Sie können alternativ auch andere Informationen senden, die Sie der Seite hinzufügen möchten).</span><span class="sxs-lookup"><span data-stu-id="789aa-182">Extract recipe information, and also render  a link to the recipeSpecify the extract.recipe`a` method and the none`src` fallback. Also send an a element with the src  attribute set to the recipe URL (or you can send any other information you want to add to the page). If the API is unable to extract any content, only the recipe link is rendered.</span></span> <span data-ttu-id="789aa-183">Wenn die API keinen Inhalt extrahieren kann, wird nur der Rezept-Link gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-183">If the API is unable to extract any content, only the recipe link is rendered.</span></span>

```html  
<div
    data-render-src="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>
## <a name="product-listing-extractions"></a><span data-ttu-id="789aa-184">Extraktionen von Produktlisten</span><span class="sxs-lookup"><span data-stu-id="789aa-184">Product listing extractions</span></span>

- <span data-ttu-id="789aa-185">Titel</span><span class="sxs-lookup"><span data-stu-id="789aa-185">Title</span></span>
- <span data-ttu-id="789aa-186">Bewertung</span><span class="sxs-lookup"><span data-stu-id="789aa-186">Rating</span></span>
- <span data-ttu-id="789aa-187">Primäres Bild</span><span class="sxs-lookup"><span data-stu-id="789aa-187">Primary image</span></span>
- <span data-ttu-id="789aa-188">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="789aa-188">Description</span></span>
- <span data-ttu-id="789aa-189">Features</span><span class="sxs-lookup"><span data-stu-id="789aa-189">Features</span></span>
- <span data-ttu-id="789aa-190">Spezifikationen</span><span class="sxs-lookup"><span data-stu-id="789aa-190">Specifications</span></span></td>

  ![Ein Beispiel für die Extraktion einer Produktliste.](images/product-extraction.png)

<span data-ttu-id="789aa-192">Die API ist für Produkte von vielen beliebten Websites wie *Amazon.com* und *HomeDepot.com* optimiert.</span><span class="sxs-lookup"><span data-stu-id="789aa-192">The API is optimized for products from many popular sites such as Amazon.com, HomeDepot.com, and Sears.com.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="789aa-193">Häufige Szenarien für Rezeptextraktionen</span><span class="sxs-lookup"><span data-stu-id="789aa-193">Common scenarios for recipe extractions</span></span>

<span data-ttu-id="789aa-194">**Extrahieren von Produktinformationen und Rendern eines Snapshots der Produktwebseite**</span><span class="sxs-lookup"><span data-stu-id="789aa-194">**Extract product information, and also render a snapshot of the product webpage**</span></span>

<span data-ttu-id="789aa-195">Geben Sie die `extract.product`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="789aa-195">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="789aa-196">Senden Sie auch ein `img`-Element, wobei das `data-render-src`-Attribut auf die Produkt-URL festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="789aa-196">Also send an `img` element with the `data-render-src` attribute set to the product URL.</span></span> <span data-ttu-id="789aa-197">Wenn die API keinen Inhalt extrahieren kann, wird nur ein Snapshot der Produktwebseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-197">If the API is unable to extract any content, it renders a snapshot of the product webpage only.</span></span>

<span data-ttu-id="789aa-198">Dieses Szenario bietet möglicherweise die meisten Informationen, da die Webseite weitere Informationen, wie z. B. Kundenbewertungen und Vorschläge, enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="789aa-198">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


<span data-ttu-id="789aa-199">**Extrahieren von Produktinformationen und Rendern eines Snapshots der Produktwebseite, wenn die Extraktion fehlschlägt**</span><span class="sxs-lookup"><span data-stu-id="789aa-199">**Extract product information, and render a snapshot of the product webpage only if the extraction fails**</span></span>

<span data-ttu-id="789aa-200">Geben Sie die `extract.product`-Methode an, und verwenden Sie das standardmäßige Render-Ausweichverhalten.</span><span class="sxs-lookup"><span data-stu-id="789aa-200">Specify the `extract.product` method and use the default render fallback.</span></span> <span data-ttu-id="789aa-201">Wenn die API keinen Inhalt extrahieren kann, wird stattdessen ein Snapshot der Produktwebseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-201">If the API is unable to extract any content, it renders a snapshot of the product webpage instead.</span></span>

```html 
<div
    data-render-src="http://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

<span data-ttu-id="789aa-202">**Extrahieren von Produktinformationen und Rendern eines Links zum Produkt**</span><span class="sxs-lookup"><span data-stu-id="789aa-202">**Extract product information, and also render a link to the product**</span></span>

<span data-ttu-id="789aa-203">Geben Sie die `extract.product`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="789aa-203">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="789aa-204">Senden Sie auch ein `a`-Element, wobei das `src`-Attribut auf die Produkt-URL festgelegt ist (Sie können alternativ auch andere Informationen senden, die Sie der Seite hinzufügen möchten).</span><span class="sxs-lookup"><span data-stu-id="789aa-204">Extract product information, and also render  a link to the productSpecify the extract.product`a` method and the none`src` fallback. Also send an a element with the src  attribute set to the product URL (or you can send any other information you want to add to the page). If the API is unable to extract any content, only the page link is rendered.</span></span> <span data-ttu-id="789aa-205">Wenn die API keinen Inhalt extrahieren kann, wird nur der Seitenlink gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-205">If the API is unable to extract any content, only the page link is rendered.</span></span>

```html 
<div
    data-render-src="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 
## <a name="unknown-content-type-extractions"></a><span data-ttu-id="789aa-206">Extraktionen unbekannter Inhaltstypen</span><span class="sxs-lookup"><span data-stu-id="789aa-206">Unknown content type extractions</span></span>

<span data-ttu-id="789aa-207">Wenn Sie den Inhaltstyp (Visitenkarte, Rezept oder Produkt), den Sie versenden möchten, nicht kennen, können Sie die unqualifizierte `extract`-Methode verwenden und die OneNote-API den Typ automatisch erkennen lassen.</span><span class="sxs-lookup"><span data-stu-id="789aa-207">If you don't know the content type (business card, recipe, or product) that you're sending,   you can use the unqualified extract method and let the onnvshort API automatically detect the type. You might want to do this if your app sends different capture types.</span></span> <span data-ttu-id="789aa-208">Dies ist möglicherweise sinnvoll, wenn Ihre App andere Erfassungstypen sendet.</span><span class="sxs-lookup"><span data-stu-id="789aa-208">You might want to do this if your app sends different capture types.</span></span>

> <span data-ttu-id="789aa-209">**Hinweis:** Wenn Sie den Inhaltstyp kennen, den Sie senden, verwenden Sie die Methode `extract.businesscard`, `extract.recipe` oder `extract.product`.</span><span class="sxs-lookup"><span data-stu-id="789aa-209">**Note:** If you do know the content type that you're sending, you should use the `extract.businesscard`, `extract.recipe`, or `extract.product` method.</span></span> <span data-ttu-id="789aa-210">In einigen Fällen kann dies hilfreich sein, um die Extraktionsergebnisse zu optimieren.</span><span class="sxs-lookup"><span data-stu-id="789aa-210">In some cases, this can help to optimize the extraction results.</span></span>
 
### <a name="common-scenarios-for-unknown-extractions"></a><span data-ttu-id="789aa-211">Häufige Szenarien für Extraktionen unbekannter Inhaltstypen</span><span class="sxs-lookup"><span data-stu-id="789aa-211">Common  scenarios for article extractions</span></span>

<span data-ttu-id="789aa-212">**Senden Sie ein Bild oder eine URL, und rendern Sie das bereitgestellte Bild oder einen Snapshot der Webseite, wenn die Extraktion fehlschlägt**</span><span class="sxs-lookup"><span data-stu-id="789aa-212">**Send an image or a URL, and render the supplied image or a snapshot of the webpage if the extraction fails**</span></span>

<span data-ttu-id="789aa-213">Geben Sie die `extract`-Methode an, damit die API den Inhaltstyp automatisch erkennen kann und verwenden Sie das standardmäßige render-Ausweichverhalten.</span><span class="sxs-lookup"><span data-stu-id="789aa-213">Specify the `extract` method so the API automatically detects the content type, and use the default render fallback.</span></span> <span data-ttu-id="789aa-214">Wenn die API keinen Inhalt extrahieren kann, wird stattdessen das bereitgestellte Bild oder ein Snapshot der Webseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="789aa-214">If the API is unable to extract any content, it renders the supplied image or snapshot of the webpage instead.</span></span>

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>
## <a name="response-information"></a><span data-ttu-id="789aa-215">Informationen in der Antwort</span><span class="sxs-lookup"><span data-stu-id="789aa-215">Response information</span></span>

| <span data-ttu-id="789aa-216">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="789aa-216">Response data</span></span> | <span data-ttu-id="789aa-217">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="789aa-217">Description</span></span> |  
|------|------|  
| <span data-ttu-id="789aa-218">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="789aa-218">Success code</span></span> | <span data-ttu-id="789aa-219">HTTP-Statuscode 201 für eine erfolgreiche POST-Anforderung, HTTP-Statuscode 204 für eine erfolgreiche PATCH-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="789aa-219">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="789aa-220">Fehler</span><span class="sxs-lookup"><span data-stu-id="789aa-220">Errors</span></span>| <span data-ttu-id="789aa-221">Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote_error_codes.md).</span><span class="sxs-lookup"><span data-stu-id="789aa-221">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="789aa-222">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="789aa-222">Permissions</span></span>

<span data-ttu-id="789aa-223">Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="789aa-223">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="789aa-224">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="789aa-224">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="789aa-225">**Berechtigungen für _POST Pages_**</span><span class="sxs-lookup"><span data-stu-id="789aa-225">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="789aa-226">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="789aa-226">Notes.Create</span></span>
- <span data-ttu-id="789aa-227">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="789aa-227">Notes.ReadWrite</span></span>
- <span data-ttu-id="789aa-228">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789aa-228">Notes.ReadWrite.All</span></span>  

<span data-ttu-id="789aa-229">**Berechtigungen für _PATCH Pages_**</span><span class="sxs-lookup"><span data-stu-id="789aa-229">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="789aa-230">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="789aa-230">Notes.ReadWrite</span></span>
- <span data-ttu-id="789aa-231">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789aa-231">Notes.ReadWrite.All</span></span>

<span data-ttu-id="789aa-232">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="789aa-232">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="789aa-233">Weitere Ressourcen</span><span class="sxs-lookup"><span data-stu-id="789aa-233">Additional resources</span></span>

- [<span data-ttu-id="789aa-234">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="789aa-234">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="789aa-235">Aktualisieren mit OneNote-Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="789aa-235">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="789aa-236">Hinzufügen von Bildern und Dateien</span><span class="sxs-lookup"><span data-stu-id="789aa-236">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="789aa-237">Integrieren in OneNote</span><span class="sxs-lookup"><span data-stu-id="789aa-237">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="789aa-238">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="789aa-238">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="789aa-239">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="789aa-239">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="789aa-240">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="789aa-240">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  


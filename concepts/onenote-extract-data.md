# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a><span data-ttu-id="32f74-101">Verwenden von div-Tags der OneNote-API zum Extrahieren von Daten aus Erfassungen</span><span class="sxs-lookup"><span data-stu-id="32f74-101">Use OneNote API div tags to extract data from captures</span></span> 

<span data-ttu-id="32f74-102">**Gilt für** Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365</span><span class="sxs-lookup"><span data-stu-id="32f74-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="32f74-103">Verwenden Sie die OneNote-API zum Extrahieren von Visitenkartendaten aus einem Bild oder von Rezept- und Produktdaten von einer URL.</span><span class="sxs-lookup"><span data-stu-id="32f74-103">Use the OneNote API to extract business card data from an image, or recipe and product data from a URL.</span></span>

<a name="attributes"></a>

## <a name="extraction-attributes"></a><span data-ttu-id="32f74-104">Extraktionsattribute</span><span class="sxs-lookup"><span data-stu-id="32f74-104">Extraction attributes</span></span>

<span data-ttu-id="32f74-105">Zum Extrahieren und Transformieren von Daten schließen Sie einfach ein div-Tag in die [create-page](onenote-create-page.md)- oder [update-page](onenote_update_page.md)-Anforderung ein, das den Quellinhalt, die Extraktionsmethode sowie ein Ausweichverhalten angibt.</span><span class="sxs-lookup"><span data-stu-id="32f74-105">To extract and transform data, simply include a div that specifies the source content, extraction method, and fallback behavior in your [create-page](onenote-create-page.md) or [update-page](onenote_update_page.md) request.</span></span> <span data-ttu-id="32f74-106">Die API rendert extrahierte Daten auf der Seite in einem einfach zu lesenden Format.</span><span class="sxs-lookup"><span data-stu-id="32f74-106">The API renders extracted data on the page in an easy-to-read format.</span></span> 

```html
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

### <a name="data-render-src"></a><span data-ttu-id="32f74-107">data-render-src</span><span class="sxs-lookup"><span data-stu-id="32f74-107">data-render-src</span></span>

<span data-ttu-id="32f74-108">Die Inhaltsquelle.</span><span class="sxs-lookup"><span data-stu-id="32f74-108">The content source.</span></span> <span data-ttu-id="32f74-109">Dies kann ein Bild einer Visitenkarte oder eine absolute URL von zahlreichen beliebten Rezept- oder Produktwebsites sein.</span><span class="sxs-lookup"><span data-stu-id="32f74-109">This can be an image of a business card or an absolute URL from many popular recipe or product websites.</span></span> <span data-ttu-id="32f74-110">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="32f74-110">Required.</span></span>

<span data-ttu-id="32f74-111">Verwenden Sie für optimale Ergebnisse beim Angeben einer URL die kanonische URL, die ggf. im HTML-Code der Quellwebseite definiert ist.</span><span class="sxs-lookup"><span data-stu-id="32f74-111">For best results when specifying a URL, use the canonical URL defined in the HTML of the source webpage, if one is defined.</span></span> <span data-ttu-id="32f74-112">Eine kanonische URL kann beispielsweise folgendermaßen in der Quellwebseite definiert werden:</span><span class="sxs-lookup"><span data-stu-id="32f74-112">For example, a canonical URL might be defined in the source webpage like this:</span></span>

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


### <a name="data-render-method"></a><span data-ttu-id="32f74-113">data-render-method</span><span class="sxs-lookup"><span data-stu-id="32f74-113">data-render-method</span></span>

<span data-ttu-id="32f74-114">Die auszuführende Extraktionsmethode.</span><span class="sxs-lookup"><span data-stu-id="32f74-114">The extraction method to run.</span></span> <span data-ttu-id="32f74-115">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="32f74-115">Required.</span></span>

| <span data-ttu-id="32f74-116">Wert</span><span class="sxs-lookup"><span data-stu-id="32f74-116">Value</span></span> | <span data-ttu-id="32f74-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32f74-117">Description</span></span> |
|:------|:------|
| <span data-ttu-id="32f74-118">extract.businesscard</span><span class="sxs-lookup"><span data-stu-id="32f74-118">extract.businesscard</span></span> | <span data-ttu-id="32f74-119">Extraktionen von Visitenkarten.</span><span class="sxs-lookup"><span data-stu-id="32f74-119">A business card extraction.</span></span> |
| <span data-ttu-id="32f74-120">extract.recipe</span><span class="sxs-lookup"><span data-stu-id="32f74-120">extract.recipe</span></span> | <span data-ttu-id="32f74-121">Extraktionen von Rezepten.</span><span class="sxs-lookup"><span data-stu-id="32f74-121">A recipe extraction.</span></span> |
| <span data-ttu-id="32f74-122">extract.product</span><span class="sxs-lookup"><span data-stu-id="32f74-122">extract.product</span></span> | <span data-ttu-id="32f74-123">Extraktionen von Produktlisten.</span><span class="sxs-lookup"><span data-stu-id="32f74-123">A product listing extraction.</span></span> |
| <span data-ttu-id="32f74-124">extract</span><span class="sxs-lookup"><span data-stu-id="32f74-124">extract</span></span> | <span data-ttu-id="32f74-125">Ein unbekannter Datenextraktionstyp.</span><span class="sxs-lookup"><span data-stu-id="32f74-125">An unknown extraction type.</span></span> |

<span data-ttu-id="32f74-126">Für optimale Ergebnisse geben Sie den Inhaltstyp (`extract.businesscard`, `extract.recipe` oder `extract.product`) an, falls bekannt.</span><span class="sxs-lookup"><span data-stu-id="32f74-126">For best results, specify the content type (`extract.businesscard`, `extract.recipe`, or `extract.product`) if you know it.</span></span> <span data-ttu-id="32f74-127">Wenn der Typ nicht bekannt ist, verwenden Sie die `extract`-Methode, und die OneNote-API versucht daraufhin, den Typ automatisch zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="32f74-127">If the type is unknown, use the `extract` method and the OneNote API will try to auto-detect the type.</span></span>

### <a name="data-render-fallback"></a><span data-ttu-id="32f74-128">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="32f74-128">data-render-fallback</span></span>

<span data-ttu-id="32f74-129">Das Ausweichverhalten, wenn die Extraktion fehlschlägt.</span><span class="sxs-lookup"><span data-stu-id="32f74-129">The fallback behavior if the extraction fails.</span></span> <span data-ttu-id="32f74-130">Wenn der Wert weggelassen wird, gilt der Standardwert **render**.</span><span class="sxs-lookup"><span data-stu-id="32f74-130">Defaults to **render** if omitted.</span></span> 

| <span data-ttu-id="32f74-131">Wert</span><span class="sxs-lookup"><span data-stu-id="32f74-131">Value</span></span> | <span data-ttu-id="32f74-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32f74-132">Description</span></span> |
|:------|:------|
| <span data-ttu-id="32f74-133">render()</span><span class="sxs-lookup"><span data-stu-id="32f74-133">render</span></span> | <span data-ttu-id="32f74-134">Rendert das Quellbild oder eine Momentaufnahme der Rezept- oder Produktwebseite.</span><span class="sxs-lookup"><span data-stu-id="32f74-134">Renders the source image or a snapshot of the recipe or product webpage.</span></span> |
| <span data-ttu-id="32f74-135">n/v</span><span class="sxs-lookup"><span data-stu-id="32f74-135">none</span></span> | <span data-ttu-id="32f74-136">Hat keine Wirkung. </span><span class="sxs-lookup"><span data-stu-id="32f74-136">Does nothing.</span></span><br /><br /><span data-ttu-id="32f74-137">Die Option ist nützlich, wenn Sie zusätzlich zum extrahierten Inhalt immer eine Momentaufnahme der Visitenkarte oder Webseite auf der Seite einschließen möchten.</span><span class="sxs-lookup"><span data-stu-id="32f74-137">This option is useful if you want to always include a snapshot of the business card or webpage on the page in addition to any extracted content.</span></span> <span data-ttu-id="32f74-138">Achten Sie darauf, ein separates `img`-Element in der Anforderung zu senden, wie in den Beispielen dargestellt.</span><span class="sxs-lookup"><span data-stu-id="32f74-138">Be sure to send a separate `img` element in the request, as shown in the examples.</span></span> |

<a name="biz-card"></a>

## <a name="business-card-extractions"></a><span data-ttu-id="32f74-139">Extraktionen von Visitenkarten</span><span class="sxs-lookup"><span data-stu-id="32f74-139">Business card extractions</span></span>

<span data-ttu-id="32f74-140">Die OneNote-API sucht und rendert die folgenden Kontaktinformationen basierend auf dem Bild einer Visitenkarte einer Person oder eines Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="32f74-140">The OneNote API tries to find and render the following contact information based on an image of a person's or company's business card.</span></span>

- <span data-ttu-id="32f74-141">Name</span><span class="sxs-lookup"><span data-stu-id="32f74-141">Name</span></span>
- <span data-ttu-id="32f74-142">Titel</span><span class="sxs-lookup"><span data-stu-id="32f74-142">Title</span></span>
- <span data-ttu-id="32f74-143">Organisation</span><span class="sxs-lookup"><span data-stu-id="32f74-143">Organization</span></span>
- <span data-ttu-id="32f74-144">Telefon- und Faxnummer</span><span class="sxs-lookup"><span data-stu-id="32f74-144">Phone and fax numbers</span></span>
- <span data-ttu-id="32f74-145">Postanschrift und physische Adressen</span><span class="sxs-lookup"><span data-stu-id="32f74-145">Mailing and physical addresses</span></span>
- <span data-ttu-id="32f74-146">E-Mail-Adressen</span><span class="sxs-lookup"><span data-stu-id="32f74-146">Email addresses</span></span>
- <span data-ttu-id="32f74-147">Websites</span><span class="sxs-lookup"><span data-stu-id="32f74-147">Websites</span></span>



<img alt="An example business card extraction" src="images/biz-card-extraction.png" width="200">

<span data-ttu-id="32f74-p108">Eine vCard (.VCF-Datei) mit den extrahierten Kontaktinformationen wird ebenfalls in die Seite eingebettet. Die vCard-Datei ist eine bequeme Möglichkeit zum Abrufen von Kontaktinformationen beim Abrufen von HTML-Seiteninhalten.</span><span class="sxs-lookup"><span data-stu-id="32f74-p108">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span>

### <a name="common-scenarios-for-business-card-extractions"></a><span data-ttu-id="32f74-150">Häufige Szenarien für Visitenkartenextraktionen</span><span class="sxs-lookup"><span data-stu-id="32f74-150">Common scenarios for business card extractions</span></span>

#### <a name="extract-business-card-information-and-also-render-the-business-card-image"></a><span data-ttu-id="32f74-151">Abbildung zum Extrahieren von Visitenkarteninformationen und Rendern der Visitenkarte</span><span class="sxs-lookup"><span data-stu-id="32f74-151">Extract business card information, and also render the business card image</span></span>

<span data-ttu-id="32f74-152">Geben Sie die `extract.businesscard`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="32f74-152">Specify the `extract.businesscard` method and the `none` fallback.</span></span> <span data-ttu-id="32f74-153">Senden Sie auch ein `img`-Element mit dem `src`-Attribut, das auch auf das Bild verweist.</span><span class="sxs-lookup"><span data-stu-id="32f74-153">Also send an `img` element with the `src` attribute that also references the image.</span></span> <span data-ttu-id="32f74-154">Wenn die API keinen Inhalt extrahieren kann, wird nur das Bild der Visitenkarte gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-154">If the API is unable to extract any content, it renders the business card image only.</span></span>

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


#### <a name="extract-business-card-information-and-render-the-business-card-image-only-if-the-extraction-fails"></a><span data-ttu-id="32f74-155">Abbildung zum Extrahieren von Visitenkarteninformationen und Rendern des Bilds der Visitenkarte, wenn die Extraktion fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="32f74-155">Extract business card information, and render the business card image only if the extraction fails</span></span>

<span data-ttu-id="32f74-156">Geben Sie die `extract.businesscard`-Methode an, und verwenden Sie das standardmäßige `render`-Ausweichverhalten.</span><span class="sxs-lookup"><span data-stu-id="32f74-156">Specify the `extract.businesscard` method and use the default `render` fallback.</span></span> <span data-ttu-id="32f74-157">Wenn die API keinen Inhalt extrahieren kann, wird stattdessen das Bild der Visitenkarte gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-157">If the API is unable to extract any content, it renders the business card image instead.</span></span>

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
<span data-ttu-id="32f74-158">Bei Visitenkartenextraktionen wird das Bild als benannten Teil in einer mehrteiligen Anforderung gesendet.</span><span class="sxs-lookup"><span data-stu-id="32f74-158">For business card extractions, the image is sent as a named part in a multipart request.</span></span> <span data-ttu-id="32f74-159">Unter [Hinzufügen von Bildern und Dateien](onenote_images_files.md) finden Sie Beispiele, in denen gezeigt wird, wie ein Bild in einer Anforderung gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="32f74-159">See [Add images and files](onenote_images_files.md) for examples that show how to send an image in a request.</span></span>


<a name="recipe"></a>

## <a name="recipe-extractions"></a><span data-ttu-id="32f74-160">Extraktionen von Rezepten</span><span class="sxs-lookup"><span data-stu-id="32f74-160">Recipe extractions</span></span>

<span data-ttu-id="32f74-161">Die OneNote-API sucht und rendert die folgenden Informationen auf der Grundlage einer Rezeptkarten-URL.</span><span class="sxs-lookup"><span data-stu-id="32f74-161">The OneNote API tries to find and render the following information based on a recipe's URL.</span></span>

- <span data-ttu-id="32f74-162">Großformatiges Hintergrundbild</span><span class="sxs-lookup"><span data-stu-id="32f74-162">Hero image</span></span>
- <span data-ttu-id="32f74-163">Bewertung</span><span class="sxs-lookup"><span data-stu-id="32f74-163">Rating</span></span>
- <span data-ttu-id="32f74-164">Zutaten</span><span class="sxs-lookup"><span data-stu-id="32f74-164">Ingredients</span></span>
- <span data-ttu-id="32f74-165">Anweisungen</span><span class="sxs-lookup"><span data-stu-id="32f74-165">Instructions</span></span>
- <span data-ttu-id="32f74-166">Vorbereitungs-, Koch- und Gesamtzeiten</span><span class="sxs-lookup"><span data-stu-id="32f74-166">Prep, cook, and total times</span></span>
- <span data-ttu-id="32f74-167">Portionen</span><span class="sxs-lookup"><span data-stu-id="32f74-167">Servings</span></span>


<img alt="An example recipe extraction" src="images/recipe-extraction.png" width="200">

<span data-ttu-id="32f74-168">Die API ist für Rezepte von vielen beliebten Websites wie *Allrecipes.com*, *FoodNetwork.com* und *SeriousEats.com* optimiert.</span><span class="sxs-lookup"><span data-stu-id="32f74-168">The API is optimized for recipes from many popular sites such as *Allrecipes.com*, *FoodNetwork.com*, and *SeriousEats.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="32f74-169">Häufige Szenarien für Rezeptextraktionen</span><span class="sxs-lookup"><span data-stu-id="32f74-169">Common scenarios for recipe extractions</span></span>

#### <a name="extract-recipe-information-and-also-render-a-snapshot-of-the-recipe-webpage"></a><span data-ttu-id="32f74-170">Extrahieren von Rezeptinformationen und Rendern eines Snapshots der Rezeptwebseite</span><span class="sxs-lookup"><span data-stu-id="32f74-170">Extract recipe information, and also render a snapshot of the recipe webpage</span></span>

<span data-ttu-id="32f74-171">Geben Sie die `extract.recipe`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="32f74-171">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="32f74-172">Senden Sie auch ein `img`-Element, wobei das `data-render-src`-Attribut auf die Rezept-URL festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="32f74-172">Also send an `img` element with the `data-render-src` attribute set to the recipe URL.</span></span> <span data-ttu-id="32f74-173">Wenn die API keinen Inhalt extrahieren kann, wird nur ein Snapshot der Rezeptwebseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-173">If the API is unable to extract any content, it renders a snapshot of the recipe webpage only.</span></span>

<span data-ttu-id="32f74-174">Dieses Szenario bietet möglicherweise die meisten Informationen, da die Webseite weitere Informationen, wie z. B. Kundenbewertungen und Vorschläge, enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="32f74-174">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="http://allrecipes.com/recipe/guacamole/" />
```
 

#### <a name="extract-recipe-information-and-render-a-snapshot-of-the-recipe-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="32f74-175">Extrahieren von Rezeptinformationen und Rendern eines Snapshots der Rezeptwebseite, wenn die Extraktion fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="32f74-175">Extract recipe information, and render a snapshot of the recipe webpage only if the extraction fails</span></span>

<span data-ttu-id="32f74-176">Geben Sie die `extract.recipe`-Methode an, und verwenden Sie das standardmäßige Render-Ausweichverhalten.</span><span class="sxs-lookup"><span data-stu-id="32f74-176">Specify the `extract.recipe` method and use the default render fallback.</span></span> <span data-ttu-id="32f74-177">Wenn die API keinen Inhalt extrahieren kann, wird stattdessen ein Snapshot der Rezeptwebseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-177">If the API is unable to extract any content, it renders a snapshot of the recipe webpage instead.</span></span>

```html  
<div
    data-render-src="http://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


#### <a name="extract-recipe-information-and-also-render-a-link-to-the-recipe"></a><span data-ttu-id="32f74-178">Extrahieren von Rezeptinformationen und Rendern eines Links zum Rezept</span><span class="sxs-lookup"><span data-stu-id="32f74-178">Extract recipe information, and also render a link to the recipe</span></span>

<span data-ttu-id="32f74-179">Geben Sie die `extract.recipe`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="32f74-179">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="32f74-180">Senden Sie auch ein `a`-Element, wobei das `src`-Attribut auf die Rezept-URL festgelegt ist (Sie können alternativ auch andere Informationen senden, die Sie der Seite hinzufügen möchten).</span><span class="sxs-lookup"><span data-stu-id="32f74-180">Also send an `a` element with the `src` attribute set to the recipe URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="32f74-181">Wenn die API keinen Inhalt extrahieren kann, wird nur der Rezept-Link gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-181">If the API is unable to extract any content, only the recipe link is rendered.</span></span>

```html  
<div
    data-render-src="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>

## <a name="product-listing-extractions"></a><span data-ttu-id="32f74-182">Extraktionen von Produktlisten</span><span class="sxs-lookup"><span data-stu-id="32f74-182">Product listing extractions</span></span>

- <span data-ttu-id="32f74-183">Titel</span><span class="sxs-lookup"><span data-stu-id="32f74-183">Title</span></span>
- <span data-ttu-id="32f74-184">Bewertung</span><span class="sxs-lookup"><span data-stu-id="32f74-184">Rating</span></span>
- <span data-ttu-id="32f74-185">Primäres Bild</span><span class="sxs-lookup"><span data-stu-id="32f74-185">Primary image</span></span>
- <span data-ttu-id="32f74-186">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32f74-186">Description</span></span>
- <span data-ttu-id="32f74-187">Features</span><span class="sxs-lookup"><span data-stu-id="32f74-187">Features</span></span>
- <span data-ttu-id="32f74-188">Spezifikationen</span><span class="sxs-lookup"><span data-stu-id="32f74-188">Specifications</span></span>



<img alt="An example product listing extraction" src="images/product-extraction.png" width="200">

<span data-ttu-id="32f74-189">Die API ist für Produkte von vielen beliebten Websites wie *Amazon.com* und *HomeDepot.com* optimiert.</span><span class="sxs-lookup"><span data-stu-id="32f74-189">The API is optimized for products from many popular sites such as *Amazon.com* and *HomeDepot.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="32f74-190">Häufige Szenarien für Rezeptextraktionen</span><span class="sxs-lookup"><span data-stu-id="32f74-190">Common scenarios for recipe extractions</span></span>

#### <a name="extract-product-information-and-also-render-a-snapshot-of-the-product-webpage"></a><span data-ttu-id="32f74-191">Extrahieren von Produktinformationen und Rendern eines Snapshots der Produktwebseite</span><span class="sxs-lookup"><span data-stu-id="32f74-191">Extract product information, and also render a snapshot of the product webpage</span></span>

<span data-ttu-id="32f74-192">Geben Sie die `extract.product`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="32f74-192">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="32f74-193">Senden Sie auch ein `img`-Element, wobei das `data-render-src`-Attribut auf die Produkt-URL festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="32f74-193">Also send an `img` element with the `data-render-src` attribute set to the product URL.</span></span> <span data-ttu-id="32f74-194">Wenn die API keinen Inhalt extrahieren kann, wird nur ein Snapshot der Produktwebseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-194">If the API is unable to extract any content, it renders a snapshot of the product webpage only.</span></span>

<span data-ttu-id="32f74-195">Dieses Szenario bietet möglicherweise die meisten Informationen, da die Webseite weitere Informationen, wie z. B. Kundenbewertungen und Vorschläge, enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="32f74-195">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


#### <a name="extract-product-information-and-render-a-snapshot-of-the-product-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="32f74-196">Extrahieren von Produktinformationen und Rendern eines Snapshots der Produktwebseite, wenn die Extraktion fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="32f74-196">Extract product information, and render a snapshot of the product webpage only if the extraction fails</span></span>

<span data-ttu-id="32f74-197">Geben Sie die `extract.product`-Methode an, und verwenden Sie das standardmäßige Render-Ausweichverhalten.</span><span class="sxs-lookup"><span data-stu-id="32f74-197">Specify the `extract.product` method and use the default render fallback.</span></span> <span data-ttu-id="32f74-198">Wenn die API keinen Inhalt extrahieren kann, wird stattdessen ein Snapshot der Produktwebseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-198">If the API is unable to extract any content, it renders a snapshot of the product webpage instead.</span></span>

```html 
<div
    data-render-src="http://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

#### <a name="extract-product-information-and-also-render-a-link-to-the-product"></a><span data-ttu-id="32f74-199">Extrahieren von Produktinformationen und Rendern eines Links zum Produkt</span><span class="sxs-lookup"><span data-stu-id="32f74-199">Extract product information, and also render a link to the product</span></span>

<span data-ttu-id="32f74-200">Geben Sie die `extract.product`-Methode und das `none`-Ausweichverhalten an.</span><span class="sxs-lookup"><span data-stu-id="32f74-200">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="32f74-201">Senden Sie auch ein `a`-Element, wobei das `src`-Attribut auf die Produkt-URL festgelegt ist (Sie können alternativ auch andere Informationen senden, die Sie der Seite hinzufügen möchten).</span><span class="sxs-lookup"><span data-stu-id="32f74-201">Also send an `a` element with the `src` attribute set to the product URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="32f74-202">Wenn die API keinen Inhalt extrahieren kann, wird nur der Seitenlink gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-202">If the API is unable to extract any content, only the page link is rendered.</span></span>

```html 
<div
    data-render-src="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 

## <a name="unknown-content-type-extractions"></a><span data-ttu-id="32f74-203">Extraktionen unbekannter Inhaltstypen</span><span class="sxs-lookup"><span data-stu-id="32f74-203">Unknown content type extractions</span></span>

<span data-ttu-id="32f74-204">Wenn Sie den Inhaltstyp (Visitenkarte, Rezept oder Produkt), den Sie versenden möchten, nicht kennen, können Sie die unqualifizierte `extract`-Methode verwenden und die OneNote-API den Typ automatisch erkennen lassen.</span><span class="sxs-lookup"><span data-stu-id="32f74-204">If you don't know the content type (business card, recipe, or product) that you're sending, you can use the unqualified `extract` method and let the OneNote API automatically detect the type.</span></span> <span data-ttu-id="32f74-205">Dies ist möglicherweise sinnvoll, wenn Ihre App andere Erfassungstypen sendet.</span><span class="sxs-lookup"><span data-stu-id="32f74-205">You might want to do this if your app sends different capture types.</span></span>

> <span data-ttu-id="32f74-206">**Hinweis:** Wenn Sie den Inhaltstyp kennen, den Sie senden, verwenden Sie die Methode `extract.businesscard`, `extract.recipe` oder `extract.product`.</span><span class="sxs-lookup"><span data-stu-id="32f74-206">**Note:** If you do know the content type that you're sending, you should use the `extract.businesscard`, `extract.recipe`, or `extract.product` method.</span></span> <span data-ttu-id="32f74-207">In einigen Fällen kann dies hilfreich sein, um die Extraktionsergebnisse zu optimieren.</span><span class="sxs-lookup"><span data-stu-id="32f74-207">In some cases, this can help to optimize the extraction results.</span></span>
 
### <a name="common-scenarios-for-unknown-extractions"></a><span data-ttu-id="32f74-208">Häufige Szenarien für Extraktionen unbekannter Inhaltstypen</span><span class="sxs-lookup"><span data-stu-id="32f74-208">Common scenarios for unknown extractions</span></span>

#### <a name="send-an-image-or-a-url-and-render-the-supplied-image-or-a-snapshot-of-the-webpage-if-the-extraction-fails"></a><span data-ttu-id="32f74-209">Senden Sie ein Bild oder eine URL, und rendern Sie das bereitgestellte Bild oder einen Snapshot der Webseite, wenn die Extraktion fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="32f74-209">Send an image or a URL, and render the supplied image or a snapshot of the webpage if the extraction fails</span></span>

<span data-ttu-id="32f74-210">Geben Sie die `extract`-Methode an, damit die API den Inhaltstyp automatisch erkennen kann und verwenden Sie das standardmäßige render-Ausweichverhalten.</span><span class="sxs-lookup"><span data-stu-id="32f74-210">Specify the `extract` method so the API automatically detects the content type, and use the default render fallback.</span></span> <span data-ttu-id="32f74-211">Wenn die API keinen Inhalt extrahieren kann, wird stattdessen das bereitgestellte Bild oder ein Snapshot der Webseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="32f74-211">If the API is unable to extract any content, it renders the supplied image or snapshot of the webpage instead.</span></span>

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="32f74-212">Informationen in der Antwort</span><span class="sxs-lookup"><span data-stu-id="32f74-212">Response information</span></span>

| <span data-ttu-id="32f74-213">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="32f74-213">Response data</span></span> | <span data-ttu-id="32f74-214">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32f74-214">Description</span></span> |  
|------|------|  
| <span data-ttu-id="32f74-215">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="32f74-215">Success code</span></span> | <span data-ttu-id="32f74-216">HTTP-Statuscode 201 bei erfolgreich ausgeführter POST-Anforderung, HTTP-Statuscode 204 bei erfolgreich ausgeführter PATCH-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32f74-216">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="32f74-217">Fehler</span><span class="sxs-lookup"><span data-stu-id="32f74-217">Errors</span></span>| <span data-ttu-id="32f74-218">Informationen zu OneNote-Fehlern, die Microsoft Graph zurückgeben kann, finden Sie unter [Fehlercodes für OneNote-APIs in Microsoft Graph](onenote_error_codes.md).</span><span class="sxs-lookup"><span data-stu-id="32f74-218">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="32f74-219">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="32f74-219">Permissions</span></span>

<span data-ttu-id="32f74-220">Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="32f74-220">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="32f74-221">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="32f74-221">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="32f74-222">Berechtigungen für BEITRAG-Seiten</span><span class="sxs-lookup"><span data-stu-id="32f74-222">Permissions for POST pages</span></span>

- <span data-ttu-id="32f74-223">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="32f74-223">Notes.Create</span></span>
- <span data-ttu-id="32f74-224">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32f74-224">Notes.ReadWrite</span></span>
- <span data-ttu-id="32f74-225">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32f74-225">Notes.ReadWrite.All</span></span>  

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="32f74-226">Berechtigungen für PATCH-Seiten</span><span class="sxs-lookup"><span data-stu-id="32f74-226">Permissions for PATCH pages</span></span>

- <span data-ttu-id="32f74-227">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32f74-227">Notes.ReadWrite</span></span>
- <span data-ttu-id="32f74-228">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32f74-228">Notes.ReadWrite.All</span></span>

<span data-ttu-id="32f74-229">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32f74-229">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="32f74-230">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="32f74-230">See also</span></span>

- [<span data-ttu-id="32f74-231">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="32f74-231">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="32f74-232">Aktualisieren mit OneNote-Seiteninhalt</span><span class="sxs-lookup"><span data-stu-id="32f74-232">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="32f74-233">Hinzufügen von Bildern und Dateien</span><span class="sxs-lookup"><span data-stu-id="32f74-233">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="32f74-234">Integrieren mit OneNote</span><span class="sxs-lookup"><span data-stu-id="32f74-234">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="32f74-235">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="32f74-235">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="32f74-236">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="32f74-236">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="32f74-237">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="32f74-237">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  


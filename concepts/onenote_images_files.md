
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="83afe-101">Hinzufügen von Bildern, Videos und Dateien zu OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="83afe-101">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="83afe-102">*__Gilt für:__ Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365*</span><span class="sxs-lookup"><span data-stu-id="83afe-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="83afe-103">Sie können Elemente der Typen **img**, **object** und **iframe** verwenden, um bei der [Erstellung](onenote-create-page.md) oder [Aktualisierung](onenote_update_page.md) von OneNote-Seiten Bilder, Videos und Dateien zur Seite hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="83afe-103">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote_update_page.md) the page.</span></span> 

- <span data-ttu-id="83afe-104">Verwenden Sie **img**, um ein Bild auf der Seite zu rendern.</span><span class="sxs-lookup"><span data-stu-id="83afe-104">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="83afe-105">Verwenden Sie **iframe**, um ein Video in die Seite einzubetten.</span><span class="sxs-lookup"><span data-stu-id="83afe-105">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="83afe-106">Verwenden Sie **object**, um der Seite eine Dateianlage hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="83afe-106">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>
## <a name="adding-images"></a><span data-ttu-id="83afe-107">Hinzufügen von Bildern</span><span class="sxs-lookup"><span data-stu-id="83afe-107">Adding images</span></span>

<span data-ttu-id="83afe-108">Bilder können mittels URL-Verweis oder durch das Senden von Rohdaten hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="83afe-108">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="83afe-109">Microsoft Graph unterstützt die folgenden Methoden zum Hinzufügen von Bildern, Logos und Fotos zu OneNote-Seiten:</span><span class="sxs-lookup"><span data-stu-id="83afe-109">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="83afe-110">Hinzufügen öffentlicher Bilder aus dem Internet</span><span class="sxs-lookup"><span data-stu-id="83afe-110">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)  
<span data-ttu-id="83afe-111">Verwenden Sie `img` mit `src="http://image-url"`, und geben Sie die URL eines öffentlich zugänglichen Bilds an.</span><span class="sxs-lookup"><span data-stu-id="83afe-111">Use `img` with `src="http://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="83afe-112">Das Bild wird auf der OneNote-Seite gerendert.</span><span class="sxs-lookup"><span data-stu-id="83afe-112">Renders the image on the OneNote page.</span></span></p>
[<span data-ttu-id="83afe-113">Hinzufügen von Bildern mithilfe von Binärdaten</span><span class="sxs-lookup"><span data-stu-id="83afe-113">Add an image using binary data</span></span>](#add-an-image-using-binary-data)</p>
<span data-ttu-id="83afe-114">Verwenden Sie `img` mit `src="name:image-block-name"`, und senden Sie die Bilddatei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83afe-114">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="83afe-115">Das Bild wird auf der OneNote-Seite gerendert.</span><span class="sxs-lookup"><span data-stu-id="83afe-115">Renders the image on the OneNote page.</span></span></p>
[<span data-ttu-id="83afe-116">Hinzufügen von Webseitenmomentaufnahmen</span><span class="sxs-lookup"><span data-stu-id="83afe-116">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)</p>
<span data-ttu-id="83afe-117">Verwenden Sie `img` mit `data-render-src="http://webpage-url"`, und geben Sie die URL einer Webseite an.</span><span class="sxs-lookup"><span data-stu-id="83afe-117">Use `img` with `data-render-src="http://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="83afe-118">Auf der OneNote-Seite wird eine Momentaufnahme der gesamten Webseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="83afe-118">Renders a snapshot of the whole webpage on the OneNote page.</span></span></p>
[<span data-ttu-id="83afe-119">Hinzufügen von HTML-basiert gerenderten Bildern</span><span class="sxs-lookup"><span data-stu-id="83afe-119">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)</p>
<span data-ttu-id="83afe-120">Verwenden Sie `img` mit `data-render-src="name:html-block-name"`, und senden Sie HTML-Code in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83afe-120">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="83afe-121">Der HTML-Code wird auf der OneNote-Seite als Bild gerendert.</span><span class="sxs-lookup"><span data-stu-id="83afe-121">Renders the HTML as an image on the OneNote page.</span></span></p>
[<span data-ttu-id="83afe-122">Hinzufügen von Bildern von PDF-Inhalten</span><span class="sxs-lookup"><span data-stu-id="83afe-122">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)</p>
<span data-ttu-id="83afe-123">Verwenden Sie `<img data-render-src="name:part-name" />`, und senden Sie die PDF-Datei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83afe-123">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="83afe-124">Jede PDF-Seite wird auf der OneNote-Seite als separates Bild gerendert.</span><span class="sxs-lookup"><span data-stu-id="83afe-124">Renders each PDF page as a separate image on the OneNote page.</span></span></p>
[<span data-ttu-id="83afe-125">Hinzufügen von Bilddateien als Dateianlage</span><span class="sxs-lookup"><span data-stu-id="83afe-125">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)</p>
<span data-ttu-id="83afe-126">Verwenden Sie `object` mit `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"`, und senden Sie eine Bilddatei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83afe-126">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="83afe-127">Der OneNote-Seite wird eine Dateianlage hinzugefügt, und es wird ein Dateisymbol angezeigt.</span><span class="sxs-lookup"><span data-stu-id="83afe-127">Adds a file attachment to the OneNote page and displays a file icon.</span></span></p>

> <span data-ttu-id="83afe-128">**Hinweis:** Zum Abrufen von Bildern auf einer OneNote-Seite müssen Sie zunächst die [Seiteninhalte per GET-Anforderung abrufen](onenote-get-content.md#page-html-content).</span><span class="sxs-lookup"><span data-stu-id="83afe-128">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="83afe-129">Das gibt die URLs der Bildressourcen auf der Seite zurück.</span><span class="sxs-lookup"><span data-stu-id="83afe-129">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="83afe-130">Dann senden Sie separat [eine GET-Anforderung je Bildressource](onenote-get-content.md#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="83afe-130">Then you separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


<span data-ttu-id="83afe-131">**Bildattribute**</span><span class="sxs-lookup"><span data-stu-id="83afe-131">**Image attributes**</span></span> 

<span data-ttu-id="83afe-132">Elemente des Typs **img** können optional Attribute der Typen **alt**, **height** und **width** enthalten sowie die Formatattribute **max-width** und **max-height**.</span><span class="sxs-lookup"><span data-stu-id="83afe-132">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

<span data-ttu-id="83afe-133">**Bildmedientypen**</span><span class="sxs-lookup"><span data-stu-id="83afe-133">**Image media types**</span></span>

<span data-ttu-id="83afe-134">Microsoft Graph unterstützt die Bildtypen TIFF, PNG, GIF, JPEG und BMP.</span><span class="sxs-lookup"><span data-stu-id="83afe-134">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="83afe-135">Soll ein anderes Bildformat ohne vorherige Konvertierung dargestellt werden, müssen Sie [die Binärdaten senden](#add-an-image-using-binary-data), in einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83afe-135">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="83afe-136">Base64 muss nicht verwendet werden, und auch eine anderweitige Codierung der gesendeten Binärdaten ist nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="83afe-136">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="83afe-137">**Hinweis:** Die API erkennt den ursprünglichen Eingabebildtyp und gibt ihn als Attribut **data-fullres-src-type** im [Ausgabe-HTML-Code](onenote_input_output_html.md#output-html) zurück.</span><span class="sxs-lookup"><span data-stu-id="83afe-137">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="83afe-138">Daneben gibt die API auch den Bildtyp des optimierten Bilds zurück, in **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="83afe-138">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="83afe-139">Unter [Einschränkungen](#size-limitations-for-post-pages-requests) sind alle Einschränkungen aufgeführt, die bei der Erstellung von Seiten mit Medien gelten.</span><span class="sxs-lookup"><span data-stu-id="83afe-139">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>
### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="83afe-140">Hinzufügen öffentlicher Bilder aus dem Internet</span><span class="sxs-lookup"><span data-stu-id="83afe-140">Add a public image from the web</span></span>

<span data-ttu-id="83afe-141">Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<img src="http://..." />` an, und setzen Sie die URL eines öffentlich verfügbaren Bilds im Attribut **src**.</span><span class="sxs-lookup"><span data-stu-id="83afe-141">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Public URL</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image from the web.</p>
    <img src="http://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>
### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="83afe-142">Hinzufügen von Bildern mithilfe von Binärdaten</span><span class="sxs-lookup"><span data-stu-id="83afe-142">Add an image using binary data</span></span>

<span data-ttu-id="83afe-143">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img src="name:part-name" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Bilddaten enthält.</span><span class="sxs-lookup"><span data-stu-id="83afe-143">In the input HTML of your request's **Presentation** part, include  `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="83afe-144">Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.</span><span class="sxs-lookup"><span data-stu-id="83afe-144">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Image binary data</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the uploaded image.</p>
    <img src="name:image-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="MyAppPictureId"
Content-Type: image/jpeg

... image binary data ...

--MyAppPartBoundary--  
```


<a name="image-img-url-data-render-src"></a>
### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="83afe-145">Hinzufügen von Webseitenmomentaufnahmen</span><span class="sxs-lookup"><span data-stu-id="83afe-145">Add a webpage snapshot</span></span>

<span data-ttu-id="83afe-146">Sie können mit Microsoft Graph Momentaufnahmen ganzer Webseiten erstellen und in neue Seiten einfügen.</span><span class="sxs-lookup"><span data-stu-id="83afe-146">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="83afe-147">Diese Methode ist nützlich, um Webseiten zu archivieren oder komplexe Webseiten mit Features abzubilden, die OneNote nicht unterstützt (beispielsweise bestimmte CSS-Formatierungen).</span><span class="sxs-lookup"><span data-stu-id="83afe-147">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="83afe-148">Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<img src="http://..." />` an, und setzen Sie die URL der einzufügenden Webseite im Attribut **src**.</span><span class="sxs-lookup"><span data-stu-id="83afe-148">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Webpage capture</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image of the webpage.</p>
    <img data-render-src="http://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>
### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="83afe-149">Hinzufügen von HTML-basiert gerenderten Bildern</span><span class="sxs-lookup"><span data-stu-id="83afe-149">Add an image rendered from HTML</span></span>
<span data-ttu-id="83afe-150">Wenn Sie den HTML-Code als Datenblock übergeben, dürfen darin weder aktive Inhalte enthalten sein, die Benutzeranmeldeinformationen erfordern, noch vorab geladene Browser-Plug-Ins.</span><span class="sxs-lookup"><span data-stu-id="83afe-150">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="83afe-151">Das Modul, das Microsoft Graph verwendet, um die HTML-Seite als Bild zu rendern, kann Benutzer nicht anmelden und enthält keine Plug-Ins wie Adobe Flash oder Apple QuickTime.</span><span class="sxs-lookup"><span data-stu-id="83afe-151">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so-on.</span></span> <span data-ttu-id="83afe-152">Das bedeutet außerdem: Dynamisch geladene Inhalte, beispielsweise in einem AJAX-Skript, werden nicht angezeigt, wenn zum Abrufen der Daten Benutzeranmeldeinformationen oder Cookies erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="83afe-152">That also means that dynamically-loaded content, like might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="83afe-153">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img data-render-src="name:part-name" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der den HTML-Code enthält.</span><span class="sxs-lookup"><span data-stu-id="83afe-153">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: HTML block</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the block of HTML as an image.</p>
    <img data-render-src="name:html-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="html-block-name"
Content-Type: text/html

<html>
<body>
<h1>This HTML will render as an image</h1>
<p><b>Don't</b> try to embed another <i>data-render-src</i> type-image inside the HTML part--
it won't work. Instead, use URL-based real images like this:</p>
<img src="http://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>
### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="83afe-154">Hinzufügen von Bilddateien als Anlage</span><span class="sxs-lookup"><span data-stu-id="83afe-154">Add an image file as an attachment</span></span>

<span data-ttu-id="83afe-155">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Bilddaten enthält.</span><span class="sxs-lookup"><span data-stu-id="83afe-155">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="83afe-156">Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.</span><span class="sxs-lookup"><span data-stu-id="83afe-156">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Binary image data as file attachment</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page contains the image as a file attachment.</p>
    <object data-attachment="image-file.jpg" data="name:image-block-name" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```

<span data-ttu-id="83afe-157">Weitere Informationen zu Dateimedientypen finden Sie unter [diesem Link](#file-media-types).</span><span class="sxs-lookup"><span data-stu-id="83afe-157">Learn more about [file media types](#file-media-types).</span></span>



<a name="videos"></a>
## <a name="adding-videos"></a><span data-ttu-id="83afe-158">Hinzufügen von Videos</span><span class="sxs-lookup"><span data-stu-id="83afe-158">Adding videos</span></span>

<span data-ttu-id="83afe-159">Wenn Sie Videos in OneNote-Seiten einbetten möchten, können Sie `<iframe data-original-src="http://..." />` im Eingabe-HTML-Code verwenden.</span><span class="sxs-lookup"><span data-stu-id="83afe-159">You can embed videos in OneNote pages using `<iframe data-original-src="http://..." />` in the input HTML.</span></span> 

<span data-ttu-id="83afe-160">**Unterstützte Videowebsites**</span><span class="sxs-lookup"><span data-stu-id="83afe-160">**Supported video sites**</span></span>

- <span data-ttu-id="83afe-161">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="83afe-161">Dailymotion</span></span>
- <span data-ttu-id="83afe-162">Office Mix</span><span class="sxs-lookup"><span data-stu-id="83afe-162">Office Mix</span></span>
- <span data-ttu-id="83afe-163">Sway</span><span class="sxs-lookup"><span data-stu-id="83afe-163">Sway</span></span>
- <span data-ttu-id="83afe-164">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="83afe-164">Sketchfab</span></span>
- <span data-ttu-id="83afe-165">TED</span><span class="sxs-lookup"><span data-stu-id="83afe-165">TED</span></span>
- <span data-ttu-id="83afe-166">YouTube</span><span class="sxs-lookup"><span data-stu-id="83afe-166">YouTube</span></span>
- <span data-ttu-id="83afe-167">Vimeo</span><span class="sxs-lookup"><span data-stu-id="83afe-167">Vimeo</span></span>
- <span data-ttu-id="83afe-168">Vine</span><span class="sxs-lookup"><span data-stu-id="83afe-168">Vine</span></span>

<span data-ttu-id="83afe-169">**„iframe“-Attribute**</span><span class="sxs-lookup"><span data-stu-id="83afe-169">**iframe attributes**</span></span>

<span data-ttu-id="83afe-170">**data-original-src**</span><span class="sxs-lookup"><span data-stu-id="83afe-170">**data-original-src**</span></span></p>
<span data-ttu-id="83afe-171">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="83afe-171">Required.</span></span> <span data-ttu-id="83afe-172">URL des Videos.</span><span class="sxs-lookup"><span data-stu-id="83afe-172">The URL of the video source.</span></span><br /><span data-ttu-id="83afe-173">Beispiel: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="83afe-173">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span></p>
<span data-ttu-id="83afe-174">**width**</span><span class="sxs-lookup"><span data-stu-id="83afe-174">**width**</span></span></p>
<span data-ttu-id="83afe-175">Optional.</span><span class="sxs-lookup"><span data-stu-id="83afe-175">Optional.</span></span> <span data-ttu-id="83afe-176">Breite des „iframe“-Elements, in dem das Video enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="83afe-176">The width of the iframe that contains the video.</span></span> <span data-ttu-id="83afe-177">Der Standardwert ist 480.</span><span class="sxs-lookup"><span data-stu-id="83afe-177">Default is 480.</span></span><br /><span data-ttu-id="83afe-178">Beispiel: `width="300"`</span><span class="sxs-lookup"><span data-stu-id="83afe-178">Example: `width="300"`</span></span></p>
<span data-ttu-id="83afe-179">**height**</span><span class="sxs-lookup"><span data-stu-id="83afe-179">**height**</span></span></p>
<span data-ttu-id="83afe-180">Optional.</span><span class="sxs-lookup"><span data-stu-id="83afe-180">Optional.</span></span> <span data-ttu-id="83afe-181">Höhe des „iframe“-Elements, in dem das Video enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="83afe-181">The height of the iframe that contains the video.</span></span> <span data-ttu-id="83afe-182">Der Standardwert ist 360.</span><span class="sxs-lookup"><span data-stu-id="83afe-182">Default is 360.</span></span><br /><span data-ttu-id="83afe-183">Beispiel: `height="300"`</span><span class="sxs-lookup"><span data-stu-id="83afe-183">Example: `height="300"`</span></span></p>

<span data-ttu-id="83afe-184">**Beispiel**</span><span class="sxs-lookup"><span data-stu-id="83afe-184">**Example**</span></span>

<span data-ttu-id="83afe-185">Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<iframe data-original-src="http://..." />` an, und setzen Sie die URL des Videos im Attribut **data-original-src**.</span><span class="sxs-lookup"><span data-stu-id="83afe-185">In the input HTML of your request, include `<iframe data-original-src="http://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
    <head>
        <title>A page with an embedded video</title>
    </head>
    <body>
        <iframe data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" width="340" height="280"/>
    </body>
</html>

--MyAppPartBoundary--
```


<a name="files"></a>
## <a name="adding-files"></a><span data-ttu-id="83afe-186">Hinzufügen von Dateien</span><span class="sxs-lookup"><span data-stu-id="83afe-186">Adding installation files</span></span>

<span data-ttu-id="83afe-187">Zum Hinzufügen von Dateianlagen zu OneNote-Seiten verwenden Sie ein Element des Typs **object** im Eingabe-HTML-Code.</span><span class="sxs-lookup"><span data-stu-id="83afe-187">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="83afe-188">Wenn Sie eine PDF-Datei hinzufügen möchten, können Sie die einzelnen PDF-Seiten mithilfe eines Elements des Typs **img** als Bild rendern.</span><span class="sxs-lookup"><span data-stu-id="83afe-188">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="83afe-189">Hinzufügen von Dateianlagen</span><span class="sxs-lookup"><span data-stu-id="83afe-189">Add a file attachment</span></span>](#add-a-file-attachment)</p>
<span data-ttu-id="83afe-190">Verwenden Sie `<object .../>`, und senden Sie die Datei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83afe-190">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="83afe-191">Der OneNote-Seite wird eine Dateianlage hinzugefügt, die als Dateisymbol angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="83afe-191">Adds a file attachment that displays a file icon on the OneNote page.</span></span></p>
[<span data-ttu-id="83afe-192">Hinzufügen von Bildern von PDF-Inhalten</span><span class="sxs-lookup"><span data-stu-id="83afe-192">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)</p>
<span data-ttu-id="83afe-193">Verwenden Sie `<img data-render-src="name:part-name" />`, und senden Sie eine PDF-Datei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83afe-193">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="83afe-194">Jede PDF-Seite wird auf der OneNote-Seite als separates Bild gerendert.</span><span class="sxs-lookup"><span data-stu-id="83afe-194">Renders each PDF page as a separate image on the OneNote page.</span></span></p>

<span data-ttu-id="83afe-195">**Dateiattribute**</span><span class="sxs-lookup"><span data-stu-id="83afe-195">**File attributes**</span></span>

<span data-ttu-id="83afe-196">Elemente des Typs **object** erfordern die folgenden Attribute:</span><span class="sxs-lookup"><span data-stu-id="83afe-196">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="83afe-197">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="83afe-197">**data-attachment**</span></span></p>
<span data-ttu-id="83afe-198">Name und Dateierweiterung der Datei, die auf der OneNote-Seite angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="83afe-198">The file name and extension to display on the OneNote page.</span></span><br /><span data-ttu-id="83afe-199">Beispiel: `data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="83afe-199">Example: `data-attachment="filename.docx"`</span></span></p>
<span data-ttu-id="83afe-200">**data**</span><span class="sxs-lookup"><span data-stu-id="83afe-200">**Data**</span></span></p>
<span data-ttu-id="83afe-201">Name des Textteils in der mehrteiligen Anforderung, der die binären Dateidaten enthält.</span><span class="sxs-lookup"><span data-stu-id="83afe-201">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="83afe-202">Microsoft Graph bietet keine Unterstützung für die Übergabe von URL-Verweisen in diesem Attribut.</span><span class="sxs-lookup"><span data-stu-id="83afe-202">Microsoft Graph does not support passing a URL reference here.</span></span><br /><span data-ttu-id="83afe-203">Beispiel: `data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="83afe-203">Example: `data="name:part-name"`</span></span></p>
<span data-ttu-id="83afe-204">**type**</span><span class="sxs-lookup"><span data-stu-id="83afe-204">**type**</span></span></p>
<span data-ttu-id="83afe-205">Medientyp der Datei. Er legt fest, welches Dateisymbol auf der Seite angezeigt werden soll und welche Anwendung gestartet wird, sobald der Benutzer die Datei auf dem Gerät über OneNote aktiviert.</span><span class="sxs-lookup"><span data-stu-id="83afe-205">type="standardMimeType" indicates the file MIME type. This is used to select the file icon on the page, and also determines which application starts when the user activates the file on the device from OneNote.</span></span><br /><span data-ttu-id="83afe-206">Beispiel: `type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="83afe-206">Example: `type="application/pdf"`</span></span></p>


<a name="file-media-types"></a>

### <a name="file-media-types"></a><span data-ttu-id="83afe-207">Dateimedientypen</span><span class="sxs-lookup"><span data-stu-id="83afe-207">File media types</span></span>  
<span data-ttu-id="83afe-208">Microsoft Graph verwendet für angefügte Dateien vordefinierte Dateitypensymbole. Erkennt die API den Dateityp nicht, wird ein generisches Symbol verwendet.</span><span class="sxs-lookup"><span data-stu-id="83afe-208">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="83afe-209">Nachfolgend sind verschiedene häufig vorkommende Dateitypen aufgeführt, die von der API erkannt werden:</span><span class="sxs-lookup"><span data-stu-id="83afe-209">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="83afe-210">application/pdf</span><span class="sxs-lookup"><span data-stu-id="83afe-210">application/pdf</span></span>  
- <span data-ttu-id="83afe-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="83afe-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="83afe-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="83afe-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="83afe-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="83afe-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="83afe-214">image/png</span><span class="sxs-lookup"><span data-stu-id="83afe-214">image/png</span></span>
- <span data-ttu-id="83afe-215">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="83afe-215">image/jpeg</span></span>
- <span data-ttu-id="83afe-216">image/gif</span><span class="sxs-lookup"><span data-stu-id="83afe-216">image/gif</span></span>
- <span data-ttu-id="83afe-217">audio/wav</span><span class="sxs-lookup"><span data-stu-id="83afe-217">audio/wav</span></span>
- <span data-ttu-id="83afe-218">video/mp4</span><span class="sxs-lookup"><span data-stu-id="83afe-218">video/mp4</span></span>
- <span data-ttu-id="83afe-219">application/msword</span><span class="sxs-lookup"><span data-stu-id="83afe-219">application/msword</span></span>
- <span data-ttu-id="83afe-220">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="83afe-220">application/mspowerpoint</span></span>
- <span data-ttu-id="83afe-221">application/excel</span><span class="sxs-lookup"><span data-stu-id="83afe-221">application/excel</span></span>

<span data-ttu-id="83afe-222">Unter [Einschränkungen](#size-limitations-for-post-pages-requests) sind alle Einschränkungen aufgeführt, die bei der Erstellung von Seiten mit Medien gelten.</span><span class="sxs-lookup"><span data-stu-id="83afe-222">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>
### <a name="add-a-file-attachment"></a><span data-ttu-id="83afe-223">Hinzufügen von Dateianlagen</span><span class="sxs-lookup"><span data-stu-id="83afe-223">Add a file attachment</span></span>

<span data-ttu-id="83afe-224">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Dateidaten enthält.</span><span class="sxs-lookup"><span data-stu-id="83afe-224">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="83afe-225">Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.</span><span class="sxs-lookup"><span data-stu-id="83afe-225">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image file attachment</title>
  </head>
  <body>
    <p>This is an image file attachment.</p>
    <object data-attachment="Logo.jpg" data="name:logo1-file" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```


<a name="file-binary-data-render-src"></a>
### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="83afe-226">Hinzufügen von Bildern von PDF-Inhalten</span><span class="sxs-lookup"><span data-stu-id="83afe-226">Add images of PDF file contents</span></span>

<span data-ttu-id="83afe-227">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img data-render-src="name:part-name" ... />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Dateidaten enthält.</span><span class="sxs-lookup"><span data-stu-id="83afe-227">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="83afe-228">Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.</span><span class="sxs-lookup"><span data-stu-id="83afe-228">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with images of the pages of a PDF file</title>
  </head>
  <body>
    <p>The pages of this PDF file render as images.</p>
    <img data-render-src="name:file-part" alt="PDF file as images" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="file-part"
Content-Type: application/pdf

... binary file data ...

--MyAppPartBoundary--  
```


<a name="size-limits"></a>
## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="83afe-229">Größenbeschränkungen bei Anforderungen des Typs „Post pages“</span><span class="sxs-lookup"><span data-stu-id="83afe-229">Size limitations for POST pages requests</span></span>

<span data-ttu-id="83afe-230">Für das Senden von Bild- und Dateidaten gelten folgende Einschränkungen: <!--TODO: check these--></span><span class="sxs-lookup"><span data-stu-id="83afe-230">When sending image and file data, be aware of these limitations: <!--TODO: check these--></span></span>

- <span data-ttu-id="83afe-231">Die maximal zulässige Gesamtgröße von POST-Anforderungen liegt bei etwa 70 MB, einschließlich Bildern, Dateien und anderer Daten.</span><span class="sxs-lookup"><span data-stu-id="83afe-231">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="83afe-232">Das tatsächlich Limit hängt von der Downstreamcodierung ab, daher ist keine feste Bytezahl als Höchstgrenze gesetzt.</span><span class="sxs-lookup"><span data-stu-id="83afe-232">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="83afe-233">Anforderungen, die das Limit überschreiten, geben möglicherweise unzuverlässige Ergebnisse zurück.</span><span class="sxs-lookup"><span data-stu-id="83afe-233">Requests that exceed the limit may produce unreliable results.</span></span>

- <span data-ttu-id="83afe-234">Die maximal zulässige Größe pro Datenteil liegt bei 25 MB, einschließlich des Headers des jeweiligen Teils.</span><span class="sxs-lookup"><span data-stu-id="83afe-234">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="83afe-235">Datenteile, die dieses Limit überschreiten, werden von Microsoft Graph abgelehnt.</span><span class="sxs-lookup"><span data-stu-id="83afe-235">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="83afe-236">Die maximal zulässige Anzahl von Bildern pro Seite beträgt 150.</span><span class="sxs-lookup"><span data-stu-id="83afe-236">The maximum number of images per page is 150.</span></span> <span data-ttu-id="83afe-237">Bei Verwendung des Attributs `src="http://..."` ignoriert die API alle Tags des Typs **img**, die über dieses Limit hinausgehen.</span><span class="sxs-lookup"><span data-stu-id="83afe-237">Image limit is 150 per page. When using the **src="internetURL"`src="http://..."` attribute, the API ignores <img>** tags beyond the limit.</span></span>

- <span data-ttu-id="83afe-238">Die maximal zulässige Anzahl von Datenteilen pro POST-Anforderung liegt bei 6, einschließlich des zwingend erforderlichen Teils **Presentation**.</span><span class="sxs-lookup"><span data-stu-id="83afe-238">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="83afe-239">Jede Anforderung darf bis zu 5 Elemente des Typs **img** enthalten, die **data-render-src** verwenden, sowie 1 Element des Typs **object**, das **data-render-src** verwendet. Alle weiteren Bild- und Dateiverweise werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="83afe-239">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="83afe-240">Die maximal zulässige Anzahl von Bildern pro POST-Anforderung liegt bei 30, unabhängig von der Methode, über die sie an die API gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="83afe-240">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="83afe-241">Alle weiteren Bilder werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="83afe-241">Additional images are ignored.</span></span> <span data-ttu-id="83afe-242">Wenn Sie eine Webseite mit vielen Bildern abbilden möchten, empfiehlt sich die [Erstellung einer Momentaufnahme der gesamten Seite](#add-a-webpage-snapshot).</span><span class="sxs-lookup"><span data-stu-id="83afe-242">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="83afe-243">Anwendungsfälle: HTML vs. *data-render-src*</span><span class="sxs-lookup"><span data-stu-id="83afe-243">When to use HTML versus *data-render-src*</span></span> 
<span data-ttu-id="83afe-244">Ob Sie den HTML-Code direkt auf der OneNote-Seite einfügen oder das Attribut **data-render-src** verwenden sollten, hängt von verschiedenen Faktoren ab. Berücksichtigen Sie bei Ihrer Entscheidung Folgendes:</span><span class="sxs-lookup"><span data-stu-id="83afe-244">When trying to decide between directly putting HTML onto the OneNote page, versus using the data-render-src rendering, consider the following:</span></span>

- <span data-ttu-id="83afe-245">Komplexer HTML-Code sollte per **data-render-src** an das Renderingmodul gesendet werden. Eine manuelle Anpassung des HTML-Codes an die Anforderungen von Microsoft Graph empfiehlt sich nicht.</span><span class="sxs-lookup"><span data-stu-id="83afe-245">Complex HTML is probably best sent to the rendering engine via data-render-src, rather than attempting to modify the HTML to fit into what the oncshort API can accept. This is also true when your HTML includes tags not yet supported (see ).</span></span> <span data-ttu-id="83afe-246">Dies gilt auch für HTML-Code mit nicht unterstützten Tags.</span><span class="sxs-lookup"><span data-stu-id="83afe-246">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="83afe-247">Für akkurates Seitenrendering unter Beibehaltung des Layouts und Designs der Seite empfiehlt sich die Verwendung des Renderingmoduls per **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="83afe-247">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="83afe-248">Bei direkt bearbeitbarem Text sollte der HTML-Code direkt auf der Seite eingefügt werden.</span><span class="sxs-lookup"><span data-stu-id="83afe-248">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span> <span data-ttu-id="83afe-249">Gerenderte Bilder werden zwar von einem System für optische Zeichenerkennung (OCR, Optical Character Recognition) gescannt, dieses System liefert jedoch keine gleichwertigen Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="83afe-249">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="83afe-250">Momentaufnahmen bestimmter Zeitpunkte zu Verlaufs- oder Archivierungszwecken sollten mithilfe der Methode „data-render-src“ angefertigt werden.</span><span class="sxs-lookup"><span data-stu-id="83afe-250">Snapshot-in-time for historical or archival purposes is usually best done with the data-render-src method.</span></span>

- <span data-ttu-id="83afe-251">**data-render-src** eignet sich hervorragend, um einem Webseitendesign Überarbeitungshinweise hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="83afe-251">Marking-up a web page design for revisions is one place the **data-render-src** truly shines.</span></span> <span data-ttu-id="83afe-252">Mit den Freihandfunktionen von OneNote können Sie Änderungen auf dem Bild markieren oder wichtige Bereiche hervorheben.</span><span class="sxs-lookup"><span data-stu-id="83afe-252">Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas.</span></span> <span data-ttu-id="83afe-253">Ist die betreffende Webseite ein Bild, gestaltet sich das sehr viel einfacher.</span><span class="sxs-lookup"><span data-stu-id="83afe-253">Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="83afe-254">Sehr große Bilder oder Bilder in Formaten, die OneNote nicht direkt unterstützt, lassen sich mit dem Attribut **data-render-src** mitunter einfacher als Miniaturansicht anzeigen und konvertieren, als dies mit eigenem Code möglich wäre.</span><span class="sxs-lookup"><span data-stu-id="83afe-254">Very large images, or images in formats that OneNote doesn't directly accept can sometimes be thumbnailed and converted with the data-render-src method more easily than by doing it in your own code.</span></span> <span data-ttu-id="83afe-255">Selbst wenn das Bild auch online verfügbar ist: Wenn Sie die Daten in die POST-Anforderung einbetten, steht die Seitenabbildung OneNote-Benutzern manchmal schneller zur Verfügung, da zur Erstellung der OneNote-Seite insgesamt weniger Roundtrips nötig sind.</span><span class="sxs-lookup"><span data-stu-id="83afe-255">You can also send the image data for up to 150 images directly inside the oncshort API POST. This is common when the images are from a mobile device camera, or if your app is running on a hardware device like a scanner or camera. Even if the image is also available on the Internet, embedding the data in your POST can sometimes make the captured page available to OneNote user sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="83afe-256">Manchmal können Sie am einfachsten herausfinden, welche Methode für Ihre Benutzer die beste ist, indem sie während der App-Entwicklung beide Varianten testen.</span><span class="sxs-lookup"><span data-stu-id="83afe-256">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="83afe-257">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="83afe-257">Permissions</span></span>

<span data-ttu-id="83afe-258">Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="83afe-258">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="83afe-259">Wählen Sie die niedrigste Stufe, die erforderlich ist, damit Ihre App korrekt funktioniert.</span><span class="sxs-lookup"><span data-stu-id="83afe-259">Choose the lowest level that your app needs to do its work.</span></span>

<span data-ttu-id="83afe-260">**Berechtigungen für _POST pages_**</span><span class="sxs-lookup"><span data-stu-id="83afe-260">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="83afe-261">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="83afe-261">Notes.Create</span></span>
- <span data-ttu-id="83afe-262">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83afe-262">Notes.ReadWrite</span></span>
- <span data-ttu-id="83afe-263">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83afe-263">Notes.ReadWrite.All</span></span> 

<span data-ttu-id="83afe-264">**Berechtigungen für _PATCH pages_**</span><span class="sxs-lookup"><span data-stu-id="83afe-264">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="83afe-265">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83afe-265">Notes.ReadWrite</span></span>
- <span data-ttu-id="83afe-266">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83afe-266">Notes.ReadWrite.All</span></span>

<span data-ttu-id="83afe-267">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie im Artikel zum Thema [OneNote-Berechtigungsbereiche](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="83afe-267">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="83afe-268">Weitere Ressourcen</span><span class="sxs-lookup"><span data-stu-id="83afe-268">Additional resources</span></span>

- [<span data-ttu-id="83afe-269">Integrieren mit OneNote</span><span class="sxs-lookup"><span data-stu-id="83afe-269">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="83afe-270">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="83afe-270">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="83afe-271">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="83afe-271">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="83afe-272">GitHub-Repositorys für OneNote</span><span class="sxs-lookup"><span data-stu-id="83afe-272">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
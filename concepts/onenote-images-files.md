---
title: Hinzufügen von Bildern, Videos und Dateien zu OneNote-Seiten
description: " Enterprise-Notizbücher in Office 365"
ms.openlocfilehash: bc298339d73b162da6b2e37c314ffedfb76bd193
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092218"
---
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="61b61-103">Hinzufügen von Bildern, Videos und Dateien zu OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="61b61-103">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="61b61-104">**Gilt für** Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365</span><span class="sxs-lookup"><span data-stu-id="61b61-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="61b61-105">Sie können Elemente der Typen **img**, **object** und **iframe** verwenden, um bei der [Erstellung](onenote-create-page.md) oder [Aktualisierung](onenote-update-page.md) von OneNote-Seiten Bilder, Videos und Dateien zur Seite hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="61b61-105">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote-update-page.md) the page.</span></span> 

- <span data-ttu-id="61b61-106">Verwenden Sie **img**, um ein Bild auf der Seite zu rendern.</span><span class="sxs-lookup"><span data-stu-id="61b61-106">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="61b61-107">Verwenden Sie **iframe**, um ein Video in die Seite einzubetten.</span><span class="sxs-lookup"><span data-stu-id="61b61-107">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="61b61-108">Verwenden Sie **object**, um der Seite eine Dateianlage hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="61b61-108">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>

## <a name="adding-images"></a><span data-ttu-id="61b61-109">Hinzufügen von Bildern</span><span class="sxs-lookup"><span data-stu-id="61b61-109">Adding images</span></span>

<span data-ttu-id="61b61-110">Bilder können mittels URL-Verweis oder durch das Senden von Rohdaten hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="61b61-110">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="61b61-111">Microsoft Graph unterstützt die folgenden Methoden zum Hinzufügen von Bildern, Logos und Fotos zu OneNote-Seiten:</span><span class="sxs-lookup"><span data-stu-id="61b61-111">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="61b61-112">Hinzufügen öffentlicher Bilder aus dem Internet</span><span class="sxs-lookup"><span data-stu-id="61b61-112">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)

<span data-ttu-id="61b61-113">Verwenden Sie `img` mit `src="https://image-url"`, und geben Sie die URL eines öffentlich zugänglichen Bilds an.</span><span class="sxs-lookup"><span data-stu-id="61b61-113">Use `img` with `src="https://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="61b61-114">Das Bild wird auf der OneNote-Seite gerendert.</span><span class="sxs-lookup"><span data-stu-id="61b61-114">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="61b61-115">Hinzufügen von Bildern mithilfe von Binärdaten</span><span class="sxs-lookup"><span data-stu-id="61b61-115">Add an image using binary data</span></span>](#add-an-image-using-binary-data)

<span data-ttu-id="61b61-116">Verwenden Sie `img` mit `src="name:image-block-name"`, und senden Sie die Bilddatei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61b61-116">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="61b61-117">Das Bild wird auf der OneNote-Seite gerendert.</span><span class="sxs-lookup"><span data-stu-id="61b61-117">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="61b61-118">Hinzufügen von Webseitenmomentaufnahmen</span><span class="sxs-lookup"><span data-stu-id="61b61-118">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)

<span data-ttu-id="61b61-119">Verwenden Sie `img` mit `data-render-src="https://webpage-url"`, und geben Sie die URL einer Webseite an.</span><span class="sxs-lookup"><span data-stu-id="61b61-119">Use `img` with `data-render-src="https://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="61b61-120">Auf der OneNote-Seite wird eine Momentaufnahme der gesamten Webseite gerendert.</span><span class="sxs-lookup"><span data-stu-id="61b61-120">Renders a snapshot of the whole webpage on the OneNote page.</span></span>

[<span data-ttu-id="61b61-121">Hinzufügen von HTML-basiert gerenderten Bildern</span><span class="sxs-lookup"><span data-stu-id="61b61-121">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)

<span data-ttu-id="61b61-122">Verwenden Sie `img` mit `data-render-src="name:html-block-name"`, und senden Sie HTML-Code in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61b61-122">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="61b61-123">Der HTML-Code wird auf der OneNote-Seite als Bild gerendert.</span><span class="sxs-lookup"><span data-stu-id="61b61-123">Renders the HTML as an image on the OneNote page.</span></span>

[<span data-ttu-id="61b61-124">Hinzufügen von Bildern von PDF-Inhalten</span><span class="sxs-lookup"><span data-stu-id="61b61-124">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="61b61-125">Verwenden Sie `<img data-render-src="name:part-name" />`, und senden Sie die PDF-Datei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61b61-125">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="61b61-126">Jede PDF-Seite wird auf der OneNote-Seite als separates Bild gerendert.</span><span class="sxs-lookup"><span data-stu-id="61b61-126">Renders each PDF page as a separate image on the OneNote page.</span></span>

[<span data-ttu-id="61b61-127">Hinzufügen von Bilddateien als Dateianlage</span><span class="sxs-lookup"><span data-stu-id="61b61-127">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)

<span data-ttu-id="61b61-128">Verwenden Sie `object` mit `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"`, und senden Sie eine Bilddatei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61b61-128">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="61b61-129">Der OneNote-Seite wird eine Dateianlage hinzugefügt, und es wird ein Dateisymbol angezeigt.</span><span class="sxs-lookup"><span data-stu-id="61b61-129">Adds a file attachment to the OneNote page and displays a file icon.</span></span>


> <span data-ttu-id="61b61-130">**Hinweis:** Zum Abrufen von Bildern auf einer OneNote-Seite müssen Sie zunächst die [Seiteninhalte per GET-Anforderung abrufen](onenote-get-content.md#page-html-content).</span><span class="sxs-lookup"><span data-stu-id="61b61-130">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="61b61-131">Das gibt die URLs der Bildressourcen auf der Seite zurück.</span><span class="sxs-lookup"><span data-stu-id="61b61-131">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="61b61-132">Dann senden Sie separat [eine GET-Anforderung je Bildressource](onenote-get-content.md#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="61b61-132">You then separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


#### <a name="image-attributes"></a><span data-ttu-id="61b61-133">Attribute von Bildern</span><span class="sxs-lookup"><span data-stu-id="61b61-133">Image attributes</span></span> 

<span data-ttu-id="61b61-134">Elemente des Typs **img** können optional Attribute der Typen **alt**, **height** und **width** enthalten sowie die Formatattribute **max-width** und **max-height**.</span><span class="sxs-lookup"><span data-stu-id="61b61-134">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

#### <a name="image-media-types"></a><span data-ttu-id="61b61-135">Bildmedientypen</span><span class="sxs-lookup"><span data-stu-id="61b61-135">Image media types</span></span>

<span data-ttu-id="61b61-136">Microsoft Graph unterstützt die Bildtypen TIFF, PNG, GIF, JPEG und BMP.</span><span class="sxs-lookup"><span data-stu-id="61b61-136">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="61b61-137">Soll ein anderes Bildformat ohne vorherige Konvertierung dargestellt werden, müssen Sie [die Binärdaten senden](#add-an-image-using-binary-data), in einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61b61-137">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="61b61-138">Base64 muss nicht verwendet werden, und auch eine anderweitige Codierung der gesendeten Binärdaten ist nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61b61-138">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="61b61-139">**Hinweis:** Die API erkennt den ursprünglichen Eingabebildtyp und gibt ihn als Attribut **data-fullres-src-type** im [Ausgabe-HTML-Code](onenote-input-output-html.md#output-html) zurück.</span><span class="sxs-lookup"><span data-stu-id="61b61-139">**Note:** The API detects the original input image type, and returns it as the **data-fullres-src-type** attribute in the [output HTML](onenote-input-output-html.md#output-html).</span></span> <span data-ttu-id="61b61-140">Daneben gibt die API auch den Bildtyp des optimierten Bilds zurück, in **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="61b61-140">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="61b61-141">Unter [Einschränkungen](#size-limitations-for-post-pages-requests) sind alle Einschränkungen aufgeführt, die bei der Erstellung von Seiten mit Medien gelten.</span><span class="sxs-lookup"><span data-stu-id="61b61-141">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="61b61-142">Hinzufügen öffentlicher Bilder aus dem Internet</span><span class="sxs-lookup"><span data-stu-id="61b61-142">Add a public image from the web</span></span>

<span data-ttu-id="61b61-143">Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<img src="https://..." />` an, und setzen Sie die URL eines öffentlich verfügbaren Bilds im Attribut **src**.</span><span class="sxs-lookup"><span data-stu-id="61b61-143">In the input HTML of your request, include `<img src="https://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```html
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
    <img src="https://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>

### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="61b61-144">Hinzufügen von Bildern mithilfe von Binärdaten</span><span class="sxs-lookup"><span data-stu-id="61b61-144">Add an image using binary data</span></span>

<span data-ttu-id="61b61-145">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img src="name:part-name" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Bilddaten enthält.</span><span class="sxs-lookup"><span data-stu-id="61b61-145">In the input HTML of your request's **Presentation** part, include `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="61b61-146">Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.</span><span class="sxs-lookup"><span data-stu-id="61b61-146">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
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

### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="61b61-147">Hinzufügen von Webseitenmomentaufnahmen</span><span class="sxs-lookup"><span data-stu-id="61b61-147">Add a webpage snapshot</span></span>

<span data-ttu-id="61b61-148">Sie können mit Microsoft Graph Momentaufnahmen ganzer Webseiten erstellen und in neue Seiten einfügen.</span><span class="sxs-lookup"><span data-stu-id="61b61-148">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="61b61-149">Diese Methode ist nützlich, um Webseiten zu archivieren oder komplexe Webseiten mit Features abzubilden, die OneNote nicht unterstützt (beispielsweise bestimmte CSS-Formatierungen).</span><span class="sxs-lookup"><span data-stu-id="61b61-149">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="61b61-150">Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<img src="https://..." />` an, und setzen Sie die URL der einzufügenden Webseite im Attribut **src**.</span><span class="sxs-lookup"><span data-stu-id="61b61-150">In the input HTML of your request, include `<img src="https://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```html
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
    <img data-render-src="https://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>

### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="61b61-151">Hinzufügen von HTML-basiert gerenderten Bildern</span><span class="sxs-lookup"><span data-stu-id="61b61-151">Add an image rendered from HTML</span></span>

<span data-ttu-id="61b61-152">Wenn Sie den HTML-Code als Datenblock übergeben, dürfen darin weder aktive Inhalte enthalten sein, die Benutzeranmeldeinformationen erfordern, noch vorab geladene Browser-Plug-Ins.</span><span class="sxs-lookup"><span data-stu-id="61b61-152">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="61b61-153">Das Modul, das Microsoft Graph verwendet, um die HTML-Seite als Bild zu rendern, kann Benutzer nicht anmelden und enthält keine Plug-Ins wie Adobe Flash oder Apple QuickTime.</span><span class="sxs-lookup"><span data-stu-id="61b61-153">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so on.</span></span> <span data-ttu-id="61b61-154">Das bedeutet außerdem: Dynamisch geladene Inhalte, wie sie in einem AJAX-Skript vorkommen können, werden nicht angezeigt, wenn zum Abrufen der Daten Benutzeranmeldeinformationen oder Cookies erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="61b61-154">That also means that dynamically-loaded content, such as might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="61b61-155">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img data-render-src="name:part-name" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der den HTML-Code enthält.</span><span class="sxs-lookup"><span data-stu-id="61b61-155">In the input HTML of your request's **Presentation** part, include `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>


```html
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
<img src="https://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>

### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="61b61-156">Hinzufügen von Bilddateien als Anlage</span><span class="sxs-lookup"><span data-stu-id="61b61-156">Add an image file as an attachment</span></span>

<span data-ttu-id="61b61-157">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Bilddaten enthält.</span><span class="sxs-lookup"><span data-stu-id="61b61-157">In the input HTML of your request's **Presentation** part, include `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="61b61-158">Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.</span><span class="sxs-lookup"><span data-stu-id="61b61-158">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
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

<span data-ttu-id="61b61-159">Weitere Informationen zu Dateimedientypen finden Sie unter [diesem Link](#file-media-types).</span><span class="sxs-lookup"><span data-stu-id="61b61-159">Learn more about [file media types](#file-media-types).</span></span>



<a name="adding-videos"></a>

## <a name="adding-videos"></a><span data-ttu-id="61b61-160">Hinzufügen von Videos</span><span class="sxs-lookup"><span data-stu-id="61b61-160">Adding videos</span></span>

<span data-ttu-id="61b61-161">Wenn Sie Videos in OneNote-Seiten einbetten möchten, können Sie `<iframe data-original-src="https://..." />` im Eingabe-HTML-Code verwenden.</span><span class="sxs-lookup"><span data-stu-id="61b61-161">You can embed videos in OneNote pages using `<iframe data-original-src="https://..." />` in the input HTML.</span></span> 

### <a name="supported-video-sites"></a><span data-ttu-id="61b61-162">Unterstützte Videowebsites</span><span class="sxs-lookup"><span data-stu-id="61b61-162">Supported video sites</span></span>

- <span data-ttu-id="61b61-163">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="61b61-163">Dailymotion</span></span>
- <span data-ttu-id="61b61-164">Office Mix</span><span class="sxs-lookup"><span data-stu-id="61b61-164">Office Mix</span></span>
- <span data-ttu-id="61b61-165">Sway</span><span class="sxs-lookup"><span data-stu-id="61b61-165">Sway</span></span>
- <span data-ttu-id="61b61-166">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="61b61-166">Sketchfab</span></span>
- <span data-ttu-id="61b61-167">TED</span><span class="sxs-lookup"><span data-stu-id="61b61-167">TED</span></span>
- <span data-ttu-id="61b61-168">YouTube</span><span class="sxs-lookup"><span data-stu-id="61b61-168">YouTube</span></span>
- <span data-ttu-id="61b61-169">Vimeo</span><span class="sxs-lookup"><span data-stu-id="61b61-169">Vimeo</span></span>
- <span data-ttu-id="61b61-170">Vine</span><span class="sxs-lookup"><span data-stu-id="61b61-170">Vine</span></span>

### <a name="iframe-attributes"></a><span data-ttu-id="61b61-171">„iframe“-Attribute</span><span class="sxs-lookup"><span data-stu-id="61b61-171">iframe attributes</span></span>

#### <a name="data-original-src"></a><span data-ttu-id="61b61-172">data-original-src</span><span class="sxs-lookup"><span data-stu-id="61b61-172">data-original-src</span></span>

<span data-ttu-id="61b61-173">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="61b61-173">Required.</span></span> <span data-ttu-id="61b61-174">URL des Videos.</span><span class="sxs-lookup"><span data-stu-id="61b61-174">The URL of the video.</span></span>

<span data-ttu-id="61b61-175">Beispiel: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="61b61-175">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span>

#### <a name="width"></a><span data-ttu-id="61b61-176">width</span><span class="sxs-lookup"><span data-stu-id="61b61-176">width</span></span>

<span data-ttu-id="61b61-177">Optional.</span><span class="sxs-lookup"><span data-stu-id="61b61-177">Optional.</span></span> <span data-ttu-id="61b61-178">Breite des „iframe“-Elements, in dem das Video enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="61b61-178">The width of the iframe that contains the video.</span></span> <span data-ttu-id="61b61-179">Der Standardwert ist 480.</span><span class="sxs-lookup"><span data-stu-id="61b61-179">Default is 480.</span></span>

<span data-ttu-id="61b61-180">Beispiel: `width="300"`</span><span class="sxs-lookup"><span data-stu-id="61b61-180">Example: `width="300"`</span></span>

#### <a name="height"></a><span data-ttu-id="61b61-181">height</span><span class="sxs-lookup"><span data-stu-id="61b61-181">height</span></span>

<span data-ttu-id="61b61-182">Optional.</span><span class="sxs-lookup"><span data-stu-id="61b61-182">Optional.</span></span> <span data-ttu-id="61b61-183">Höhe des „iframe“-Elements, in dem das Video enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="61b61-183">The height of the iframe that contains the video.</span></span> <span data-ttu-id="61b61-184">Der Standardwert ist 360.</span><span class="sxs-lookup"><span data-stu-id="61b61-184">Default is 360.</span></span>

<span data-ttu-id="61b61-185">Beispiel: `height="300"`</span><span class="sxs-lookup"><span data-stu-id="61b61-185">Example: `height="300"`</span></span>

### <a name="example"></a><span data-ttu-id="61b61-186">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61b61-186">Example</span></span>

<span data-ttu-id="61b61-187">Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<iframe data-original-src="https://..." />` an, und setzen Sie die URL des Videos im Attribut **data-original-src**.</span><span class="sxs-lookup"><span data-stu-id="61b61-187">In the input HTML of your request, include `<iframe data-original-src="https://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```html
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


<a name="adding-files"></a>

## <a name="adding-files"></a><span data-ttu-id="61b61-188">Hinzufügen von Dateien</span><span class="sxs-lookup"><span data-stu-id="61b61-188">Adding files</span></span>

<span data-ttu-id="61b61-189">Zum Hinzufügen von Dateianlagen zu OneNote-Seiten verwenden Sie ein Element des Typs **object** im Eingabe-HTML-Code.</span><span class="sxs-lookup"><span data-stu-id="61b61-189">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="61b61-190">Wenn Sie eine PDF-Datei hinzufügen möchten, können Sie die einzelnen PDF-Seiten mithilfe eines Elements des Typs **img** als Bild rendern.</span><span class="sxs-lookup"><span data-stu-id="61b61-190">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="61b61-191">Hinzufügen von Dateianlagen</span><span class="sxs-lookup"><span data-stu-id="61b61-191">Add a file attachment</span></span>](#add-a-file-attachment)

<span data-ttu-id="61b61-192">Verwenden Sie `<object .../>`, und senden Sie die Datei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61b61-192">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="61b61-193">Der OneNote-Seite wird eine Dateianlage hinzugefügt, die als Dateisymbol angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="61b61-193">Adds a file attachment that displays a file icon on the OneNote page.</span></span>

[<span data-ttu-id="61b61-194">Hinzufügen von Bildern von PDF-Inhalten</span><span class="sxs-lookup"><span data-stu-id="61b61-194">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="61b61-195">Verwenden Sie `<img data-render-src="name:part-name" />`, und senden Sie eine PDF-Datei in einem Datenteil einer mehrteiligen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61b61-195">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="61b61-196">Jede PDF-Seite wird auf der OneNote-Seite als separates Bild gerendert.</span><span class="sxs-lookup"><span data-stu-id="61b61-196">Renders each PDF page as a separate image on the OneNote page.</span></span>

#### <a name="file-attributes"></a><span data-ttu-id="61b61-197">Dateiattribute</span><span class="sxs-lookup"><span data-stu-id="61b61-197">File attributes</span></span>

<span data-ttu-id="61b61-198">Elemente des Typs **object** erfordern die folgenden Attribute:</span><span class="sxs-lookup"><span data-stu-id="61b61-198">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="61b61-199">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="61b61-199">**data-attachment**</span></span>

<span data-ttu-id="61b61-200">Name und Dateierweiterung der Datei, die auf der OneNote-Seite angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="61b61-200">The file name and extension to display on the OneNote page.</span></span>

<span data-ttu-id="61b61-201">Beispiel: `data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="61b61-201">Example: `data-attachment="filename.docx"`</span></span>

<span data-ttu-id="61b61-202">**data**</span><span class="sxs-lookup"><span data-stu-id="61b61-202">**data**</span></span>

<span data-ttu-id="61b61-203">Name des Textteils in der mehrteiligen Anforderung, der die binären Dateidaten enthält.</span><span class="sxs-lookup"><span data-stu-id="61b61-203">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="61b61-204">Microsoft Graph bietet keine Unterstützung für die Übergabe von URL-Verweisen in diesem Attribut.</span><span class="sxs-lookup"><span data-stu-id="61b61-204">Microsoft Graph does not support passing a URL reference here.</span></span>

<span data-ttu-id="61b61-205">Beispiel: `data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="61b61-205">Example: `data="name:part-name"`</span></span>

<span data-ttu-id="61b61-206">**type**</span><span class="sxs-lookup"><span data-stu-id="61b61-206">**type**</span></span>

<span data-ttu-id="61b61-207">Medientyp der Datei. Er legt fest, welches Dateisymbol auf der Seite angezeigt werden soll und welche Anwendung gestartet wird, sobald der Benutzer die Datei auf dem Gerät über OneNote aktiviert.</span><span class="sxs-lookup"><span data-stu-id="61b61-207">The file media type, used to determine the file icon to use on the page, and which application starts when the user activates the file on the device from OneNote.</span></span>

<span data-ttu-id="61b61-208">Beispiel: `type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="61b61-208">Example: `type="application/pdf"`</span></span>


<a name="file-media-types"></a>

#### <a name="file-media-types"></a><span data-ttu-id="61b61-209">Dateimedientypen</span><span class="sxs-lookup"><span data-stu-id="61b61-209">File media types</span></span>  

<span data-ttu-id="61b61-210">Microsoft Graph verwendet für angefügte Dateien vordefinierte Dateitypensymbole. Erkennt die API den Dateityp nicht, wird ein generisches Symbol verwendet.</span><span class="sxs-lookup"><span data-stu-id="61b61-210">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="61b61-211">Nachfolgend sind verschiedene häufig vorkommende Dateitypen aufgeführt, die von der API erkannt werden:</span><span class="sxs-lookup"><span data-stu-id="61b61-211">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="61b61-212">application/pdf</span><span class="sxs-lookup"><span data-stu-id="61b61-212">application/pdf</span></span>  
- <span data-ttu-id="61b61-213">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="61b61-213">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="61b61-214">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="61b61-214">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="61b61-215">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="61b61-215">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="61b61-216">image/png</span><span class="sxs-lookup"><span data-stu-id="61b61-216">image/png</span></span>
- <span data-ttu-id="61b61-217">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="61b61-217">image/jpeg</span></span>
- <span data-ttu-id="61b61-218">image/gif</span><span class="sxs-lookup"><span data-stu-id="61b61-218">image/gif</span></span>
- <span data-ttu-id="61b61-219">audio/wav</span><span class="sxs-lookup"><span data-stu-id="61b61-219">audio/wav</span></span>
- <span data-ttu-id="61b61-220">video/mp4</span><span class="sxs-lookup"><span data-stu-id="61b61-220">video/mp4</span></span>
- <span data-ttu-id="61b61-221">application/msword</span><span class="sxs-lookup"><span data-stu-id="61b61-221">application/msword</span></span>
- <span data-ttu-id="61b61-222">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="61b61-222">application/mspowerpoint</span></span>
- <span data-ttu-id="61b61-223">application/excel</span><span class="sxs-lookup"><span data-stu-id="61b61-223">application/excel</span></span>

<span data-ttu-id="61b61-224">Unter [Einschränkungen](#size-limitations-for-post-pages-requests) sind alle Einschränkungen aufgeführt, die bei der Erstellung von Seiten mit Medien gelten.</span><span class="sxs-lookup"><span data-stu-id="61b61-224">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a><span data-ttu-id="61b61-225">Hinzufügen von Dateianlagen</span><span class="sxs-lookup"><span data-stu-id="61b61-225">Add a file attachment</span></span>

<span data-ttu-id="61b61-226">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Dateidaten enthält.</span><span class="sxs-lookup"><span data-stu-id="61b61-226">In the input HTML of your request's **Presentation** part, include `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="61b61-227">Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.</span><span class="sxs-lookup"><span data-stu-id="61b61-227">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
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

### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="61b61-228">Hinzufügen von Bildern von PDF-Inhalten</span><span class="sxs-lookup"><span data-stu-id="61b61-228">Add images of PDF file contents</span></span>

<span data-ttu-id="61b61-229">Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img data-render-src="name:part-name" ... />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Dateidaten enthält.</span><span class="sxs-lookup"><span data-stu-id="61b61-229">In the input HTML of your request's **Presentation** part, include `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="61b61-230">Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.</span><span class="sxs-lookup"><span data-stu-id="61b61-230">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
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

## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="61b61-231">Größenbeschränkungen bei Anforderungen des Typs „Post pages“</span><span class="sxs-lookup"><span data-stu-id="61b61-231">Size limitations for POST pages requests</span></span>

<span data-ttu-id="61b61-232">Für das Senden von Bild- und Dateidaten gelten folgende Einschränkungen: <!--TODO: check these--></span><span class="sxs-lookup"><span data-stu-id="61b61-232">When sending image and file data, be aware of these limitations: <!--TODO: check these--></span></span>

- <span data-ttu-id="61b61-233">Die maximal zulässige Gesamtgröße von POST-Anforderungen liegt bei etwa 70 MB, einschließlich Bildern, Dateien und anderer Daten.</span><span class="sxs-lookup"><span data-stu-id="61b61-233">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="61b61-234">Das tatsächlich Limit hängt von der Downstreamcodierung ab, daher ist keine feste Bytezahl als Höchstgrenze gesetzt.</span><span class="sxs-lookup"><span data-stu-id="61b61-234">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="61b61-235">Anforderungen, die das Limit überschreiten, geben möglicherweise unzuverlässige Ergebnisse zurück.</span><span class="sxs-lookup"><span data-stu-id="61b61-235">Requests that exceed the limit may produce unreliable results.</span></span>

- <span data-ttu-id="61b61-236">Die maximal zulässige Größe pro Datenteil liegt bei 25 MB, einschließlich des Headers des jeweiligen Teils.</span><span class="sxs-lookup"><span data-stu-id="61b61-236">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="61b61-237">Datenteile, die dieses Limit überschreiten, werden von Microsoft Graph abgelehnt.</span><span class="sxs-lookup"><span data-stu-id="61b61-237">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="61b61-238">Die maximal zulässige Anzahl von Bildern pro Seite beträgt 150.</span><span class="sxs-lookup"><span data-stu-id="61b61-238">The maximum number of images per page is 150.</span></span> <span data-ttu-id="61b61-239">Bei Verwendung des Attributs `src="https://..."` ignoriert die API alle Tags des Typs **img**, die über dieses Limit hinausgehen.</span><span class="sxs-lookup"><span data-stu-id="61b61-239">When using the `src="https://..."` attribute, the API ignores **img** tags beyond the limit.</span></span>

- <span data-ttu-id="61b61-240">Die maximal zulässige Anzahl von Datenteilen pro POST-Anforderung liegt bei 6, einschließlich des zwingend erforderlichen Teils **Presentation**.</span><span class="sxs-lookup"><span data-stu-id="61b61-240">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="61b61-241">Jede Anforderung darf bis zu 5 Elemente des Typs **img** enthalten, die **data-render-src** verwenden, sowie 1 Element des Typs **object**, das **data-render-src** verwendet. Alle weiteren Bild- und Dateiverweise werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="61b61-241">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="61b61-242">Die maximal zulässige Anzahl von Bildern pro POST-Anforderung liegt bei 30, unabhängig von der Methode, über die sie an die API gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="61b61-242">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="61b61-243">Alle weiteren Bilder werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="61b61-243">Additional images are ignored.</span></span> <span data-ttu-id="61b61-244">Wenn Sie eine Webseite mit vielen Bildern abbilden möchten, empfiehlt sich die [Erstellung einer Momentaufnahme der gesamten Seite](#add-a-webpage-snapshot).</span><span class="sxs-lookup"><span data-stu-id="61b61-244">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="61b61-245">Anwendungsfälle: HTML vs. data-render-src</span><span class="sxs-lookup"><span data-stu-id="61b61-245">When to use HTML versus data-render-src</span></span> 

<span data-ttu-id="61b61-246">Ob Sie den HTML-Code direkt auf der OneNote-Seite einfügen oder das Attribut **data-render-src** verwenden sollten, hängt von verschiedenen Faktoren ab. Berücksichtigen Sie bei Ihrer Entscheidung Folgendes:</span><span class="sxs-lookup"><span data-stu-id="61b61-246">When trying to decide between putting HTML directly onto the OneNote page instead of using the **data-render-src** attribute, consider the following:</span></span>

- <span data-ttu-id="61b61-247">Komplexer HTML-Code sollte per **data-render-src** an das Renderingmodul gesendet werden. Eine manuelle Anpassung des HTML-Codes an die Anforderungen von Microsoft Graph empfiehlt sich nicht.</span><span class="sxs-lookup"><span data-stu-id="61b61-247">Complex HTML is probably best sent to the rendering engine via **data-render-src**, rather than attempting to modify the HTML to fit into what Microsoft Graph can accept.</span></span> <span data-ttu-id="61b61-248">Dies gilt auch für HTML-Code mit nicht unterstützten Tags.</span><span class="sxs-lookup"><span data-stu-id="61b61-248">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="61b61-249">Für akkurates Seitenrendering unter Beibehaltung des Layouts und Designs der Seite empfiehlt sich die Verwendung des Renderingmoduls per **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="61b61-249">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="61b61-p130">Direkt bearbeitbarer Text lässt sich häufig am besten durch direktes Einfügen des HTML-Codes in die Seite erreichen. Die gerenderten Bilder werden von einem System für die optische Zeichenerkennung (OCR) gescannt, sind jedoch nicht unbedingt identisch.</span><span class="sxs-lookup"><span data-stu-id="61b61-p130">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="61b61-252">Momentaufnahmen bestimmter Zeitpunkte zu Verlaufs- oder Archivierungszwecken sollten mithilfe der Methode **data-render-src** angefertigt werden.</span><span class="sxs-lookup"><span data-stu-id="61b61-252">Snapshot-in-time for historical or archival purposes is usually best done with the **data-render-src** method.</span></span>

- <span data-ttu-id="61b61-p131">Das Markieren eines Webseitenentwurfs für Überprüfungen ist ein Bereich, in dem **data-render-src** besonders hervorsticht. Mithilfe der Freihandfunktionen von OneNote können Sie auf einem Bild zeichnen, um Änderungen anzugeben oder bestimmte Abschnitte hervorzuheben. Wenn die Webseite als Bild vorliegt, ist das wesentlich einfacher.</span><span class="sxs-lookup"><span data-stu-id="61b61-p131">Marking-up a web page design for revisions is one place the **data-render-src** truly shines. Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas. Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="61b61-256">Sehr große Bilder oder Bilder in Formaten, die OneNote nicht direkt unterstützt, lassen sich mit dem Attribut **data-render-src** mitunter einfacher als Miniaturansicht anzeigen und konvertieren, als dies mit eigenem Code möglich wäre.</span><span class="sxs-lookup"><span data-stu-id="61b61-256">Very large images, or images in formats that OneNote doesn't directly accept, can sometimes be thumbnailed and converted with the **data-render-src** attribute more easily than by doing it in your own code.</span></span> <span data-ttu-id="61b61-257">Selbst wenn das Bild auch online verfügbar ist: Wenn Sie die Daten in die POST-Anforderung einbetten, steht die Seitenabbildung OneNote-Benutzern manchmal schneller zur Verfügung, da zur Erstellung der OneNote-Seite insgesamt weniger Roundtrips nötig sind.</span><span class="sxs-lookup"><span data-stu-id="61b61-257">Even if the image is also available online, embedding the data in your POST can sometimes make the captured page available to OneNote users sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="61b61-258">Manchmal können Sie am einfachsten herausfinden, welche Methode für Ihre Benutzer die beste ist, indem sie während der App-Entwicklung beide Varianten testen.</span><span class="sxs-lookup"><span data-stu-id="61b61-258">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="61b61-259">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61b61-259">Permissions</span></span>

<span data-ttu-id="61b61-260">Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="61b61-260">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="61b61-261">Wählen Sie die niedrigste Stufe, die erforderlich ist, damit Ihre App korrekt funktioniert.</span><span class="sxs-lookup"><span data-stu-id="61b61-261">Choose the lowest level that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="61b61-262">Berechtigungen für BEITRAG-Seiten</span><span class="sxs-lookup"><span data-stu-id="61b61-262">Permissions for POST pages</span></span>

- <span data-ttu-id="61b61-263">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="61b61-263">Notes.Create</span></span>
- <span data-ttu-id="61b61-264">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b61-264">Notes.ReadWrite</span></span>
- <span data-ttu-id="61b61-265">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61b61-265">Notes.ReadWrite.All</span></span> 

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="61b61-266">Berechtigungen für PATCH-Seiten</span><span class="sxs-lookup"><span data-stu-id="61b61-266">Permissions for PATCH pages</span></span>

- <span data-ttu-id="61b61-267">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61b61-267">Notes.ReadWrite</span></span>
- <span data-ttu-id="61b61-268">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61b61-268">Notes.ReadWrite.All</span></span>

<span data-ttu-id="61b61-269">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie unter [OneNote-Berechtigungsbereiche](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="61b61-269">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="61b61-270">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="61b61-270">See also</span></span>

- [<span data-ttu-id="61b61-271">Integrieren mit OneNote</span><span class="sxs-lookup"><span data-stu-id="61b61-271">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="61b61-272">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="61b61-272">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="61b61-273">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="61b61-273">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="61b61-274">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="61b61-274">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

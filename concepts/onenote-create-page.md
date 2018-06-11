# <a name="create-onenote-pages"></a><span data-ttu-id="43101-101">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="43101-101">Create OneNote pages</span></span>

<span data-ttu-id="43101-102">*__Gilt für:__ Privatanwender-Notizbücher auf OneDrive | Enterprise-Notizbücher auf Office 365*</span><span class="sxs-lookup"><span data-stu-id="43101-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="43101-103">Zum Erstellen einer OneNote-Seite senden Sie eine POST-Anforderung an einen *pages*-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="43101-103">When you create a OneNote page, you send a POST request to  the pages endpoint:</span></span> <span data-ttu-id="43101-104">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="43101-104">For example:</span></span>

`POST ../notes/sections/{id}/pages`</p>

<span data-ttu-id="43101-105">Senden Sie den HTML-Code, der die Seite definiert, im Nachrichtentext.</span><span class="sxs-lookup"><span data-stu-id="43101-105">Send the HTML that defines the page in the message body.</span></span> <span data-ttu-id="43101-106">Wenn die Anforderung erfolgreich ist, gibt Microsoft Graph den HTTP-Statuscode 201 zurück.</span><span class="sxs-lookup"><span data-stu-id="43101-106">If the create request is successful, the onnvshort API returns a 201 HTTP status code.</span></span>


> <span data-ttu-id="43101-107">**Hinweis:** Informationen zu den POST-Anforderungen, mit denen Sie Abschnitte, Abschnittsgruppen und Notizbücher erstellen können, finden Sie in der [interaktiven REST-Referenz](http://dev.onenote.com/docs).</span><span class="sxs-lookup"><span data-stu-id="43101-107">**Note:** To learn about the POST requests you can send to create sections, section groups, and notebooks, see our [interactive REST reference](http://dev.onenote.com/docs).</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="43101-108">Erstellen des Anforderungs-URI</span><span class="sxs-lookup"><span data-stu-id="43101-108">Construct the request</span></span>

<span data-ttu-id="43101-109">Um den URI der POST-Anforderung zu erstellen, beginnen Sie mit der Stamm-URL des Diensts:</span><span class="sxs-lookup"><span data-stu-id="43101-109">To construct the POST request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="43101-110">Fügen Sie dann den *pages*-Endpunkt an:</span><span class="sxs-lookup"><span data-stu-id="43101-110">Then append the *pages* endpoint:</span></span>

<span data-ttu-id="43101-111">**Erstellen einer Seite in einem beliebigen Abschnitt (angegeben durch den Abschnittsnamen)**</span><span class="sxs-lookup"><span data-stu-id="43101-111">**Create a page in any section (specified by section name)**</span></span>

`.../pages?sectionName=DefaultSection`

<span data-ttu-id="43101-112">**Erstellen einer Seite in einem beliebigen Abschnitt (angegeben durch die ID)**</span><span class="sxs-lookup"><span data-stu-id="43101-112">**Create a page in any section (specified by ID)**</span></span> 

`.../sections/{section-id}/pages` 

<span data-ttu-id="43101-113">Wenn Sie Seiten im persönlichen Notizbuch des Benutzers erstellen, bietet Microsoft Graph auch Endpunkte, die Sie zum Erstellen von Seiten im Standardnotizbuch verwenden können:</span><span class="sxs-lookup"><span data-stu-id="43101-113">If you're creating pages in the user's personal notebook, Microsoft Graph also provides endpoints you can use to create pages in the default notebook:</span></span>

<span data-ttu-id="43101-114">**Erstellen einer Seite im Standardabschnitt des Standardnotizbuchs**</span><span class="sxs-lookup"><span data-stu-id="43101-114">**Create a new OneNote page in the default section of the default notebook.**</span></span> 

`../pages` 



<span data-ttu-id="43101-115">Ihr vollständiger Anforderungs-URI gleicht einem der folgenden Beispiele:</span><span class="sxs-lookup"><span data-stu-id="43101-115">Your full request URI will look like one of these examples:</span></span>
* `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
* `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

<span data-ttu-id="43101-116">Hier erfahren Sie mehr über die [Stamm-URL des Diensts](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="43101-116">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="post-pages-section-name"></a>
### <a name="using-the-sectionname-url-parameter"></a><span data-ttu-id="43101-117">Verwenden des URL-Parameters *sectionName*</span><span class="sxs-lookup"><span data-stu-id="43101-117">Using the *sectionName* URL parameter</span></span>

<span data-ttu-id="43101-118">Die folgenden Regeln gelten bei Verwendung des *sectionName*-Parameters zum Erstellen einer Seite in einem benannten Abschnitt im Standardnotizbuch:</span><span class="sxs-lookup"><span data-stu-id="43101-118">The following rules apply when using the *sectionName* parameter to create a page in a named section in the default notebook:</span></span>

- <span data-ttu-id="43101-119">Nur auf Abschnitte auf oberster Ebene kann verwiesen werden (keine Abschnitte in Abschnittsgruppen).</span><span class="sxs-lookup"><span data-stu-id="43101-119">Only top-level sections can be referenced (not sections within section groups).</span></span>

- <span data-ttu-id="43101-120">Ist im Standardnotizbuch kein Abschnitt mit dem angegebenen Namen vorhanden, wird er von der API erstellt.</span><span class="sxs-lookup"><span data-stu-id="43101-120">If a section with the specified name doesn't exist in the default notebook, the API creates it.</span></span> <span data-ttu-id="43101-121">Die folgenden Zeichen sind für Abschnittsnamen nicht zulässig: ?</span><span class="sxs-lookup"><span data-stu-id="43101-121">These characters are not allowed for section names: ?</span></span> <span data-ttu-id="43101-122">\* \ / : &lt; &gt; | &amp; # " % ~</span><span class="sxs-lookup"><span data-stu-id="43101-122">\* \ / : &lt; &gt; | &amp; # " % ~</span></span>

- <span data-ttu-id="43101-123">Beim Abgleich von Abschnittsnamen wird die Groß-und Kleinschreibung nicht beachtet, aber beim Erstellen von Abschnitten bleibt die Groß-/Kleinschreibung erhalten.</span><span class="sxs-lookup"><span data-stu-id="43101-123">Section names are case-insensitive for matching, but case is preserved when sections are created.</span></span> <span data-ttu-id="43101-124">Somit wird z. B. „Mein neuer Abschnitt“ genau so angezeigt, aber „mein neuer abschnitt“ würde bei nachfolgenden Übermittlungen ebenfalls übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="43101-124">Section names are case-insensitive for matching, but the case is preserved when they are created. So "My New Section" will be displayed like that, but "my new section" would also match on subsequent posts.</span></span>

- <span data-ttu-id="43101-125">Abschnittsnamen müssen URL-codiert sein.</span><span class="sxs-lookup"><span data-stu-id="43101-125">Section names must be URL-encoded.</span></span> <span data-ttu-id="43101-126">Z. B. müssen Leerzeichen als *%20* codiert werden.</span><span class="sxs-lookup"><span data-stu-id="43101-126">The new section name must be URL-encoded.  For example, spaces must be encoded as *%20*.</span></span>

- <span data-ttu-id="43101-127">Der *sectionName*-Parameter gilt nur für die Route `../notes/pages` (nicht für `../notes/sections/{id}/pages`).</span><span class="sxs-lookup"><span data-stu-id="43101-127">The *sectionName* parameter is valid only with the `../notes/pages` route (not `../notes/sections/{id}/pages`).</span></span>

<span data-ttu-id="43101-128">Da Abschnitte erstellt werden, wenn sie noch nicht vorhanden sind, ist es sicherer, diesen Aufruf mit jeder Seite zu verwenden, die Ihre App erstellt.</span><span class="sxs-lookup"><span data-stu-id="43101-128">Because sections are created if they don't exist, it's safe to use this call with every page your app creates.</span></span> <span data-ttu-id="43101-129">Benutzer können Abschnitte möglicherweise umbenennen, doch die API erstellt einen neuen Abschnitt mit dem Abschnittsnamen, den Sie angeben.</span><span class="sxs-lookup"><span data-stu-id="43101-129">Users might rename sections, in which case the API will create a new section with the sectionName you supply.</span></span> 

> <span data-ttu-id="43101-130">**Hinweis:** Die von der API zurückgegebenen Links für Seiten in einem umbenannten Abschnitt führen weiterhin zu den betreffenden älteren Seiten.</span><span class="sxs-lookup"><span data-stu-id="43101-130">**Note:** The links returned by the API for pages in a renamed section will still reach those older pages.</span></span> 


<a name="message-body"></a>
## <a name="construct-the-message-body"></a><span data-ttu-id="43101-131">Erstellen des Nachrichtentexts</span><span class="sxs-lookup"><span data-stu-id="43101-131">Construct the message body</span></span>

<span data-ttu-id="43101-132">Der HTML-Code, der Seiteninhalt definiert, wird als *Eingabe-HTML* bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="43101-132">The HTML that defines the page content and structure when you create or update a OneNote page is called *input HTML*.</span></span> <span data-ttu-id="43101-133">Eingabe-HTML unterstützt eine [Teilmenge der Standard-HTML und -CSS](#supported-html-and-css-for-onenote-pages) mit zusätzlichen benutzerdefinierten Attributen.</span><span class="sxs-lookup"><span data-stu-id="43101-133">Input HTML supports a [subset of standard HTML and CSS](#supported-html-and-css-for-onenote-pages), with the addition of custom attributes.</span></span> <span data-ttu-id="43101-134">(Benutzerdefinierte Attribute, wie **data-id** und **data-render-src**, werden in [Eingabe- und Ausgabe-HTML](onenote_input_output_html.md) beschrieben.)</span><span class="sxs-lookup"><span data-stu-id="43101-134">(Custom attributes, like **data-id** and **data-render-src**, are described in [Input and output HTML](onenote_input_output_html.md).)</span></span> 

<span data-ttu-id="43101-135">Senden Sie die Eingabe-HTML im Nachrichtentext der POST-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43101-135">Send the input HTML in the message body of the POST request.</span></span> <span data-ttu-id="43101-136">Sie können die Eingabe-HTML direkt im Nachrichtentext mit dem Inhaltstyp `application/xhtml+xml` oder `text/html` senden, oder Sie können sie im „Presentation“-Teil einer mehrteiligen Anforderung senden.</span><span class="sxs-lookup"><span data-stu-id="43101-136">You can send the input HTML directly in the message body using the  `application/xhtml+xml` or `text/html` content type, or you can send it in the "Presentation" part of a multipart request.</span></span> 

<span data-ttu-id="43101-137">Das folgende Beispiel sendet die Eingabe-HTML direkt im Nachrichtentext.</span><span class="sxs-lookup"><span data-stu-id="43101-137">The following example sends the input HTML directly in the message body.</span></span>

```
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="http://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<span data-ttu-id="43101-138">Wenn Sie Binärdaten senden, müssen Sie eine [mehrteilige Anforderung](#example-request) verwenden.</span><span class="sxs-lookup"><span data-stu-id="43101-138">If you're sending binary data, you must use a [multipart request](#example-request).</span></span> 

><span data-ttu-id="43101-139">Zur Vereinfachung der Programmierung und Konsistenz in Ihrer App können Sie mehrteilige Anforderungen verwenden, um alle Seiten zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="43101-139">To simplify programming and consistency in your app, you can use multipart requests to create all pages.</span></span> <span data-ttu-id="43101-140">Es ist ratsam, eine Bibliothek zu verwenden, um mehrteilige Nachrichten zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="43101-140">It's a good idea to use a library to construct multipart messages.</span></span> <span data-ttu-id="43101-141">Dadurch wird das Risiko der Erstellung von fehlerhaften Nutzlasten reduziert.</span><span class="sxs-lookup"><span data-stu-id="43101-141">This reduces the risk of creating malformed payloads.</span></span>


<a name="input-html-rules"></a>
### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a><span data-ttu-id="43101-142">Anforderungen und Einschränkungen für Eingabe-HTML in POST-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="43101-142">Requirements and limitations for input HTML in POST pages requests</span></span>

<span data-ttu-id="43101-143">Beachten Sie beim Senden von Eingabe-HTML diese allgemeinen Anforderungen und Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="43101-143">When sending input HTML, be aware of these general requirements and limitations:</span></span>  

- <span data-ttu-id="43101-144">Die Eingabe-HTML sollte UTF-8-codierter und wohlgeformter XHTML-Code sein.</span><span class="sxs-lookup"><span data-stu-id="43101-144">Input HTML should be UTF-8 encoded and well-formed XHTML.</span></span> <span data-ttu-id="43101-145">Für alle Container-Starttags müssen die entsprechenden schließenden Tags vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="43101-145">All container start tags require matching closing tags.</span></span> <span data-ttu-id="43101-146">Alle Attributwerte müssen in doppelte oder einzelne Anführungszeichen eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="43101-146">All attribute values must be surrounded by double- or single-quote marks like in the preceding img tag.</span></span>  <!--docs say MUST be encoded-->

- <span data-ttu-id="43101-147">JavaScript-Code, hinzugefügte Dateien und CSS werden entfernt.</span><span class="sxs-lookup"><span data-stu-id="43101-147">Javascript code, included files and CSS are removed.</span></span> 

- <span data-ttu-id="43101-148">HTML-Formulare werden vollständig entfernt.</span><span class="sxs-lookup"><span data-stu-id="43101-148">HTML forms are removed in their entirety.</span></span>  

- <span data-ttu-id="43101-149">Microsoft Graph unterstützt eine [Teilmenge der HTML-Elemente](#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="43101-149">Microsoft Graph supports a [subset of HTML elements](#supported-html-and-css-for-onenote-pages).</span></span> 

- <span data-ttu-id="43101-150">Microsoft Graph unterstützt eine Teilmenge der allgemeinen HTML-Attribute und eine Reihe von benutzerdefinierten Attributen, z. B. das **data-id**-Attribut, das für das Aktualisieren von Seiten verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="43101-150">Microsoft Graph supports a subset of common HTML attributes and a set of custom attributes, such as the **data-id** attribute used for updating pages.</span></span> <span data-ttu-id="43101-151">Weitere Informationen zu den unterstützten Attributen finden Sie unter [Eingabe- und Ausgabe-HTML](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="43101-151">See [Input and output HTML](onenote_input_output_html.md) for supported attributes.</span></span>


<a name="supported-html"></a>
### <a name="supported-html-and-css-for-onenote-pages"></a><span data-ttu-id="43101-152">Unterstützte HTML und CSS für OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="43101-152">Supported HTML and CSS for OneNote pages</span></span>

<span data-ttu-id="43101-153">Nicht alle Elemente, Attribute und Eigenschaften werden (in HTML4, XHTML, CSS, HTML5 usw.) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43101-153">Not all elements, attributes, and properties are supported (in HTML4, XHTML, CSS, HTML5, etc.).</span></span> <span data-ttu-id="43101-154">Stattdessen akzeptiert Microsoft Graph einen eingeschränkten Satz von HTML-Elementen, der der üblichen Verwendung von OneNote besser entspricht.</span><span class="sxs-lookup"><span data-stu-id="43101-154">Instead, Microsoft Graph accepts a limited set of HTML that better fits how people use OneNote.</span></span> <span data-ttu-id="43101-155">Weitere Informationen finden Sie unter [Unterstützung von HTML-Tags für Seiten](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span><span class="sxs-lookup"><span data-stu-id="43101-155">For more information, see [HTML tag support for pages](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span></span> <span data-ttu-id="43101-156">Wenn ein Tag dort nicht aufgeführt ist, wird es wahrscheinlich ignoriert.</span><span class="sxs-lookup"><span data-stu-id="43101-156">If a tag's not listed there, it'll probably be ignored.</span></span>

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

<span data-ttu-id="43101-157">Die folgende Liste zeigt die grundlegenden Elementtypen, die Microsoft Graph unterstützt:</span><span class="sxs-lookup"><span data-stu-id="43101-157">The following list shows the basic element types that Microsoft Graph supports:</span></span>

- <span data-ttu-id="43101-158">`<head>` und `<body>`</span><span class="sxs-lookup"><span data-stu-id="43101-158">`<head>` and `<body>`</span></span></p>
- <span data-ttu-id="43101-159">`<title>` und `<meta>`, die den Seitentitel und das Erstellungsdatum festlegen</span><span class="sxs-lookup"><span data-stu-id="43101-159"><title>`<title>` and <meta>`<meta>` that set the page title and creation date</span></span></p>
- <span data-ttu-id="43101-160">`<h1>` bis `<h6>` für Abschnittsüberschriften</span><span class="sxs-lookup"><span data-stu-id="43101-160"><h1>`<h1>` through <h6>`<h6>` for section headings</span></span></p>
- <span data-ttu-id="43101-161">`<p>` für Absätze</span><span class="sxs-lookup"><span data-stu-id="43101-161">`<p>` for paragraphs</span></span></p>
- <span data-ttu-id="43101-162">`<ul>`, `<ol>` und `<li>` für Listen und Listenelemente</span><span class="sxs-lookup"><span data-stu-id="43101-162">`<ul>`, `<ol>`, and `<li>` for lists and list items</span></span></p>
- <span data-ttu-id="43101-163">`<table>`, `<tr>` und `<td>`, einschließlich geschachtelter Tabellen</span><span class="sxs-lookup"><span data-stu-id="43101-163"><table>, <tr> and <td>, including nested tables</span></span></p>
- <span data-ttu-id="43101-164">`<pre>` für vorformatierten Text (behält Leerräume und Zeilenumbrüche bei)</span><span class="sxs-lookup"><span data-stu-id="43101-164">`<pre>` for preformatted text (preserves white space and line breaks)</span></span></p>
- <span data-ttu-id="43101-165">`<b>` und `<i>` für fette und kursive Zeichenformate</span><span class="sxs-lookup"><span data-stu-id="43101-165"><b>`<b>` and <i>`<i>` for bold and italic character styles</span></span></p>

<span data-ttu-id="43101-166">Microsoft Graph behält den semantischen Inhalt und die grundlegende Struktur der Eingabe-HTML bei der Seitenerstellung bei, konvertiert jedoch die Eingabe-HTML in die unterstützte Teilmenge von HTML und CSS.</span><span class="sxs-lookup"><span data-stu-id="43101-166">Microsoft Graph preserves the semantic content and basic structure of the input HTML when it creates pages, but it converts the input HTML to use the supported set of HTML and CSS.</span></span> <span data-ttu-id="43101-167">Features, die in OneNote nicht vorhanden sind, können nicht übersetzt werden und werden somit möglicherweise in der HTML-Quelldatei nicht erkannt.</span><span class="sxs-lookup"><span data-stu-id="43101-167">Features that don't exist in OneNote have nothing to be translated to, so they might not be recognized in the source HTML.</span></span> 


<a name="example"></a>
## <a name="example-request"></a><span data-ttu-id="43101-168">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="43101-168">Example request</span></span>

<span data-ttu-id="43101-169">Dieses Beispiel einer mehrteiligen Anforderung erstellt eine Seite, die Bilder und eine eingebettete Datei enthält.</span><span class="sxs-lookup"><span data-stu-id="43101-169">This example multipart request creates a page that contains images and an embedded file.</span></span> <span data-ttu-id="43101-170">Der erforderliche **Presentation**-Teil enthält die Eingabe-HTML, die die Seite definiert.</span><span class="sxs-lookup"><span data-stu-id="43101-170">The required **Presentation** part contains the input HTML that defines the page.</span></span> <span data-ttu-id="43101-171">Der **imageBlock1**-Teil enthält die binären Bilddaten und **fileBlock1** die Binärdateidaten.</span><span class="sxs-lookup"><span data-stu-id="43101-171">The **imageBlock1** part contains the binary image data and **fileBlock1** contains the binary file data.</span></span> <span data-ttu-id="43101-172">Datenteile enthalten können auch HTML enthalten. In diesem Fall [rendert Microsoft Graph den HTML-Code als Bild](onenote_images_files.md#add-an-image-using-binary-data) auf der OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="43101-172">Data parts can also contain HTML, in which case Microsoft Graph [renders the HTML as an image](onenote_images_files.md#add-an-image-using-binary-data) on the OneNote page.</span></span> 

```
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="http://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```

<span data-ttu-id="43101-173">Weitere Beispiele für die Erstellung von Seiten, die Bilder und andere Dateien enthalten, finden Sie unter [Hinzufügen von Bildern und Dateien](onenote_images_files.md) sowie in unseren [Lernprogrammen](https://msdn.microsoft.com/de-DE/office/office365/howto/onenote-tutorial) und [Beispielen](https://github.com/onenotedev).</span><span class="sxs-lookup"><span data-stu-id="43101-173">For more examples that show how to create pages that contain images and other files, see [Add images and files](onenote_images_files.md), our [tutorials](https://msdn.microsoft.com/de-DE/office/office365/howto/onenote-tutorial), and our [samples](https://github.com/onenotedev).</span></span> <span data-ttu-id="43101-174">Außerdem finden Sie Informationen zum [Erstellen absolut positionierter Elemente](onenote-abs-pos.md), [Verwenden von Notiztags](onenote-note-tags.md) und [Extrahieren von Daten](onenote-extract-data.md) für Visitenkarten und Onlinerezept- und Produktlisten.</span><span class="sxs-lookup"><span data-stu-id="43101-174">Also, learn how to [create absolute positioned elements](onenote-abs-pos.md), [use note tags](onenote-note-tags.md), and [extract data](onenote-extract-data.md) for business card captures and online recipe and product listings.</span></span>

<span data-ttu-id="43101-175">Microsoft Graph hat in einigen Formaten strenge Anforderungen, z. B. CRLF-Zeilenumbrüche in einem mehrteiligen Nachrichtentext.</span><span class="sxs-lookup"><span data-stu-id="43101-175">Microsoft Graph is strict about some formats, such as CRLF newlines in a multipart message body.</span></span> <span data-ttu-id="43101-176">Um das Risiko fehlerhafter Nutzlasten zu reduzieren, sollten Sie eine Bibliothek verwenden, um mehrteilige Nachrichten zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="43101-176">To reduce the risk of creating malformed payloads, you should use a library to construct multipart messages.</span></span> <span data-ttu-id="43101-177">Wenn Sie eine Statusmeldung 400 für eine fehlerhafte Nutzlast erhalten, überprüfen Sie die Formatierung der Zeilenumbrüche und Leerräume, und achten Sie auf Codierungsprobleme.</span><span class="sxs-lookup"><span data-stu-id="43101-177">If you do receive a 400 status for a malformed payload, check the formatting of newlines and whitespaces, and check for encoding issues.</span></span> <span data-ttu-id="43101-178">Versuchen Sie beispielsweise die Verwendung von `charset=utf-8` (Beispiel: `Content-Type: text/html; charset=utf-8`).</span><span class="sxs-lookup"><span data-stu-id="43101-178">For example, try using `charset=utf-8` (example: `Content-Type: text/html; charset=utf-8`).</span></span>

<span data-ttu-id="43101-179">Siehe [Anforderungen und Einschränkungen für Eingabe-HTML](#requirements-and-limitations-for-input-html-in-post-pages-requests) und [Größenbeschränkungen für POST-Anforderungen](onenote_images_files.md#size-limitations-for-post-pages-requests).</span><span class="sxs-lookup"><span data-stu-id="43101-179">See [requirements and limitations for input HTML](#requirements-and-limitations-for-input-html-in-post-pages-requests) and [size limits for POST requests](onenote_images_files.md#size-limitations-for-post-pages-requests).</span></span>


<a name="request-response-info"></a>
## <a name="request-and-response-information-for-post-pages-requests"></a><span data-ttu-id="43101-180">Anforderungs- und Antwortinformationen für *POST pages*-Anforderungen</span><span class="sxs-lookup"><span data-stu-id="43101-180">Request and response information for *POST pages* requests</span></span>

| <span data-ttu-id="43101-181">Anforderungsdaten</span><span class="sxs-lookup"><span data-stu-id="43101-181">Request data</span></span> | <span data-ttu-id="43101-182">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43101-182">Description</span></span> |  
|------|------|  
| <span data-ttu-id="43101-183">Protokoll</span><span class="sxs-lookup"><span data-stu-id="43101-183">Protocol</span></span> | <span data-ttu-id="43101-184">Alle Anforderungen verwenden das SSL/TLS HTTPS-Protokoll.</span><span class="sxs-lookup"><span data-stu-id="43101-184">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="43101-185">Header „Authorization“</span><span class="sxs-lookup"><span data-stu-id="43101-185">Authorization header</span></span> | <p><span data-ttu-id="43101-186">`Bearer {token}`, wobei *{token}* ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</span><span class="sxs-lookup"><span data-stu-id="43101-186">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="43101-187">Wenn dies fehlt oder ungültig ist, schlägt die Anforderung mit dem Statuscode 401 fehl.</span><span class="sxs-lookup"><span data-stu-id="43101-187">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="43101-188">Siehe [Authentifizierung und Berechtigungen](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43101-188">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="43101-189">Header „Content-Type“</span><span class="sxs-lookup"><span data-stu-id="43101-189">content-type header</span></span> | <p><span data-ttu-id="43101-190">`text/html` oder `application/xhtml+xml` für den HTML-Inhalt, unabhängig davon, ob er direkt im Nachrichtentext oder im erforderlichen „Presentation“-Teil einer mehrteiligen Anforderung gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="43101-190">`text/html` or `application/xhtml+xml` for the HTML content, whether it's sent directly in the message body or in the required "Presentation" part of multipart requests.</span></span></p><p><span data-ttu-id="43101-191">Mehrteilige Anfragen sind erforderlich, wenn Binärdaten gesendet werden sollen. Sie verwenden den Inhaltstyp `multipart/form-data; boundary=part-boundary`, wobei *{part-boundary}* eine Zeichenfolge ist, die den Beginn und das Ende jedes Datenteils signalisiert.</span><span class="sxs-lookup"><span data-stu-id="43101-191">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where *{part-boundary}* is a string that signals the start and end of each data part.</span></span></p> |  
| <span data-ttu-id="43101-192">Header „Accept“</span><span class="sxs-lookup"><span data-stu-id="43101-192">accept header</span></span> | `application/json` | 

| <span data-ttu-id="43101-193">Antwortdaten</span><span class="sxs-lookup"><span data-stu-id="43101-193">Response data</span></span> | <span data-ttu-id="43101-194">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43101-194">Description</span></span> |  
|------|------|  
| <span data-ttu-id="43101-195">Erfolgscode</span><span class="sxs-lookup"><span data-stu-id="43101-195">Success code</span></span> | <span data-ttu-id="43101-196">HTTP-Statuscode 201.</span><span class="sxs-lookup"><span data-stu-id="43101-196">A 201 HTTP status code.</span></span> |  
| <span data-ttu-id="43101-197">Antworttext</span><span class="sxs-lookup"><span data-stu-id="43101-197">Response body</span></span> | <span data-ttu-id="43101-198">Eine OData-Darstellung der neuen Seite im JSON-Format.</span><span class="sxs-lookup"><span data-stu-id="43101-198">A OData representation of the new page in JSON format.</span></span> |  
| <span data-ttu-id="43101-199">Fehler</span><span class="sxs-lookup"><span data-stu-id="43101-199">Errors</span></span> | <span data-ttu-id="43101-200">Wenn die Anforderung nicht erfüllt wird, gibt die API Fehler im **@api.diagnostics**-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="43101-200">If the update request fails, the API returns errors in the **api.diagnostics** object in the response body. The request will fail if:</span></span> |  
| <span data-ttu-id="43101-201">Header „Location“</span><span class="sxs-lookup"><span data-stu-id="43101-201">Location header</span></span> | <span data-ttu-id="43101-202">Die URL der Ressource für die neue Seite.</span><span class="sxs-lookup"><span data-stu-id="43101-202">The resource URL for the new page.</span></span> |  
| <span data-ttu-id="43101-203">Header „X-CorrelationId“</span><span class="sxs-lookup"><span data-stu-id="43101-203">X-CorrelationId header</span></span> | <span data-ttu-id="43101-204">Ein globaler Bezeichner (GUID), über den die Anforderung eindeutig identifiziert wird.</span><span class="sxs-lookup"><span data-stu-id="43101-204">A GUID that uniquely identifies a query request.</span></span> <span data-ttu-id="43101-205">Sie können diesen Wert zusammen mit dem Wert des Date-Headers verwenden, um zusammen mit dem Microsoft Support Probleme zu behandeln.</span><span class="sxs-lookup"><span data-stu-id="43101-205">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>
### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="43101-206">Zusammensetzen der Stamm-URL des Microsoft Graph-Diensts</span><span class="sxs-lookup"><span data-stu-id="43101-206">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="43101-207">Die Stamm-URL des Microsoft Graph-Diensts verwendet das folgende Format für alle Aufrufe von Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="43101-207">The Microsoft Graph service root URL uses the following format for all calls to Microsoft Graph.</span></span> <span data-ttu-id="43101-208">`https://graph.microsoft.com/{version}/me/onenote/`  Das `version`-Segment in der URL stellt die Version von Microsoft Graph dar, die Sie verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="43101-208">`https://graph.microsoft.com/{version}/me/onenote/`  The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="43101-209">Verwenden Sie `v1.0` für stabilen Produktionscode.</span><span class="sxs-lookup"><span data-stu-id="43101-209">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="43101-210">Verwenden Sie `beta`, um ein Feature zu testen, das sich in der Entwicklung befindet.</span><span class="sxs-lookup"><span data-stu-id="43101-210">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="43101-211">Features und Funktionen in der Betaversion ändern sich möglicherweise, sodass Sie es nicht in Ihrem Produktionscode verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="43101-211">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> <span data-ttu-id="43101-212">Verwenden Sie `me` für OneNote-Inhalt, auf den der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte).</span><span class="sxs-lookup"><span data-stu-id="43101-212">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="43101-213">Verwenden Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="43101-213">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="43101-214">Verwenden Sie [Microsoft Graph](https://graph.microsoft.com/v1.0/users), um Benutzer-IDs abzurufen.</span><span class="sxs-lookup"><span data-stu-id="43101-214">Use the [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="43101-215">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="43101-215">Permissions</span></span>

<span data-ttu-id="43101-216">Zum Erstellen von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern.</span><span class="sxs-lookup"><span data-stu-id="43101-216">To create OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="43101-217">Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.</span><span class="sxs-lookup"><span data-stu-id="43101-217">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="43101-218">Wählen Sie zwischen:</span><span class="sxs-lookup"><span data-stu-id="43101-218">Choose from:</span></span> 
- <span data-ttu-id="43101-219">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="43101-219">Notes.Create</span></span>
- <span data-ttu-id="43101-220">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43101-220">Notes.ReadWrite</span></span>
- <span data-ttu-id="43101-221">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43101-221">Notes.ReadWrite.All</span></span>

<span data-ttu-id="43101-222">Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43101-222">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>




<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="43101-223">Weitere Ressourcen</span><span class="sxs-lookup"><span data-stu-id="43101-223">Additional resources</span></span>

- [<span data-ttu-id="43101-224">Hinzufügen von Bildern und Dateien</span><span class="sxs-lookup"><span data-stu-id="43101-224">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="43101-225">Erstellen von absolut positionierten Elementen</span><span class="sxs-lookup"><span data-stu-id="43101-225">Create absolute positioned elements</span></span>](onenote-abs-pos.md)  
- [<span data-ttu-id="43101-226">Extrahieren von Daten</span><span class="sxs-lookup"><span data-stu-id="43101-226">Extract data</span></span>](onenote-extract-data.md)
- [<span data-ttu-id="43101-227">Verwenden von Notiztags</span><span class="sxs-lookup"><span data-stu-id="43101-227">Use note tags</span></span>](onenote-note-tags.md)
- [<span data-ttu-id="43101-228">Integrieren in OneNote</span><span class="sxs-lookup"><span data-stu-id="43101-228">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="43101-229">OneNote-Entwicklerblog</span><span class="sxs-lookup"><span data-stu-id="43101-229">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="43101-230">Fragen zur OneNote-Entwicklung auf Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="43101-230">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="43101-231">OneNote GitHub-Repos</span><span class="sxs-lookup"><span data-stu-id="43101-231">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  


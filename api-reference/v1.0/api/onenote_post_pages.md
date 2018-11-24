# <a name="create-page"></a><span data-ttu-id="624fb-101">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="624fb-101">Create page</span></span>

<span data-ttu-id="624fb-102">Dient zum Erstellen einer neuen OneNote-Seite im Standardabschnitt des Standardnotizbuchs.</span><span class="sxs-lookup"><span data-stu-id="624fb-102">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="624fb-p101">Um eine Seite in einem anderen Abschnitt des Standardnotizbuchs zu erstellen, können Sie den Abfrageparameter `sectionName` verwenden.  Beispiel: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="624fb-p101">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.  Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="624fb-p102">Der `POST /onenote/pages`-Vorgang wird nur verwendet, um Seiten im Standardnotizbuch des aktuellen Benutzers zu erstellen. Wenn andere Notizbücher Ihr Ziel sind, können Sie [Seiten in einem angegebenen Abschnitt erstellen](../api/section_post_pages.md).</span><span class="sxs-lookup"><span data-stu-id="624fb-p102">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook. If you're targeting other notebooks, you can [create pages in a specified section](../api/section_post_pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="624fb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="624fb-107">Permissions</span></span>
<span data-ttu-id="624fb-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="624fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="624fb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="624fb-110">Permission type</span></span>      | <span data-ttu-id="624fb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="624fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="624fb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="624fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="624fb-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="624fb-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="624fb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="624fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="624fb-115">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="624fb-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="624fb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="624fb-116">Application</span></span> | <span data-ttu-id="624fb-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="624fb-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="624fb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="624fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="624fb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="624fb-119">Request headers</span></span>  
| <span data-ttu-id="624fb-120">Name</span><span class="sxs-lookup"><span data-stu-id="624fb-120">Name</span></span>       | <span data-ttu-id="624fb-121">Typ</span><span class="sxs-lookup"><span data-stu-id="624fb-121">Type</span></span> | <span data-ttu-id="624fb-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="624fb-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="624fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="624fb-123">Authorization</span></span>  | <span data-ttu-id="624fb-124">string</span><span class="sxs-lookup"><span data-stu-id="624fb-124">string</span></span>  | <span data-ttu-id="624fb-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="624fb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="624fb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="624fb-127">Content-Type</span></span> | <span data-ttu-id="624fb-128">string</span><span class="sxs-lookup"><span data-stu-id="624fb-128">string</span></span> | <span data-ttu-id="624fb-p105">`text/html` oder `application/xhtml+xml` für den HTML-Inhalt, auch für den erforderlichen Teil „Präsentation“ von mehrteiligen Anforderungen. Mehrteilige Anforderungen verwenden den Inhaltstyp `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="624fb-p105">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="624fb-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="624fb-131">Request body</span></span>
<span data-ttu-id="624fb-132">Geben Sie im Anforderungstext den HTML-Inhalt für die Seite an.</span><span class="sxs-lookup"><span data-stu-id="624fb-132">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="624fb-p106">Der Text kann HTML-Code enthalten, der direkt im Anforderungstext platziert ist, oder er kann ein mehrteiliges Nachrichtenformat enthalten, wie im Beispiel gezeigt. Wenn Sie Binärdaten senden, müssen Sie eine mehrteilige Anforderung senden.</span><span class="sxs-lookup"><span data-stu-id="624fb-p106">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="624fb-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="624fb-135">Response</span></span>

<span data-ttu-id="624fb-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein neues [page](../resources/page.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="624fb-136">If successful, this method returns a `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="624fb-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="624fb-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="624fb-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="624fb-138">Request</span></span>
<span data-ttu-id="624fb-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="624fb-139">Here is an example of the request.</span></span>

<span data-ttu-id="624fb-p107">Im Pfad `../onenote/pages` können Sie den Abfrageparameter `sectionName` verwenden, um eine Seite in einem bestimmten Abschnitt des Standardnotizbuchs zu erstellen. Beispiel: `../onenote/pages?sectionName=My%20section`. Wenn der Abschnitt nicht vorhanden ist (oder umbenannt wurde), erstellt die API einen neuen Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="624fb-p107">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook. Example: `../onenote/pages?sectionName=My%20section`. If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Content-length: 312
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
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
##### <a name="response"></a><span data-ttu-id="624fb-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="624fb-143">Response</span></span>
<span data-ttu-id="624fb-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="624fb-144">Here is an example of the response.</span></span> <span data-ttu-id="624fb-145">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="624fb-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="624fb-146">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="624fb-146">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
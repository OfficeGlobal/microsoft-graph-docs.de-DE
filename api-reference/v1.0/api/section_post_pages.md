# <a name="create-page"></a><span data-ttu-id="f2ddc-101">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="f2ddc-101">Create page</span></span>

<span data-ttu-id="f2ddc-102">Mit dieser API können Sie eine neue Ressource des Typs [page](../resources/page.md) in dem jeweils angegebenen Abschnitt erstellen.</span><span class="sxs-lookup"><span data-stu-id="f2ddc-102">Create a new [page](../resources/page.md) in the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2ddc-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f2ddc-103">Permissions</span></span>
<span data-ttu-id="f2ddc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f2ddc-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2ddc-106">Permission type</span></span>      | <span data-ttu-id="f2ddc-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2ddc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2ddc-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2ddc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f2ddc-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2ddc-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2ddc-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2ddc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2ddc-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2ddc-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f2ddc-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2ddc-112">Application</span></span> | <span data-ttu-id="f2ddc-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2ddc-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2ddc-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2ddc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="f2ddc-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2ddc-115">Request headers</span></span>
| <span data-ttu-id="f2ddc-116">Name</span><span class="sxs-lookup"><span data-stu-id="f2ddc-116">Name</span></span>       | <span data-ttu-id="f2ddc-117">Typ</span><span class="sxs-lookup"><span data-stu-id="f2ddc-117">Type</span></span> | <span data-ttu-id="f2ddc-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2ddc-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2ddc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2ddc-119">Authorization</span></span>  | <span data-ttu-id="f2ddc-120">string</span><span class="sxs-lookup"><span data-stu-id="f2ddc-120">string</span></span>  | <span data-ttu-id="f2ddc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2ddc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2ddc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2ddc-123">Content-Type</span></span> | <span data-ttu-id="f2ddc-124">string</span><span class="sxs-lookup"><span data-stu-id="f2ddc-124">string</span></span> | <span data-ttu-id="f2ddc-p103">`text/html` oder `application/xhtml+xml` für den HTML-Inhalt, auch für den erforderlichen Teil „Präsentation“ von mehrteiligen Anforderungen. Mehrteilige Anforderungen verwenden den Inhaltstyp `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="f2ddc-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2ddc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2ddc-127">Request body</span></span>
<span data-ttu-id="f2ddc-128">Geben Sie im Anforderungstext den HTML-Inhalt für die Seite an.</span><span class="sxs-lookup"><span data-stu-id="f2ddc-128">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="f2ddc-p104">Der Text kann HTML-Code enthalten, der direkt im Anforderungstext platziert ist, oder er kann ein mehrteiliges Nachrichtenformat enthalten, wie im Beispiel gezeigt. Wenn Sie Binärdaten senden, müssen Sie eine mehrteilige Anforderung senden.</span><span class="sxs-lookup"><span data-stu-id="f2ddc-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="f2ddc-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2ddc-131">Response</span></span>

<span data-ttu-id="f2ddc-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein neues [page](../resources/page.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2ddc-132">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2ddc-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2ddc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2ddc-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2ddc-134">Request</span></span>
<span data-ttu-id="f2ddc-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2ddc-135">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
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
    <img src="http://..." alt="an image on the page" width="500" />
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
##### <a name="response"></a><span data-ttu-id="f2ddc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2ddc-136">Response</span></span>
<span data-ttu-id="f2ddc-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2ddc-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

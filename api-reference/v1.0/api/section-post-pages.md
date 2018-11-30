---
title: Seite erstellen
description: Mit dieser API können Sie eine neue Ressource des Typs page in dem jeweils angegebenen Abschnitt erstellen.
ms.openlocfilehash: ec4373af59ef8a324e8da8f685fc2ff01bde4a2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019348"
---
# <a name="create-page"></a><span data-ttu-id="e154e-103">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="e154e-103">Create page</span></span>

<span data-ttu-id="e154e-104">Mit dieser API können Sie eine neue Ressource des Typs [page](../resources/page.md) in dem jeweils angegebenen Abschnitt erstellen.</span><span class="sxs-lookup"><span data-stu-id="e154e-104">Create a new [page](../resources/page.md) in the specified section.</span></span>

## <a name="permissions"></a><span data-ttu-id="e154e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e154e-105">Permissions</span></span>
<span data-ttu-id="e154e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e154e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e154e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e154e-108">Permission type</span></span>      | <span data-ttu-id="e154e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e154e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e154e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e154e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e154e-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e154e-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e154e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e154e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e154e-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e154e-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e154e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e154e-114">Application</span></span> | <span data-ttu-id="e154e-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e154e-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e154e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e154e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="e154e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e154e-117">Request headers</span></span>
| <span data-ttu-id="e154e-118">Name</span><span class="sxs-lookup"><span data-stu-id="e154e-118">Name</span></span>       | <span data-ttu-id="e154e-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e154e-119">Type</span></span> | <span data-ttu-id="e154e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e154e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e154e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e154e-121">Authorization</span></span>  | <span data-ttu-id="e154e-122">string</span><span class="sxs-lookup"><span data-stu-id="e154e-122">string</span></span>  | <span data-ttu-id="e154e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e154e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e154e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e154e-125">Content-Type</span></span> | <span data-ttu-id="e154e-126">string</span><span class="sxs-lookup"><span data-stu-id="e154e-126">string</span></span> | <span data-ttu-id="e154e-p103">`text/html` oder `application/xhtml+xml` für den HTML-Inhalt, auch für den erforderlichen Teil „Präsentation“ von mehrteiligen Anforderungen. Mehrteilige Anforderungen verwenden den Inhaltstyp `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="e154e-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e154e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e154e-129">Request body</span></span>
<span data-ttu-id="e154e-130">Geben Sie im Anforderungstext den HTML-Inhalt für die Seite an.</span><span class="sxs-lookup"><span data-stu-id="e154e-130">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="e154e-p104">Der Text kann HTML-Code enthalten, der direkt im Anforderungstext platziert ist, oder er kann ein mehrteiliges Nachrichtenformat enthalten, wie im Beispiel gezeigt. Wenn Sie Binärdaten senden, müssen Sie eine mehrteilige Anforderung senden.</span><span class="sxs-lookup"><span data-stu-id="e154e-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="e154e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e154e-133">Response</span></span>

<span data-ttu-id="e154e-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein neues [page](../resources/page.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e154e-134">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e154e-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e154e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e154e-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e154e-136">Request</span></span>
<span data-ttu-id="e154e-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e154e-137">Here is an example of the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="e154e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="e154e-138">Response</span></span>
<span data-ttu-id="e154e-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e154e-139">Here is an example of the response.</span></span> <span data-ttu-id="e154e-140">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="e154e-140">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="e154e-141">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e154e-141">All of the properties will be returned from an actual call.</span></span>
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

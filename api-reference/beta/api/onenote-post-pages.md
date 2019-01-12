---
title: Seite erstellen
description: Dient zum Erstellen einer neuen OneNote-Seite im Standardabschnitt des Standardnotizbuchs.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d82971bdb3b1e8db4c89e69880681c43ab913939
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965208"
---
# <a name="create-page"></a><span data-ttu-id="166f7-103">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="166f7-103">Create page</span></span>

> <span data-ttu-id="166f7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="166f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="166f7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="166f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="166f7-106">Dient zum Erstellen einer neuen OneNote-Seite im Standardabschnitt des Standardnotizbuchs.</span><span class="sxs-lookup"><span data-stu-id="166f7-106">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="166f7-p102">Um eine Seite in einem anderen Abschnitt des Standardnotizbuchs zu erstellen, können Sie den Abfrageparameter `sectionName` verwenden.  Beispiel: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="166f7-p102">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.  Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="166f7-p103">Der `POST /onenote/pages`-Vorgang wird nur verwendet, um Seiten im Standardnotizbuch des aktuellen Benutzers zu erstellen. Wenn andere Notizbücher Ihr Ziel sind, können Sie [Seiten in einem angegebenen Abschnitt erstellen](../api/section-post-pages.md).</span><span class="sxs-lookup"><span data-stu-id="166f7-p103">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook. If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="166f7-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="166f7-111">Permissions</span></span>
<span data-ttu-id="166f7-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="166f7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="166f7-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="166f7-114">Permission type</span></span>      | <span data-ttu-id="166f7-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="166f7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="166f7-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="166f7-116">Delegated (work or school account)</span></span> | <span data-ttu-id="166f7-117">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="166f7-117">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="166f7-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="166f7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="166f7-119">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="166f7-119">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="166f7-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="166f7-120">Application</span></span> | <span data-ttu-id="166f7-121">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="166f7-121">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="166f7-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="166f7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="166f7-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="166f7-123">Request headers</span></span>  
| <span data-ttu-id="166f7-124">Name</span><span class="sxs-lookup"><span data-stu-id="166f7-124">Name</span></span>       | <span data-ttu-id="166f7-125">Typ</span><span class="sxs-lookup"><span data-stu-id="166f7-125">Type</span></span> | <span data-ttu-id="166f7-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="166f7-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="166f7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="166f7-127">Authorization</span></span>  | <span data-ttu-id="166f7-128">string</span><span class="sxs-lookup"><span data-stu-id="166f7-128">string</span></span>  | <span data-ttu-id="166f7-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="166f7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="166f7-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="166f7-131">Content-Type</span></span> | <span data-ttu-id="166f7-132">string</span><span class="sxs-lookup"><span data-stu-id="166f7-132">string</span></span> | <span data-ttu-id="166f7-p106">`text/html` oder `application/xhtml+xml` für den HTML-Inhalt, auch für den erforderlichen Teil „Präsentation“ von mehrteiligen Anforderungen. Mehrteilige Anforderungen verwenden den Inhaltstyp `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="166f7-p106">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="166f7-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="166f7-135">Request body</span></span>
<span data-ttu-id="166f7-136">Geben Sie im Anforderungstext den HTML-Inhalt für die Seite an.</span><span class="sxs-lookup"><span data-stu-id="166f7-136">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="166f7-p107">Der Text kann HTML-Code enthalten, der direkt im Anforderungstext platziert ist, oder er kann ein mehrteiliges Nachrichtenformat enthalten, wie im Beispiel gezeigt. Wenn Sie Binärdaten senden, müssen Sie eine mehrteilige Anforderung senden.</span><span class="sxs-lookup"><span data-stu-id="166f7-p107">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="166f7-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="166f7-139">Response</span></span>

<span data-ttu-id="166f7-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein neues [page](../resources/page.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="166f7-140">If successful, this method returns a `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="166f7-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="166f7-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="166f7-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="166f7-142">Request</span></span>
<span data-ttu-id="166f7-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="166f7-143">Here is an example of the request.</span></span>

<span data-ttu-id="166f7-p108">Im Pfad `../onenote/pages` können Sie den Abfrageparameter `sectionName` verwenden, um eine Seite in einem bestimmten Abschnitt des Standardnotizbuchs zu erstellen. Beispiel: `../onenote/pages?sectionName=My%20section`. Wenn der Abschnitt nicht vorhanden ist (oder umbenannt wurde), erstellt die API einen neuen Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="166f7-p108">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook. Example: `../onenote/pages?sectionName=My%20section`. If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages
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
##### <a name="response"></a><span data-ttu-id="166f7-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="166f7-147">Response</span></span>
<span data-ttu-id="166f7-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="166f7-148">Here is an example of the response.</span></span> <span data-ttu-id="166f7-149">Hinweis: Das hier gezeigte Response-Objekt wird aus Platzgründen Zahl gekürzt.</span><span class="sxs-lookup"><span data-stu-id="166f7-149">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="166f7-150">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="166f7-150">All of the properties will be returned from an actual call.</span></span>
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

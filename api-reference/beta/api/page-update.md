---
title: Seite aktualisieren
description: Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 91be57e33bba2d90725beaee8607fd3e2eddb84a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960694"
---
# <a name="update-page"></a><span data-ttu-id="33638-103">Seite aktualisieren</span><span class="sxs-lookup"><span data-stu-id="33638-103">Update page</span></span>

> <span data-ttu-id="33638-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33638-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33638-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33638-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33638-106">Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="33638-106">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="33638-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="33638-107">Permissions</span></span>
<span data-ttu-id="33638-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33638-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33638-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33638-110">Permission type</span></span>      | <span data-ttu-id="33638-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33638-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33638-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33638-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33638-113">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33638-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="33638-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33638-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33638-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33638-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="33638-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33638-116">Application</span></span> | <span data-ttu-id="33638-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33638-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33638-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33638-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="33638-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33638-119">Request headers</span></span>
| <span data-ttu-id="33638-120">Name</span><span class="sxs-lookup"><span data-stu-id="33638-120">Name</span></span>       | <span data-ttu-id="33638-121">Typ</span><span class="sxs-lookup"><span data-stu-id="33638-121">Type</span></span> | <span data-ttu-id="33638-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33638-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="33638-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33638-123">Authorization</span></span>  | <span data-ttu-id="33638-124">string</span><span class="sxs-lookup"><span data-stu-id="33638-124">string</span></span>  | <span data-ttu-id="33638-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="33638-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33638-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33638-127">Content-Type</span></span> | <span data-ttu-id="33638-128">string</span><span class="sxs-lookup"><span data-stu-id="33638-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="33638-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33638-129">Request body</span></span>
<span data-ttu-id="33638-130">Geben Sie im Textkörper Anforderung ein Array von [PatchContentCommand](../resources/patchcontentcommand.md) -Objekten, die Änderungen auf der Seite darstellen.</span><span class="sxs-lookup"><span data-stu-id="33638-130">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="33638-131">Weitere Informationen und Beispiele finden Sie unter [Update OneNote Seiteninhalt](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="33638-131">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="33638-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="33638-132">Response</span></span>

<span data-ttu-id="33638-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.  Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33638-p105">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="33638-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33638-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33638-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33638-136">Request</span></span>
<span data-ttu-id="33638-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33638-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="33638-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="33638-138">Response</span></span>
<span data-ttu-id="33638-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="33638-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

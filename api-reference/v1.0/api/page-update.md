---
title: Seite aktualisieren
description: Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.
ms.openlocfilehash: fd81e2c14db5a60fee9d0c8c5092c09957ed8421
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018160"
---
# <a name="update-page"></a><span data-ttu-id="acd1d-103">Seite aktualisieren</span><span class="sxs-lookup"><span data-stu-id="acd1d-103">Update page</span></span>

<span data-ttu-id="acd1d-104">Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="acd1d-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="acd1d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="acd1d-105">Permissions</span></span>
<span data-ttu-id="acd1d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acd1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd1d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acd1d-108">Permission type</span></span>      | <span data-ttu-id="acd1d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acd1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acd1d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acd1d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="acd1d-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acd1d-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="acd1d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acd1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acd1d-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acd1d-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="acd1d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acd1d-114">Application</span></span> | <span data-ttu-id="acd1d-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acd1d-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acd1d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acd1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="acd1d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acd1d-117">Request headers</span></span>
| <span data-ttu-id="acd1d-118">Name</span><span class="sxs-lookup"><span data-stu-id="acd1d-118">Name</span></span>       | <span data-ttu-id="acd1d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="acd1d-119">Type</span></span> | <span data-ttu-id="acd1d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acd1d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="acd1d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd1d-121">Authorization</span></span>  | <span data-ttu-id="acd1d-122">string</span><span class="sxs-lookup"><span data-stu-id="acd1d-122">string</span></span>  | <span data-ttu-id="acd1d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="acd1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="acd1d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="acd1d-125">Content-Type</span></span> | <span data-ttu-id="acd1d-126">string</span><span class="sxs-lookup"><span data-stu-id="acd1d-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="acd1d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acd1d-127">Request body</span></span>
<span data-ttu-id="acd1d-p103">Geben Sie im Anforderungstext ein Array von [patchContentCommand](../resources/patchcontentcommand.md)-Objekten an, die die Änderungen an der Seite darstellen. Weitere Informationen und Beispiele finden Sie im unter <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">OneNote-Seiten aktualisieren</a>.</span><span class="sxs-lookup"><span data-stu-id="acd1d-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="acd1d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="acd1d-130">Response</span></span>

<span data-ttu-id="acd1d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.  Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="acd1d-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="acd1d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acd1d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acd1d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acd1d-134">Request</span></span>
<span data-ttu-id="acd1d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acd1d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
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
##### <a name="response"></a><span data-ttu-id="acd1d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="acd1d-136">Response</span></span>
<span data-ttu-id="acd1d-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="acd1d-137">Here is an example of the response.</span></span> 
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
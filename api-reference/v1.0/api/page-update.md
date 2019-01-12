---
title: Seite aktualisieren
description: Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ef51342aba7bab49fde6d69ea0c77c62dc841b7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971711"
---
# <a name="update-page"></a><span data-ttu-id="69736-103">Seite aktualisieren</span><span class="sxs-lookup"><span data-stu-id="69736-103">Update page</span></span>

<span data-ttu-id="69736-104">Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="69736-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="69736-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="69736-105">Permissions</span></span>
<span data-ttu-id="69736-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69736-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69736-108">Permission type</span></span>      | <span data-ttu-id="69736-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69736-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69736-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69736-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69736-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69736-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="69736-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69736-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69736-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69736-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="69736-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69736-114">Application</span></span> | <span data-ttu-id="69736-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69736-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69736-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69736-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="69736-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69736-117">Request headers</span></span>
| <span data-ttu-id="69736-118">Name</span><span class="sxs-lookup"><span data-stu-id="69736-118">Name</span></span>       | <span data-ttu-id="69736-119">Typ</span><span class="sxs-lookup"><span data-stu-id="69736-119">Type</span></span> | <span data-ttu-id="69736-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69736-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69736-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69736-121">Authorization</span></span>  | <span data-ttu-id="69736-122">string</span><span class="sxs-lookup"><span data-stu-id="69736-122">string</span></span>  | <span data-ttu-id="69736-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="69736-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69736-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69736-125">Content-Type</span></span> | <span data-ttu-id="69736-126">string</span><span class="sxs-lookup"><span data-stu-id="69736-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="69736-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69736-127">Request body</span></span>
<span data-ttu-id="69736-p103">Geben Sie im Anforderungstext ein Array von [patchContentCommand](../resources/patchcontentcommand.md)-Objekten an, die die Änderungen an der Seite darstellen. Weitere Informationen und Beispiele finden Sie im unter <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">OneNote-Seiten aktualisieren</a>.</span><span class="sxs-lookup"><span data-stu-id="69736-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="69736-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="69736-130">Response</span></span>

<span data-ttu-id="69736-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.  Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69736-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="69736-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69736-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69736-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69736-134">Request</span></span>
<span data-ttu-id="69736-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69736-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="69736-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="69736-136">Response</span></span>
<span data-ttu-id="69736-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="69736-137">Here is an example of the response.</span></span> 
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

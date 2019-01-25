---
title: Seite aktualisieren
description: Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d80aae98828fa2ad07360e3a5b8d660e5d980b35
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519808"
---
# <a name="update-page"></a><span data-ttu-id="fe1b3-103">Seite aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fe1b3-103">Update page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe1b3-104">Mit dieser API können Sie den Inhalt einer OneNote-Seite aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="fe1b3-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe1b3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe1b3-105">Permissions</span></span>
<span data-ttu-id="fe1b3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe1b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe1b3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe1b3-108">Permission type</span></span>      | <span data-ttu-id="fe1b3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe1b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe1b3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe1b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe1b3-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe1b3-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe1b3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe1b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe1b3-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe1b3-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="fe1b3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe1b3-114">Application</span></span> | <span data-ttu-id="fe1b3-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe1b3-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe1b3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe1b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="fe1b3-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe1b3-117">Request headers</span></span>
| <span data-ttu-id="fe1b3-118">Name</span><span class="sxs-lookup"><span data-stu-id="fe1b3-118">Name</span></span>       | <span data-ttu-id="fe1b3-119">Typ</span><span class="sxs-lookup"><span data-stu-id="fe1b3-119">Type</span></span> | <span data-ttu-id="fe1b3-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe1b3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe1b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe1b3-121">Authorization</span></span>  | <span data-ttu-id="fe1b3-122">string</span><span class="sxs-lookup"><span data-stu-id="fe1b3-122">string</span></span>  | <span data-ttu-id="fe1b3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fe1b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe1b3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe1b3-125">Content-Type</span></span> | <span data-ttu-id="fe1b3-126">string</span><span class="sxs-lookup"><span data-stu-id="fe1b3-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="fe1b3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe1b3-127">Request body</span></span>
<span data-ttu-id="fe1b3-128">Geben Sie im Textkörper Anforderung ein Array von [PatchContentCommand](../resources/patchcontentcommand.md) -Objekten, die Änderungen auf der Seite darstellen.</span><span class="sxs-lookup"><span data-stu-id="fe1b3-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="fe1b3-129">Weitere Informationen und Beispiele finden Sie unter [Update OneNote Seiteninhalt](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="fe1b3-129">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="fe1b3-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe1b3-130">Response</span></span>

<span data-ttu-id="fe1b3-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.  Für eine PATCH-Anforderung werden keine JSON-Daten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe1b3-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="fe1b3-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe1b3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe1b3-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe1b3-134">Request</span></span>
<span data-ttu-id="fe1b3-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe1b3-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fe1b3-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe1b3-136">Response</span></span>
<span data-ttu-id="fe1b3-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fe1b3-137">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/page-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

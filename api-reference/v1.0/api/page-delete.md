---
title: Seite löschen
description: Mit dieser API können Sie OneNote-Seiten löschen.
ms.openlocfilehash: 574fa3a84a3ca18a788035e4a90bcc833907014e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017925"
---
# <a name="delete-page"></a><span data-ttu-id="53618-103">Seite löschen</span><span class="sxs-lookup"><span data-stu-id="53618-103">Delete page</span></span>

<span data-ttu-id="53618-104">Mit dieser API können Sie OneNote-Seiten löschen.</span><span class="sxs-lookup"><span data-stu-id="53618-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="53618-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53618-105">Permissions</span></span>
<span data-ttu-id="53618-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53618-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53618-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53618-108">Permission type</span></span>      | <span data-ttu-id="53618-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53618-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53618-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53618-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53618-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53618-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="53618-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53618-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53618-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53618-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="53618-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53618-114">Application</span></span> | <span data-ttu-id="53618-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53618-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53618-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53618-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="53618-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53618-117">Request headers</span></span>
| <span data-ttu-id="53618-118">Name</span><span class="sxs-lookup"><span data-stu-id="53618-118">Name</span></span>       | <span data-ttu-id="53618-119">Typ</span><span class="sxs-lookup"><span data-stu-id="53618-119">Type</span></span> | <span data-ttu-id="53618-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53618-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53618-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53618-121">Authorization</span></span>  | <span data-ttu-id="53618-122">string</span><span class="sxs-lookup"><span data-stu-id="53618-122">string</span></span>  | <span data-ttu-id="53618-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53618-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="53618-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="53618-125">Response</span></span>

<span data-ttu-id="53618-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53618-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53618-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53618-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53618-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53618-129">Request</span></span>
<span data-ttu-id="53618-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53618-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="53618-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="53618-131">Response</span></span>
<span data-ttu-id="53618-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53618-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
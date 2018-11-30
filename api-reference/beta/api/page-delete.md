---
title: Seite löschen
description: Mit dieser API können Sie OneNote-Seiten löschen.
ms.openlocfilehash: f2e566696937ee6f7808a66f994298802be66a17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059643"
---
# <a name="delete-page"></a><span data-ttu-id="07bba-103">Seite löschen</span><span class="sxs-lookup"><span data-stu-id="07bba-103">Delete page</span></span>

> <span data-ttu-id="07bba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07bba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07bba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07bba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07bba-106">Mit dieser API können Sie OneNote-Seiten löschen.</span><span class="sxs-lookup"><span data-stu-id="07bba-106">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="07bba-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07bba-107">Permissions</span></span>
<span data-ttu-id="07bba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07bba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07bba-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07bba-110">Permission type</span></span>      | <span data-ttu-id="07bba-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07bba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07bba-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07bba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07bba-113">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07bba-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="07bba-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07bba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07bba-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07bba-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="07bba-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07bba-116">Application</span></span> | <span data-ttu-id="07bba-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07bba-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07bba-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07bba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="07bba-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07bba-119">Request headers</span></span>
| <span data-ttu-id="07bba-120">Name</span><span class="sxs-lookup"><span data-stu-id="07bba-120">Name</span></span>       | <span data-ttu-id="07bba-121">Typ</span><span class="sxs-lookup"><span data-stu-id="07bba-121">Type</span></span> | <span data-ttu-id="07bba-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07bba-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="07bba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07bba-123">Authorization</span></span>  | <span data-ttu-id="07bba-124">string</span><span class="sxs-lookup"><span data-stu-id="07bba-124">string</span></span>  | <span data-ttu-id="07bba-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07bba-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="07bba-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="07bba-127">Response</span></span>

<span data-ttu-id="07bba-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07bba-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07bba-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07bba-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07bba-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07bba-131">Request</span></span>
<span data-ttu-id="07bba-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07bba-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="07bba-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="07bba-133">Response</span></span>
<span data-ttu-id="07bba-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="07bba-134">Here is an example of the response.</span></span>
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
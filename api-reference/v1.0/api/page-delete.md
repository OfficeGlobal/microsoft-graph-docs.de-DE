---
title: Seite löschen
description: Mit dieser API können Sie OneNote-Seiten löschen.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 691ec8d4d2f6c95c217a9ddb99fbd4e8608483f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962198"
---
# <a name="delete-page"></a><span data-ttu-id="89459-103">Seite löschen</span><span class="sxs-lookup"><span data-stu-id="89459-103">Delete page</span></span>

<span data-ttu-id="89459-104">Mit dieser API können Sie OneNote-Seiten löschen.</span><span class="sxs-lookup"><span data-stu-id="89459-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="89459-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="89459-105">Permissions</span></span>
<span data-ttu-id="89459-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89459-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89459-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89459-108">Permission type</span></span>      | <span data-ttu-id="89459-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89459-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89459-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89459-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89459-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89459-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="89459-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89459-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89459-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89459-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="89459-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89459-114">Application</span></span> | <span data-ttu-id="89459-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89459-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89459-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89459-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="89459-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89459-117">Request headers</span></span>
| <span data-ttu-id="89459-118">Name</span><span class="sxs-lookup"><span data-stu-id="89459-118">Name</span></span>       | <span data-ttu-id="89459-119">Typ</span><span class="sxs-lookup"><span data-stu-id="89459-119">Type</span></span> | <span data-ttu-id="89459-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89459-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89459-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="89459-121">Authorization</span></span>  | <span data-ttu-id="89459-122">string</span><span class="sxs-lookup"><span data-stu-id="89459-122">string</span></span>  | <span data-ttu-id="89459-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="89459-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="89459-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="89459-125">Response</span></span>

<span data-ttu-id="89459-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89459-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89459-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89459-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89459-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89459-129">Request</span></span>
<span data-ttu-id="89459-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89459-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="89459-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="89459-131">Response</span></span>
<span data-ttu-id="89459-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="89459-132">Here is an example of the response.</span></span>
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

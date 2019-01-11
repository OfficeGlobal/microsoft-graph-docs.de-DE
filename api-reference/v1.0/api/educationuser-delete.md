---
title: EducationUser löschen
description: Löscht einen Benutzer.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9fc544734d00ba713d6cb3f92020dfbb68a3857e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860354"
---
# <a name="delete-educationuser"></a><span data-ttu-id="5a92a-103">EducationUser löschen</span><span class="sxs-lookup"><span data-stu-id="5a92a-103">Delete educationUser</span></span>

<span data-ttu-id="5a92a-104">Löscht einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5a92a-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="5a92a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5a92a-105">Permissions</span></span>
<span data-ttu-id="5a92a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a92a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a92a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a92a-108">Permission type</span></span>      | <span data-ttu-id="5a92a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a92a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a92a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a92a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5a92a-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a92a-111">Not supported.</span></span>  |
|<span data-ttu-id="5a92a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a92a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5a92a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a92a-113">Not supported.</span></span>  |
|<span data-ttu-id="5a92a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a92a-114">Application</span></span> | <span data-ttu-id="5a92a-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a92a-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a92a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a92a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5a92a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a92a-117">Request headers</span></span>
| <span data-ttu-id="5a92a-118">Header</span><span class="sxs-lookup"><span data-stu-id="5a92a-118">Header</span></span>       | <span data-ttu-id="5a92a-119">Wert</span><span class="sxs-lookup"><span data-stu-id="5a92a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a92a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a92a-120">Authorization</span></span>  | <span data-ttu-id="5a92a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5a92a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a92a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a92a-123">Request body</span></span>
<span data-ttu-id="5a92a-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5a92a-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5a92a-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a92a-125">Response</span></span>
<span data-ttu-id="5a92a-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a92a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a92a-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a92a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a92a-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a92a-129">Request</span></span>
<span data-ttu-id="5a92a-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a92a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="5a92a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a92a-131">Response</span></span>
<span data-ttu-id="5a92a-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5a92a-132">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: EducationUser löschen
description: Löscht einen Benutzer.
ms.openlocfilehash: d9e3cab7d34cdf418b3553d69881bb951217ae22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017073"
---
# <a name="delete-educationuser"></a><span data-ttu-id="a7cf0-103">EducationUser löschen</span><span class="sxs-lookup"><span data-stu-id="a7cf0-103">Delete educationUser</span></span>

<span data-ttu-id="a7cf0-104">Löscht einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="a7cf0-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="a7cf0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a7cf0-105">Permissions</span></span>
<span data-ttu-id="a7cf0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7cf0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a7cf0-108">Permission type</span></span>      | <span data-ttu-id="a7cf0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a7cf0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7cf0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a7cf0-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a7cf0-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7cf0-111">Not supported.</span></span>  |
|<span data-ttu-id="a7cf0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a7cf0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a7cf0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a7cf0-113">Not supported.</span></span>  |
|<span data-ttu-id="a7cf0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a7cf0-114">Application</span></span> | <span data-ttu-id="a7cf0-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7cf0-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7cf0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7cf0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a7cf0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a7cf0-117">Request headers</span></span>
| <span data-ttu-id="a7cf0-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a7cf0-118">Header</span></span>       | <span data-ttu-id="a7cf0-119">Wert</span><span class="sxs-lookup"><span data-stu-id="a7cf0-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7cf0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7cf0-120">Authorization</span></span>  | <span data-ttu-id="a7cf0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a7cf0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7cf0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a7cf0-123">Request body</span></span>
<span data-ttu-id="a7cf0-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a7cf0-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a7cf0-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7cf0-125">Response</span></span>
<span data-ttu-id="a7cf0-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a7cf0-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7cf0-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a7cf0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7cf0-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a7cf0-129">Request</span></span>
<span data-ttu-id="a7cf0-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a7cf0-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="a7cf0-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a7cf0-131">Response</span></span>
<span data-ttu-id="a7cf0-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a7cf0-132">The following is an example of the response.</span></span> 
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
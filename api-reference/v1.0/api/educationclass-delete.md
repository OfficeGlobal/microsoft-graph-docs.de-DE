---
title: EducationClass löschen
description: Löschen einer Klasse. Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b94ff899d3787c61958739fe266d062097c08305
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973083"
---
# <a name="delete-educationclass"></a><span data-ttu-id="561c9-104">EducationClass löschen</span><span class="sxs-lookup"><span data-stu-id="561c9-104">Delete educationClass</span></span>

<span data-ttu-id="561c9-105">Löschen einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="561c9-105">Delete a class.</span></span> <span data-ttu-id="561c9-106">Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.</span><span class="sxs-lookup"><span data-stu-id="561c9-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="561c9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="561c9-107">Permissions</span></span>
<span data-ttu-id="561c9-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="561c9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="561c9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="561c9-110">Permission type</span></span>      | <span data-ttu-id="561c9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="561c9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="561c9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="561c9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="561c9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="561c9-113">Not supported.</span></span>  |
|<span data-ttu-id="561c9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="561c9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="561c9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="561c9-115">Not supported.</span></span>  |
|<span data-ttu-id="561c9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="561c9-116">Application</span></span> | <span data-ttu-id="561c9-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="561c9-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="561c9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="561c9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="561c9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="561c9-119">Request headers</span></span>
| <span data-ttu-id="561c9-120">Header</span><span class="sxs-lookup"><span data-stu-id="561c9-120">Header</span></span>       | <span data-ttu-id="561c9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="561c9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="561c9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="561c9-122">Authorization</span></span>  | <span data-ttu-id="561c9-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="561c9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="561c9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="561c9-125">Request body</span></span>
<span data-ttu-id="561c9-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="561c9-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="561c9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="561c9-127">Response</span></span>
<span data-ttu-id="561c9-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="561c9-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="561c9-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="561c9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="561c9-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="561c9-131">Request</span></span>
<span data-ttu-id="561c9-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="561c9-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="561c9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="561c9-133">Response</span></span>
<span data-ttu-id="561c9-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="561c9-134">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: EducationClass löschen
description: Löschen einer Klasse. Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.
ms.openlocfilehash: a0afd0175d1bfe79711e442182990ddb50088fb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016831"
---
# <a name="delete-educationclass"></a><span data-ttu-id="f86d4-104">EducationClass löschen</span><span class="sxs-lookup"><span data-stu-id="f86d4-104">Delete educationClass</span></span>

<span data-ttu-id="f86d4-105">Löschen einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="f86d4-105">Delete a class.</span></span> <span data-ttu-id="f86d4-106">Da eine Klasse auch eine universelle Gruppe ist, wird beim Löschen einer Klasse die Gruppe gelöscht.</span><span class="sxs-lookup"><span data-stu-id="f86d4-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f86d4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f86d4-107">Permissions</span></span>
<span data-ttu-id="f86d4-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f86d4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f86d4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f86d4-110">Permission type</span></span>      | <span data-ttu-id="f86d4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f86d4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f86d4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f86d4-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f86d4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f86d4-113">Not supported.</span></span>  |
|<span data-ttu-id="f86d4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f86d4-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f86d4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f86d4-115">Not supported.</span></span>  |
|<span data-ttu-id="f86d4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f86d4-116">Application</span></span> | <span data-ttu-id="f86d4-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f86d4-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f86d4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f86d4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f86d4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f86d4-119">Request headers</span></span>
| <span data-ttu-id="f86d4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f86d4-120">Header</span></span>       | <span data-ttu-id="f86d4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f86d4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f86d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f86d4-122">Authorization</span></span>  | <span data-ttu-id="f86d4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f86d4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f86d4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f86d4-125">Request body</span></span>
<span data-ttu-id="f86d4-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f86d4-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f86d4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f86d4-127">Response</span></span>
<span data-ttu-id="f86d4-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f86d4-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f86d4-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f86d4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f86d4-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f86d4-131">Request</span></span>
<span data-ttu-id="f86d4-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f86d4-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="f86d4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f86d4-133">Response</span></span>
<span data-ttu-id="f86d4-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f86d4-134">The following is an example of the response.</span></span> 

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
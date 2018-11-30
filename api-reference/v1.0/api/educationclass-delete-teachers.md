---
title: Lehrer entfernen
description: Entfernen eines Lehrers von einer Klasse.
ms.openlocfilehash: d0ae11901bf8e8cd05dd7705acad09a6604180fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019404"
---
# <a name="remove-teacher"></a><span data-ttu-id="de7f8-103">Lehrer entfernen</span><span class="sxs-lookup"><span data-stu-id="de7f8-103">Remove teacher</span></span>

<span data-ttu-id="de7f8-104">Entfernen eines Lehrers von einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="de7f8-104">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="de7f8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="de7f8-105">Permissions</span></span>
<span data-ttu-id="de7f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de7f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de7f8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de7f8-108">Permission type</span></span>      | <span data-ttu-id="de7f8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de7f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de7f8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de7f8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="de7f8-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de7f8-111">Not supported.</span></span>  |
|<span data-ttu-id="de7f8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de7f8-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="de7f8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de7f8-113">Not supported.</span></span>  |
|<span data-ttu-id="de7f8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de7f8-114">Application</span></span> | <span data-ttu-id="de7f8-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de7f8-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="de7f8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de7f8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="de7f8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de7f8-117">Request headers</span></span>
| <span data-ttu-id="de7f8-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="de7f8-118">Header</span></span>       | <span data-ttu-id="de7f8-119">Wert</span><span class="sxs-lookup"><span data-stu-id="de7f8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de7f8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de7f8-120">Authorization</span></span>  | <span data-ttu-id="de7f8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de7f8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de7f8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de7f8-123">Request body</span></span>
<span data-ttu-id="de7f8-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="de7f8-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="de7f8-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="de7f8-125">Response</span></span>
<span data-ttu-id="de7f8-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein leerer Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de7f8-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="de7f8-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de7f8-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de7f8-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de7f8-128">Request</span></span>
<span data-ttu-id="de7f8-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de7f8-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```

##### <a name="response"></a><span data-ttu-id="de7f8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="de7f8-130">Response</span></span>
<span data-ttu-id="de7f8-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="de7f8-131">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

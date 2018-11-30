---
title: EducationSchool löschen
description: Löschen einer Schule.
ms.openlocfilehash: 6ae69b725021c2a3e0a2776e8593c4346c5c6e34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061612"
---
# <a name="delete-educationschool"></a><span data-ttu-id="e0d7d-103">EducationSchool löschen</span><span class="sxs-lookup"><span data-stu-id="e0d7d-103">Delete educationSchool</span></span>

> <span data-ttu-id="e0d7d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e0d7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0d7d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e0d7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0d7d-106">Löschen einer Schule.</span><span class="sxs-lookup"><span data-stu-id="e0d7d-106">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0d7d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0d7d-107">Permissions</span></span>
<span data-ttu-id="e0d7d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0d7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0d7d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0d7d-110">Permission type</span></span>      | <span data-ttu-id="e0d7d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0d7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0d7d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0d7d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e0d7d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0d7d-113">Not supported.</span></span>  |
|<span data-ttu-id="e0d7d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0d7d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e0d7d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0d7d-115">Not supported.</span></span>  |
|<span data-ttu-id="e0d7d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0d7d-116">Application</span></span> | <span data-ttu-id="e0d7d-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0d7d-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e0d7d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0d7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e0d7d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0d7d-119">Request headers</span></span>
| <span data-ttu-id="e0d7d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e0d7d-120">Header</span></span>       | <span data-ttu-id="e0d7d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e0d7d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0d7d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0d7d-122">Authorization</span></span>  | <span data-ttu-id="e0d7d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0d7d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0d7d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0d7d-125">Request body</span></span>
<span data-ttu-id="e0d7d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e0d7d-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e0d7d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0d7d-127">Response</span></span>
<span data-ttu-id="e0d7d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0d7d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0d7d-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0d7d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0d7d-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0d7d-131">Request</span></span>
<span data-ttu-id="e0d7d-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0d7d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="e0d7d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0d7d-133">Response</span></span>
<span data-ttu-id="e0d7d-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0d7d-134">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
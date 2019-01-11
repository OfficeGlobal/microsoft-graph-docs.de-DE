---
title: EducationUser aus einer educationSchool entfernen
description: Löschen eines Benutzers aus einer Schule.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 4249ae683cab4dc2c9d42699f67dfbd5ca9c3ece
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865548"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="cea0c-103">EducationUser aus einer educationSchool entfernen</span><span class="sxs-lookup"><span data-stu-id="cea0c-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="cea0c-104">Löschen eines Benutzers aus einer Schule.</span><span class="sxs-lookup"><span data-stu-id="cea0c-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="cea0c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cea0c-105">Permissions</span></span>
<span data-ttu-id="cea0c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cea0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cea0c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cea0c-108">Permission type</span></span>      | <span data-ttu-id="cea0c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cea0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cea0c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cea0c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="cea0c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cea0c-111">Not supported.</span></span>  |
|<span data-ttu-id="cea0c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cea0c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cea0c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cea0c-113">Not supported.</span></span>  |
|<span data-ttu-id="cea0c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cea0c-114">Application</span></span> | <span data-ttu-id="cea0c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cea0c-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cea0c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cea0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cea0c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cea0c-117">Request headers</span></span>
| <span data-ttu-id="cea0c-118">Header</span><span class="sxs-lookup"><span data-stu-id="cea0c-118">Header</span></span>       | <span data-ttu-id="cea0c-119">Wert</span><span class="sxs-lookup"><span data-stu-id="cea0c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cea0c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cea0c-120">Authorization</span></span>  | <span data-ttu-id="cea0c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cea0c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cea0c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cea0c-123">Request body</span></span>
<span data-ttu-id="cea0c-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cea0c-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cea0c-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="cea0c-125">Response</span></span>
<span data-ttu-id="cea0c-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein leerer Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cea0c-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="cea0c-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cea0c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cea0c-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cea0c-128">Request</span></span>
<span data-ttu-id="cea0c-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cea0c-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```

##### <a name="response"></a><span data-ttu-id="cea0c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="cea0c-130">Response</span></span>
<span data-ttu-id="cea0c-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cea0c-131">The following is an example of the response.</span></span> 
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

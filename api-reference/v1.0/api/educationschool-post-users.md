---
title: EducationUser zu einer educationSchool hinzufügen
description: Hinzufügen eines Benutzers zu einer Schule.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e3c4284d17080dc8c46072117dd08c2fda08c662
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957267"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="53719-103">EducationUser zu einer educationSchool hinzufügen</span><span class="sxs-lookup"><span data-stu-id="53719-103">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="53719-104">Hinzufügen eines Benutzers zu einer Schule.</span><span class="sxs-lookup"><span data-stu-id="53719-104">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="53719-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53719-105">Permissions</span></span>
<span data-ttu-id="53719-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53719-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53719-108">Permission type</span></span>      | <span data-ttu-id="53719-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53719-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53719-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53719-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="53719-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53719-111">Not supported.</span></span>  |
|<span data-ttu-id="53719-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53719-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="53719-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53719-113">Not supported.</span></span>  |
|<span data-ttu-id="53719-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53719-114">Application</span></span> | <span data-ttu-id="53719-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53719-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="53719-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53719-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="53719-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53719-117">Request headers</span></span>
| <span data-ttu-id="53719-118">Header</span><span class="sxs-lookup"><span data-stu-id="53719-118">Header</span></span>       | <span data-ttu-id="53719-119">Wert</span><span class="sxs-lookup"><span data-stu-id="53719-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53719-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="53719-120">Authorization</span></span>  | <span data-ttu-id="53719-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53719-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="53719-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53719-123">Content-Type</span></span>  | <span data-ttu-id="53719-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53719-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53719-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53719-125">Request body</span></span>
<span data-ttu-id="53719-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="53719-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="53719-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="53719-127">Response</span></span>
<span data-ttu-id="53719-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53719-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53719-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53719-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53719-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53719-130">Request</span></span>
<span data-ttu-id="53719-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53719-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="53719-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="53719-132">Response</span></span>
<span data-ttu-id="53719-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53719-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

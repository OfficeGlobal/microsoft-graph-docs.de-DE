---
title: EducationUser zu einer educationSchool hinzufügen
description: Hinzufügen eines Benutzers zu einer Schule.
author: mmast-msft
ms.openlocfilehash: d7cabee054eddb6ac83bfdee5b0dea1ea25f9f36
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323079"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="94afd-103">EducationUser zu einer educationSchool hinzufügen</span><span class="sxs-lookup"><span data-stu-id="94afd-103">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="94afd-104">Hinzufügen eines Benutzers zu einer Schule.</span><span class="sxs-lookup"><span data-stu-id="94afd-104">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="94afd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="94afd-105">Permissions</span></span>
<span data-ttu-id="94afd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94afd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94afd-108">Permission type</span></span>      | <span data-ttu-id="94afd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94afd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94afd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94afd-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="94afd-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94afd-111">Not supported.</span></span>  |
|<span data-ttu-id="94afd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94afd-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="94afd-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94afd-113">Not supported.</span></span>  |
|<span data-ttu-id="94afd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94afd-114">Application</span></span> | <span data-ttu-id="94afd-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94afd-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="94afd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94afd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="94afd-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94afd-117">Request headers</span></span>
| <span data-ttu-id="94afd-118">Header</span><span class="sxs-lookup"><span data-stu-id="94afd-118">Header</span></span>       | <span data-ttu-id="94afd-119">Wert</span><span class="sxs-lookup"><span data-stu-id="94afd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94afd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="94afd-120">Authorization</span></span>  | <span data-ttu-id="94afd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="94afd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94afd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94afd-123">Content-Type</span></span>  | <span data-ttu-id="94afd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="94afd-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94afd-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94afd-125">Request body</span></span>
<span data-ttu-id="94afd-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="94afd-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="94afd-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="94afd-127">Response</span></span>
<span data-ttu-id="94afd-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94afd-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94afd-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94afd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94afd-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94afd-130">Request</span></span>
<span data-ttu-id="94afd-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94afd-131">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="94afd-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="94afd-132">Response</span></span>
<span data-ttu-id="94afd-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94afd-133">The following is an example of the response.</span></span> 

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
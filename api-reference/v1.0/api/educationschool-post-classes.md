---
title: EducationClass zu educationSchool hinzufügen
description: Hinzufügen einer Klasse zu einer Schule.
author: mmast-msft
ms.openlocfilehash: d5b32f1fabe40383f4c9d8dac79b52f85d9af4b0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303129"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="6a7ce-103">EducationClass zu educationSchool hinzufügen</span><span class="sxs-lookup"><span data-stu-id="6a7ce-103">Add educationClass to educationSchool</span></span>

<span data-ttu-id="6a7ce-104">Hinzufügen einer Klasse zu einer Schule.</span><span class="sxs-lookup"><span data-stu-id="6a7ce-104">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a7ce-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6a7ce-105">Permissions</span></span>
<span data-ttu-id="6a7ce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a7ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a7ce-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a7ce-108">Permission type</span></span>      | <span data-ttu-id="6a7ce-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a7ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a7ce-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a7ce-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6a7ce-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a7ce-111">Not supported.</span></span>  |
|<span data-ttu-id="6a7ce-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a7ce-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6a7ce-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a7ce-113">Not supported.</span></span>  |
|<span data-ttu-id="6a7ce-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a7ce-114">Application</span></span> | <span data-ttu-id="6a7ce-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a7ce-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6a7ce-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a7ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6a7ce-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a7ce-117">Request headers</span></span>
| <span data-ttu-id="6a7ce-118">Header</span><span class="sxs-lookup"><span data-stu-id="6a7ce-118">Header</span></span>       | <span data-ttu-id="6a7ce-119">Wert</span><span class="sxs-lookup"><span data-stu-id="6a7ce-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6a7ce-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a7ce-120">Authorization</span></span>  | <span data-ttu-id="6a7ce-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a7ce-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6a7ce-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a7ce-123">Content-Type</span></span>  | <span data-ttu-id="6a7ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6a7ce-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a7ce-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a7ce-125">Request body</span></span>
<span data-ttu-id="6a7ce-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationClass](../resources/educationclass.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6a7ce-126">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="6a7ce-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a7ce-127">Response</span></span>
<span data-ttu-id="6a7ce-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `204 No Content` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a7ce-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a7ce-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a7ce-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a7ce-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a7ce-130">Request</span></span>
<span data-ttu-id="6a7ce-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a7ce-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/v1.0/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="6a7ce-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a7ce-132">Response</span></span> 
<span data-ttu-id="6a7ce-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6a7ce-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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
---
title: EducationCategory abrufen
description: Ruft ein Category-Objekt ab.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a26edfd8fe3296f92c7f62b40eea7d3be35722a5
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801001"
---
# <a name="get-educationcategory"></a><span data-ttu-id="a0fd0-103">EducationCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="a0fd0-103">Get educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0fd0-104">Ruft ein [educationCategory](../resources/educationcategory.md) -Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="a0fd0-104">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0fd0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a0fd0-105">Permissions</span></span>
<span data-ttu-id="a0fd0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0fd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0fd0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0fd0-108">Permission type</span></span>      | <span data-ttu-id="a0fd0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0fd0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0fd0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0fd0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0fd0-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0fd0-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="a0fd0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0fd0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a0fd0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0fd0-113">Not supported.</span></span>  |
|<span data-ttu-id="a0fd0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0fd0-114">Application</span></span> | <span data-ttu-id="a0fd0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0fd0-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a0fd0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0fd0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0fd0-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a0fd0-117">Optional query parameters</span></span>
<span data-ttu-id="a0fd0-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0fd0-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0fd0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0fd0-119">Request headers</span></span>
| <span data-ttu-id="a0fd0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a0fd0-120">Header</span></span>       | <span data-ttu-id="a0fd0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a0fd0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0fd0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0fd0-122">Authorization</span></span>  | <span data-ttu-id="a0fd0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a0fd0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0fd0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0fd0-125">Request body</span></span>
<span data-ttu-id="a0fd0-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a0fd0-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a0fd0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0fd0-127">Response</span></span>
<span data-ttu-id="a0fd0-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [educationCategory](../resources/educationcategory.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a0fd0-128">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0fd0-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0fd0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0fd0-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0fd0-130">Request</span></span>
<span data-ttu-id="a0fd0-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a0fd0-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignmentCategories/<id>
```
##### <a name="response"></a><span data-ttu-id="a0fd0-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0fd0-132">Response</span></span>
<span data-ttu-id="a0fd0-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0fd0-133">The following is an example of the response.</span></span> 

><span data-ttu-id="a0fd0-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a0fd0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get category",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-get-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

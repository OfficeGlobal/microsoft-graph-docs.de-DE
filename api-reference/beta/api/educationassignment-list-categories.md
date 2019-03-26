---
title: Kategorien auflisten
description: Listet alle Kategorien auf, die dieser Zuordnung zugeordnet sind.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 925b2f558b98e50cfcebd7b68c3af52452f2e3df
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801004"
---
# <a name="list-categories"></a><span data-ttu-id="d918d-103">Kategorien auflisten</span><span class="sxs-lookup"><span data-stu-id="d918d-103">List categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d918d-104">Listet alle Kategorien auf, die dieser Zuordnung zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="d918d-104">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="d918d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d918d-105">Permissions</span></span>
<span data-ttu-id="d918d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d918d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d918d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d918d-108">Permission type</span></span>      | <span data-ttu-id="d918d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d918d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d918d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d918d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d918d-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d918d-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d918d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d918d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d918d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d918d-113">Not supported.</span></span>  |
|<span data-ttu-id="d918d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d918d-114">Application</span></span> | <span data-ttu-id="d918d-115">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d918d-115">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d918d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d918d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d918d-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d918d-117">Optional query parameters</span></span>
<span data-ttu-id="d918d-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d918d-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d918d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d918d-119">Request headers</span></span>
| <span data-ttu-id="d918d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d918d-120">Header</span></span>       | <span data-ttu-id="d918d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d918d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d918d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d918d-122">Authorization</span></span>  | <span data-ttu-id="d918d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d918d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d918d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d918d-125">Request body</span></span>
<span data-ttu-id="d918d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d918d-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d918d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d918d-127">Response</span></span>
<span data-ttu-id="d918d-128">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [educationCategory](../resources/educationcategory.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d918d-128">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d918d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d918d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d918d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d918d-130">Request</span></span>
<span data-ttu-id="d918d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d918d-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="d918d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d918d-132">Response</span></span>
<span data-ttu-id="d918d-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d918d-133">The following is an example of the response.</span></span> 

><span data-ttu-id="d918d-134">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="d918d-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d918d-135">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d918d-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-categories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

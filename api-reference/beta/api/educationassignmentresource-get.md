---
title: Abrufen von educationAssignmentResource
description: 'Rufen Sie die Eigenschaften einer bestimmten Ressource an einer Zuordnung.  '
author: dipakboyed
ms.openlocfilehash: 25c448f3247631c9129a837bd00842588bf152d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358814"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="2d3a4-103">Abrufen von educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="2d3a4-103">Get educationAssignmentResource</span></span>

> <span data-ttu-id="2d3a4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d3a4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d3a4-106">Rufen Sie die Eigenschaften einer bestimmten Ressource an einer Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-106">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="2d3a4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2d3a4-107">Permissions</span></span>
<span data-ttu-id="2d3a4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d3a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d3a4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d3a4-110">Permission type</span></span>      | <span data-ttu-id="2d3a4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d3a4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d3a4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d3a4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d3a4-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d3a4-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="2d3a4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d3a4-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2d3a4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d3a4-115">Not supported.</span></span>  |
|<span data-ttu-id="2d3a4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d3a4-116">Application</span></span> |  <span data-ttu-id="2d3a4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d3a4-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2d3a4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d3a4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d3a4-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2d3a4-119">Optional query parameters</span></span>
<span data-ttu-id="2d3a4-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d3a4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d3a4-121">Request headers</span></span>
| <span data-ttu-id="2d3a4-122">Header</span><span class="sxs-lookup"><span data-stu-id="2d3a4-122">Header</span></span>       | <span data-ttu-id="2d3a4-123">Wert</span><span class="sxs-lookup"><span data-stu-id="2d3a4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d3a4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d3a4-124">Authorization</span></span>  | <span data-ttu-id="2d3a4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d3a4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d3a4-127">Request body</span></span>
<span data-ttu-id="2d3a4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2d3a4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d3a4-129">Response</span></span>
<span data-ttu-id="2d3a4-130">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationAssignmentResource](../resources/educationassignmentresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d3a4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d3a4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d3a4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d3a4-132">Request</span></span>
<span data-ttu-id="2d3a4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="2d3a4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d3a4-134">Response</span></span>
<span data-ttu-id="2d3a4-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2d3a4-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2d3a4-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d3a4-137">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
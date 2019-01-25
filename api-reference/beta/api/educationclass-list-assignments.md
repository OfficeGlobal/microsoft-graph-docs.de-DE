---
title: Liste Zuordnungen
description: Abrufen einer Liste von Assignment-Objekten. Lehrer ist zulässig, um alle Assignment-Objekten für die Klasse finden Sie unter. Studenten können nur Arbeitsaufträge angezeigt, die ihnen zugewiesen sind.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7cd47c61d4958d42ce099396147d421a6555041b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519143"
---
# <a name="list-assignments"></a><span data-ttu-id="f66c1-105">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="f66c1-105">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f66c1-106">Abrufen einer Liste von Assignment-Objekten.</span><span class="sxs-lookup"><span data-stu-id="f66c1-106">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="f66c1-107">Lehrer ist zulässig, um alle Assignment-Objekten für die Klasse finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="f66c1-107">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="f66c1-108">Studenten können nur Arbeitsaufträge angezeigt, die ihnen zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="f66c1-108">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="f66c1-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f66c1-109">Permissions</span></span>
<span data-ttu-id="f66c1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f66c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f66c1-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f66c1-112">Permission type</span></span>      | <span data-ttu-id="f66c1-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f66c1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f66c1-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f66c1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f66c1-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f66c1-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="f66c1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f66c1-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f66c1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f66c1-117">Not supported.</span></span>  |
|<span data-ttu-id="f66c1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f66c1-118">Application</span></span> | <span data-ttu-id="f66c1-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f66c1-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f66c1-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f66c1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f66c1-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f66c1-121">Optional query parameters</span></span>
<span data-ttu-id="f66c1-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f66c1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f66c1-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f66c1-123">Request headers</span></span>
| <span data-ttu-id="f66c1-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f66c1-124">Header</span></span>       | <span data-ttu-id="f66c1-125">Wert</span><span class="sxs-lookup"><span data-stu-id="f66c1-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f66c1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f66c1-126">Authorization</span></span>  | <span data-ttu-id="f66c1-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f66c1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f66c1-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f66c1-129">Request body</span></span>
<span data-ttu-id="f66c1-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f66c1-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f66c1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f66c1-131">Response</span></span>
<span data-ttu-id="f66c1-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f66c1-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f66c1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f66c1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f66c1-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f66c1-134">Request</span></span>
<span data-ttu-id="f66c1-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f66c1-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="f66c1-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f66c1-136">Response</span></span>
<span data-ttu-id="f66c1-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f66c1-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f66c1-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f66c1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
  "value": [
    {
      "id": "19002",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-02-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-02-01T00:00:00Z",
      "classId": "11018",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "createdDateTime": "2014-02-01T00:00:00Z",
      "displayName": "published",
      "dueDateTime": "2014-02-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "contentType": "Text",
        "content": "Read chapters 1 through 3"
      },
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2014-02-01T00:00:00Z",
      "status": "published"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

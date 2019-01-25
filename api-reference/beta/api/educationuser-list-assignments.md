---
title: Liste Zuordnungen
description: Gibt eine Liste der Zuordnungen für einen Benutzer für alle Klassen zugewiesen. Dieser Namespace Dienstprogramm kann Anrufer, in einem einzigen Aufruf und erspart Zuordnungen von jede Klasse Anfordern einer Student Zuordnungen zu erhalten. Die Zuordnung Liste enthält, was benötigt wird, um die detaillierten Informationen für die Zuordnung von innerhalb der Klassennamespace abzurufen. Alle anderen Operationen für die Zuordnung sollten den Klassennamespace verwenden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e2e11eb94c07fc523d6d64143ffc3df401fd9906
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515979"
---
# <a name="list-assignments"></a><span data-ttu-id="8cf75-106">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="8cf75-106">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cf75-107">Gibt eine Liste der Zuordnungen für einen Benutzer für alle Klassen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="8cf75-107">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="8cf75-108">Dieser Namespace Dienstprogramm kann Anrufer, in einem einzigen Aufruf und erspart Zuordnungen von jede Klasse Anfordern einer Student Zuordnungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="8cf75-108">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="8cf75-109">Die Zuordnung Liste enthält, was benötigt wird, um die detaillierten Informationen für die Zuordnung von innerhalb der Klassennamespace abzurufen.</span><span class="sxs-lookup"><span data-stu-id="8cf75-109">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="8cf75-110">Alle anderen Operationen für die Zuordnung sollten den Klassennamespace verwenden.</span><span class="sxs-lookup"><span data-stu-id="8cf75-110">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cf75-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8cf75-111">Permissions</span></span>
<span data-ttu-id="8cf75-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cf75-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cf75-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8cf75-114">Permission type</span></span>      | <span data-ttu-id="8cf75-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8cf75-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cf75-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8cf75-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8cf75-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8cf75-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8cf75-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8cf75-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cf75-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8cf75-119">Not supported.</span></span>   |
|<span data-ttu-id="8cf75-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8cf75-120">Application</span></span> | <span data-ttu-id="8cf75-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8cf75-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8cf75-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8cf75-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8cf75-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8cf75-123">Optional query parameters</span></span>
<span data-ttu-id="8cf75-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8cf75-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cf75-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8cf75-125">Request headers</span></span>
| <span data-ttu-id="8cf75-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8cf75-126">Header</span></span>       | <span data-ttu-id="8cf75-127">Wert</span><span class="sxs-lookup"><span data-stu-id="8cf75-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8cf75-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cf75-128">Authorization</span></span>  | <span data-ttu-id="8cf75-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8cf75-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8cf75-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8cf75-131">Request body</span></span>
<span data-ttu-id="8cf75-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8cf75-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8cf75-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8cf75-133">Response</span></span>
<span data-ttu-id="8cf75-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8cf75-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cf75-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8cf75-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cf75-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8cf75-136">Request</span></span>
<span data-ttu-id="8cf75-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8cf75-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="8cf75-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="8cf75-138">Response</span></span>
<span data-ttu-id="8cf75-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8cf75-139">The following is an example of the response.</span></span> 

><span data-ttu-id="8cf75-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8cf75-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "assignDateTime": "2014-01-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-01-01T00:00:00Z",
      "classId": "11010",
      "createdBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "createdDateTime": "2014-01-01T00:00:00Z",
      "displayName": "Assignment 1",
      "dueDateTime": "2014-01-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "content": "Answer every question correctly",
        "contentType": "Text"
      },
      "lastModifiedBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "lastModifiedDateTime": "2014-01-01T00:00:00Z",
      "status": "assigned"
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
    "Error: /api-reference/beta/api/educationuser-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

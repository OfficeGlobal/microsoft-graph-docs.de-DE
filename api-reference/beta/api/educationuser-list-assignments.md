---
title: Liste Zuordnungen
description: Gibt eine Liste der Zuordnungen für einen Benutzer für alle Klassen zugewiesen. Dieser Namespace Dienstprogramm kann Anrufer, in einem einzigen Aufruf und erspart Zuordnungen von jede Klasse Anfordern einer Student Zuordnungen zu erhalten. Die Zuordnung Liste enthält, was benötigt wird, um die detaillierten Informationen für die Zuordnung von innerhalb der Klassennamespace abzurufen. Alle anderen Operationen für die Zuordnung sollten den Klassennamespace verwenden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0366a159e3e28e9ad3933ec4d1eea6799c1f65c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940841"
---
# <a name="list-assignments"></a><span data-ttu-id="12f78-106">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="12f78-106">List assignments</span></span>

> <span data-ttu-id="12f78-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12f78-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12f78-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12f78-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12f78-109">Gibt eine Liste der Zuordnungen für einen Benutzer für alle Klassen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="12f78-109">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="12f78-110">Dieser Namespace Dienstprogramm kann Anrufer, in einem einzigen Aufruf und erspart Zuordnungen von jede Klasse Anfordern einer Student Zuordnungen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="12f78-110">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="12f78-111">Die Zuordnung Liste enthält, was benötigt wird, um die detaillierten Informationen für die Zuordnung von innerhalb der Klassennamespace abzurufen.</span><span class="sxs-lookup"><span data-stu-id="12f78-111">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="12f78-112">Alle anderen Operationen für die Zuordnung sollten den Klassennamespace verwenden.</span><span class="sxs-lookup"><span data-stu-id="12f78-112">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="12f78-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12f78-113">Permissions</span></span>
<span data-ttu-id="12f78-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12f78-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f78-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12f78-116">Permission type</span></span>      | <span data-ttu-id="12f78-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12f78-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12f78-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12f78-118">Delegated (work or school account)</span></span> | <span data-ttu-id="12f78-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12f78-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="12f78-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12f78-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12f78-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12f78-121">Not supported.</span></span>   |
|<span data-ttu-id="12f78-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12f78-122">Application</span></span> | <span data-ttu-id="12f78-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12f78-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="12f78-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12f78-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12f78-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="12f78-125">Optional query parameters</span></span>
<span data-ttu-id="12f78-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="12f78-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12f78-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12f78-127">Request headers</span></span>
| <span data-ttu-id="12f78-128">Header</span><span class="sxs-lookup"><span data-stu-id="12f78-128">Header</span></span>       | <span data-ttu-id="12f78-129">Wert</span><span class="sxs-lookup"><span data-stu-id="12f78-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12f78-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="12f78-130">Authorization</span></span>  | <span data-ttu-id="12f78-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12f78-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12f78-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12f78-133">Request body</span></span>
<span data-ttu-id="12f78-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="12f78-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="12f78-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="12f78-135">Response</span></span>
<span data-ttu-id="12f78-136">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="12f78-136">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12f78-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12f78-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12f78-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12f78-138">Request</span></span>
<span data-ttu-id="12f78-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="12f78-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="12f78-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="12f78-140">Response</span></span>
<span data-ttu-id="12f78-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="12f78-141">The following is an example of the response.</span></span> 

><span data-ttu-id="12f78-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="12f78-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

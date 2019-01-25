---
title: Abrufen von educationAssignment
description: " Lehrer können alle Zuordnungen in einer Klasse finden Sie unter."
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eba959dcaf2478f3c49fc0fbb434d7269e37e5ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508370"
---
# <a name="get-educationassignment"></a><span data-ttu-id="be965-103">Abrufen von educationAssignment</span><span class="sxs-lookup"><span data-stu-id="be965-103">Get educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be965-104">Rufen Sie die Eigenschaften und Beziehungen einer Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="be965-104">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="be965-105">Studenten können nur ihnen zugewiesene Aufgaben anzeigen. Lehrer können alle Zuordnungen in einer Klasse finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="be965-105">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="be965-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be965-106">Permissions</span></span>
<span data-ttu-id="be965-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be965-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="be965-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be965-109">Permission type</span></span>      | <span data-ttu-id="be965-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be965-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be965-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be965-111">Delegated (work or school account)</span></span> | <span data-ttu-id="be965-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be965-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="be965-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be965-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="be965-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be965-114">Not supported.</span></span>  |
|<span data-ttu-id="be965-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be965-115">Application</span></span> | <span data-ttu-id="be965-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be965-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="be965-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be965-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be965-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="be965-118">Optional query parameters</span></span>
<span data-ttu-id="be965-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be965-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be965-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be965-120">Request headers</span></span>
| <span data-ttu-id="be965-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="be965-121">Header</span></span>       | <span data-ttu-id="be965-122">Wert</span><span class="sxs-lookup"><span data-stu-id="be965-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be965-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be965-123">Authorization</span></span>  | <span data-ttu-id="be965-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="be965-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be965-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be965-126">Request body</span></span>
<span data-ttu-id="be965-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="be965-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be965-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="be965-128">Response</span></span>
<span data-ttu-id="be965-129">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationAssignment](../resources/educationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="be965-129">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be965-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be965-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be965-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be965-131">Request</span></span>
<span data-ttu-id="be965-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be965-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="be965-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="be965-133">Response</span></span>
<span data-ttu-id="be965-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be965-134">The following is an example of the response.</span></span> 

><span data-ttu-id="be965-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="be965-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
      "maxPoints": 100
  },
  "instructions": {
    "content": "Answer every question correctly",
    "contentType": "Text"
  },
  "lastModifiedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

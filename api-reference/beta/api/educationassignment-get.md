---
title: Abrufen von educationAssignment
description: " Lehrer können alle Zuordnungen in einer Klasse finden Sie unter."
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 66279d72952a561a5e98be00ae268ca58c5dcc92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976401"
---
# <a name="get-educationassignment"></a><span data-ttu-id="cdd8e-103">Abrufen von educationAssignment</span><span class="sxs-lookup"><span data-stu-id="cdd8e-103">Get educationAssignment</span></span>

> <span data-ttu-id="cdd8e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdd8e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cdd8e-106">Rufen Sie die Eigenschaften und Beziehungen einer Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-106">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="cdd8e-107">Studenten können nur ihnen zugewiesene Aufgaben anzeigen. Lehrer können alle Zuordnungen in einer Klasse finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-107">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdd8e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cdd8e-108">Permissions</span></span>
<span data-ttu-id="cdd8e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdd8e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cdd8e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cdd8e-111">Permission type</span></span>      | <span data-ttu-id="cdd8e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cdd8e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdd8e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cdd8e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cdd8e-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdd8e-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="cdd8e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cdd8e-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cdd8e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cdd8e-116">Not supported.</span></span>  |
|<span data-ttu-id="cdd8e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cdd8e-117">Application</span></span> | <span data-ttu-id="cdd8e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cdd8e-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="cdd8e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cdd8e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cdd8e-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cdd8e-120">Optional query parameters</span></span>
<span data-ttu-id="cdd8e-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdd8e-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cdd8e-122">Request headers</span></span>
| <span data-ttu-id="cdd8e-123">Header</span><span class="sxs-lookup"><span data-stu-id="cdd8e-123">Header</span></span>       | <span data-ttu-id="cdd8e-124">Wert</span><span class="sxs-lookup"><span data-stu-id="cdd8e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdd8e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdd8e-125">Authorization</span></span>  | <span data-ttu-id="cdd8e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdd8e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cdd8e-128">Request body</span></span>
<span data-ttu-id="cdd8e-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdd8e-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="cdd8e-130">Response</span></span>
<span data-ttu-id="cdd8e-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationAssignment](../resources/educationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdd8e-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cdd8e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdd8e-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cdd8e-133">Request</span></span>
<span data-ttu-id="cdd8e-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="cdd8e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cdd8e-135">Response</span></span>
<span data-ttu-id="cdd8e-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-136">The following is an example of the response.</span></span> 

><span data-ttu-id="cdd8e-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cdd8e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

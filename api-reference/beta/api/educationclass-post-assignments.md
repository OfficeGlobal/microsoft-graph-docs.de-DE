---
title: Erstellen von educationAssignment
description: 'Erstellt eine neue Zuordnung. Nur Lehrer in einer Klasse können eine Zuordnung erstellen. Zuordnungen starten Sie den Status Entwurf, was bedeutet, dass die Zuordnung von Studenten nicht angezeigt werden, bis veröffentlichen aufgerufen wird.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4a7f7da89343156267a307c66abe73b4a352da17
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519556"
---
# <a name="create-educationassignment"></a><span data-ttu-id="50ffd-105">Erstellen von educationAssignment</span><span class="sxs-lookup"><span data-stu-id="50ffd-105">Create educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50ffd-106">Erstellt eine neue Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="50ffd-106">Creates a new assignment.</span></span> <span data-ttu-id="50ffd-107">Nur Lehrer in einer Klasse können eine Zuordnung erstellen.</span><span class="sxs-lookup"><span data-stu-id="50ffd-107">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="50ffd-108">Zuordnungen starten Sie den Status Entwurf, was bedeutet, dass die Zuordnung von Studenten nicht angezeigt werden, bis veröffentlichen aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="50ffd-108">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="50ffd-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="50ffd-109">Permissions</span></span>
<span data-ttu-id="50ffd-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50ffd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ffd-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50ffd-112">Permission type</span></span>      | <span data-ttu-id="50ffd-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50ffd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50ffd-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50ffd-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="50ffd-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50ffd-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="50ffd-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50ffd-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="50ffd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50ffd-117">Not supported.</span></span>  |
|<span data-ttu-id="50ffd-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50ffd-118">Application</span></span> | <span data-ttu-id="50ffd-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50ffd-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="50ffd-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50ffd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="50ffd-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50ffd-121">Request headers</span></span>
| <span data-ttu-id="50ffd-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="50ffd-122">Header</span></span>       | <span data-ttu-id="50ffd-123">Wert</span><span class="sxs-lookup"><span data-stu-id="50ffd-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50ffd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="50ffd-124">Authorization</span></span>  | <span data-ttu-id="50ffd-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50ffd-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50ffd-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50ffd-127">Content-Type</span></span>  | <span data-ttu-id="50ffd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="50ffd-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50ffd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50ffd-129">Request body</span></span>
<span data-ttu-id="50ffd-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [EducationAssignment](../resources/educationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="50ffd-130">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="50ffd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="50ffd-131">Response</span></span>
<span data-ttu-id="50ffd-132">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201 Created` Antwortcode und eines [EducationAssignment](../resources/educationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="50ffd-132">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50ffd-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50ffd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50ffd-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50ffd-134">Request</span></span>
<span data-ttu-id="50ffd-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50ffd-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignment_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignments
Content-type: application/json
Content-length: 279

{ 
  "dueDateTime": "2014-02-01T00:00:00Z",
  "displayName": "Midterm 1",
    "instructions":  {
      "contentType": "Text",
      "content": "Read chapters 1 through 3"
    },
      "grading": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "assignTo": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentClassRecipient"
      },
      "status":"draft",
      "allowStudentsToAddResourcesToSubmission": true
}
```
<span data-ttu-id="50ffd-136">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [EducationAssignment](../resources/educationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="50ffd-136">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="50ffd-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="50ffd-137">Response</span></span>
<span data-ttu-id="50ffd-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="50ffd-138">The following is an example of the response.</span></span> 

><span data-ttu-id="50ffd-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="50ffd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 279

{
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-post-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

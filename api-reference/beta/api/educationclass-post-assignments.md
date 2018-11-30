---
title: Erstellen von educationAssignment
description: 'Erstellt eine neue Zuordnung. Nur Lehrer in einer Klasse können eine Zuordnung erstellen. Zuordnungen starten Sie den Status Entwurf, was bedeutet, dass die Zuordnung von Studenten nicht angezeigt werden, bis veröffentlichen aufgerufen wird.  '
ms.openlocfilehash: 9a6af2a0c0689ca2118ce4d06a55d7b27a70a4ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060317"
---
# <a name="create-educationassignment"></a><span data-ttu-id="48595-105">Erstellen von educationAssignment</span><span class="sxs-lookup"><span data-stu-id="48595-105">Create educationAssignment</span></span>

> <span data-ttu-id="48595-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="48595-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48595-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48595-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48595-108">Erstellt eine neue Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="48595-108">Creates a new assignment.</span></span> <span data-ttu-id="48595-109">Nur Lehrer in einer Klasse können eine Zuordnung erstellen.</span><span class="sxs-lookup"><span data-stu-id="48595-109">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="48595-110">Zuordnungen starten Sie den Status Entwurf, was bedeutet, dass die Zuordnung von Studenten nicht angezeigt werden, bis veröffentlichen aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="48595-110">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="48595-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48595-111">Permissions</span></span>
<span data-ttu-id="48595-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48595-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48595-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48595-114">Permission type</span></span>      | <span data-ttu-id="48595-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48595-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48595-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48595-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="48595-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48595-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="48595-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48595-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="48595-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48595-119">Not supported.</span></span>  |
|<span data-ttu-id="48595-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48595-120">Application</span></span> | <span data-ttu-id="48595-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48595-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="48595-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48595-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="48595-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48595-123">Request headers</span></span>
| <span data-ttu-id="48595-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="48595-124">Header</span></span>       | <span data-ttu-id="48595-125">Wert</span><span class="sxs-lookup"><span data-stu-id="48595-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48595-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="48595-126">Authorization</span></span>  | <span data-ttu-id="48595-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48595-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48595-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48595-129">Content-Type</span></span>  | <span data-ttu-id="48595-130">application/json</span><span class="sxs-lookup"><span data-stu-id="48595-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48595-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48595-131">Request body</span></span>
<span data-ttu-id="48595-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [EducationAssignment](../resources/educationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="48595-132">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="48595-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="48595-133">Response</span></span>
<span data-ttu-id="48595-134">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201 Created` Antwortcode und eines [EducationAssignment](../resources/educationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="48595-134">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48595-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48595-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48595-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48595-136">Request</span></span>
<span data-ttu-id="48595-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48595-137">The following is an example of the request.</span></span>
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
<span data-ttu-id="48595-138">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [EducationAssignment](../resources/educationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="48595-138">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="48595-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="48595-139">Response</span></span>
<span data-ttu-id="48595-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48595-140">The following is an example of the response.</span></span> 

><span data-ttu-id="48595-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="48595-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
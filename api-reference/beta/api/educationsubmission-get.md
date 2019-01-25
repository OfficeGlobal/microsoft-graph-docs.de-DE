---
title: Abrufen von educationSubmission
description: 'Abrufen einer bestimmten Übermittlung an. Eine Übermittlung-Objekt stellt einen Schüler Arbeit für eine Zuordnung dar. Ressourcen im Zusammenhang mit der Übermittlung darstellen diese arbeiten. Nur der Student, die Übermittlung zugewiesen ist, kann finden Sie unter und die Übermittlung geändert werden. Lehrer verfügt über Vollzugriff auf alle Übermittlungen. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d0542bec537b8317a46e98c215768f5228f9a07c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511954"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="1afaa-107">Abrufen von educationSubmission</span><span class="sxs-lookup"><span data-stu-id="1afaa-107">Get educationSubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1afaa-108">Abrufen einer bestimmten Übermittlung an.</span><span class="sxs-lookup"><span data-stu-id="1afaa-108">Retrieve a particular submission.</span></span> <span data-ttu-id="1afaa-109">Eine Übermittlung-Objekt stellt einen Schüler Arbeit für eine Zuordnung dar.</span><span class="sxs-lookup"><span data-stu-id="1afaa-109">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="1afaa-110">Ressourcen im Zusammenhang mit der Übermittlung darstellen diese arbeiten.</span><span class="sxs-lookup"><span data-stu-id="1afaa-110">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="1afaa-111">Nur der Student, die Übermittlung zugewiesen ist, kann finden Sie unter und die Übermittlung geändert werden.</span><span class="sxs-lookup"><span data-stu-id="1afaa-111">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="1afaa-112">Lehrer verfügt über Vollzugriff auf alle Übermittlungen.</span><span class="sxs-lookup"><span data-stu-id="1afaa-112">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="1afaa-113">Die Qualität und Feedback von Lehrer sind ebenfalls Teil dieses Objekt.</span><span class="sxs-lookup"><span data-stu-id="1afaa-113">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="1afaa-114">Nur Lehrer können hinzufügen oder Ändern von Kategorien und Feedback.</span><span class="sxs-lookup"><span data-stu-id="1afaa-114">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="1afaa-115">Studenten werden nicht angezeigt, der Kategorie oder Feedback, bis die Zuordnung freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="1afaa-115">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="1afaa-116">Die grundlegenden Berechtigungen Note und Feedback keinen aber alles einschließen.</span><span class="sxs-lookup"><span data-stu-id="1afaa-116">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="1afaa-117">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1afaa-117">Permissions</span></span>
<span data-ttu-id="1afaa-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1afaa-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1afaa-120">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1afaa-120">Permission type</span></span>      | <span data-ttu-id="1afaa-121">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1afaa-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1afaa-122">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1afaa-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="1afaa-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1afaa-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="1afaa-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1afaa-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1afaa-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1afaa-125">Not supported.</span></span>  |
|<span data-ttu-id="1afaa-126">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1afaa-126">Application</span></span> | <span data-ttu-id="1afaa-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1afaa-127">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1afaa-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1afaa-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1afaa-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1afaa-129">Optional query parameters</span></span>
<span data-ttu-id="1afaa-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1afaa-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1afaa-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1afaa-131">Request headers</span></span>
| <span data-ttu-id="1afaa-132">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1afaa-132">Header</span></span>       | <span data-ttu-id="1afaa-133">Wert</span><span class="sxs-lookup"><span data-stu-id="1afaa-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1afaa-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1afaa-134">Authorization</span></span>  | <span data-ttu-id="1afaa-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1afaa-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1afaa-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1afaa-137">Request body</span></span>
<span data-ttu-id="1afaa-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1afaa-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1afaa-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="1afaa-139">Response</span></span>
<span data-ttu-id="1afaa-140">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationSubmission](../resources/educationsubmission.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1afaa-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1afaa-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1afaa-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1afaa-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1afaa-142">Request</span></span>
<span data-ttu-id="1afaa-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1afaa-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="1afaa-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1afaa-144">Response</span></span>
<span data-ttu-id="1afaa-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1afaa-145">The following is an example of the response.</span></span> 

><span data-ttu-id="1afaa-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1afaa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
    "feedback": {
      text: {
        "content": "Good work!",
        "contentType": "Text"
      },
      feedbackDateTime: "2014-01-01T00:00:00Z",
      feedbackBy: {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
      },
      "@odata.type": "microsoft.graph.educationFeedback"
      },
      "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
        "gradedDateTime": "2014-01-01T00:00:00Z"
      },
      "id": "33223",
      "recipient": {
        "userId": "13015"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

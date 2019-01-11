---
title: Abrufen von educationSubmission
description: 'Abrufen einer bestimmten Übermittlung an. Eine Übermittlung-Objekt stellt einen Schüler Arbeit für eine Zuordnung dar. Ressourcen im Zusammenhang mit der Übermittlung darstellen diese arbeiten. Nur der Student, die Übermittlung zugewiesen ist, kann finden Sie unter und die Übermittlung geändert werden. Lehrer verfügt über Vollzugriff auf alle Übermittlungen. '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 4eacc6ce261566afdc6d712172d35a46f9d9e595
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813363"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="02d76-107">Abrufen von educationSubmission</span><span class="sxs-lookup"><span data-stu-id="02d76-107">Get educationSubmission</span></span>

> <span data-ttu-id="02d76-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02d76-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02d76-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d76-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02d76-110">Abrufen einer bestimmten Übermittlung an.</span><span class="sxs-lookup"><span data-stu-id="02d76-110">Retrieve a particular submission.</span></span> <span data-ttu-id="02d76-111">Eine Übermittlung-Objekt stellt einen Schüler Arbeit für eine Zuordnung dar.</span><span class="sxs-lookup"><span data-stu-id="02d76-111">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="02d76-112">Ressourcen im Zusammenhang mit der Übermittlung darstellen diese arbeiten.</span><span class="sxs-lookup"><span data-stu-id="02d76-112">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="02d76-113">Nur der Student, die Übermittlung zugewiesen ist, kann finden Sie unter und die Übermittlung geändert werden.</span><span class="sxs-lookup"><span data-stu-id="02d76-113">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="02d76-114">Lehrer verfügt über Vollzugriff auf alle Übermittlungen.</span><span class="sxs-lookup"><span data-stu-id="02d76-114">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="02d76-115">Die Qualität und Feedback von Lehrer sind ebenfalls Teil dieses Objekt.</span><span class="sxs-lookup"><span data-stu-id="02d76-115">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="02d76-116">Nur Lehrer können hinzufügen oder Ändern von Kategorien und Feedback.</span><span class="sxs-lookup"><span data-stu-id="02d76-116">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="02d76-117">Studenten werden nicht angezeigt, der Kategorie oder Feedback, bis die Zuordnung freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="02d76-117">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="02d76-118">Die grundlegenden Berechtigungen Note und Feedback keinen aber alles einschließen.</span><span class="sxs-lookup"><span data-stu-id="02d76-118">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="02d76-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="02d76-119">Permissions</span></span>
<span data-ttu-id="02d76-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02d76-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02d76-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02d76-122">Permission type</span></span>      | <span data-ttu-id="02d76-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02d76-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02d76-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02d76-124">Delegated (work or school account)</span></span> |  <span data-ttu-id="02d76-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02d76-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="02d76-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02d76-126">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="02d76-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02d76-127">Not supported.</span></span>  |
|<span data-ttu-id="02d76-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02d76-128">Application</span></span> | <span data-ttu-id="02d76-129">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02d76-129">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="02d76-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02d76-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02d76-131">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="02d76-131">Optional query parameters</span></span>
<span data-ttu-id="02d76-132">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="02d76-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02d76-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02d76-133">Request headers</span></span>
| <span data-ttu-id="02d76-134">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="02d76-134">Header</span></span>       | <span data-ttu-id="02d76-135">Wert</span><span class="sxs-lookup"><span data-stu-id="02d76-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02d76-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="02d76-136">Authorization</span></span>  | <span data-ttu-id="02d76-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02d76-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02d76-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02d76-139">Request body</span></span>
<span data-ttu-id="02d76-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="02d76-140">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="02d76-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="02d76-141">Response</span></span>
<span data-ttu-id="02d76-142">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationSubmission](../resources/educationsubmission.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="02d76-142">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02d76-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02d76-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02d76-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02d76-144">Request</span></span>
<span data-ttu-id="02d76-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02d76-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="02d76-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="02d76-146">Response</span></span>
<span data-ttu-id="02d76-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="02d76-147">The following is an example of the response.</span></span> 

><span data-ttu-id="02d76-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="02d76-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

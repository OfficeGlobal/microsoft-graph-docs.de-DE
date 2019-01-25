---
title: Liste Übermittlungen
description: Listen Sie alle Übermittlungen, die diese Zuordnung zugeordnet. Lehrer erhalten alle Übermittlungen, während nur ein Schüler Übermittlungen erhalten, denen sie zugeordnet sind.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47088cb7a4290827ce75e35d3ac705b31addefac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510638"
---
# <a name="list-submissions"></a><span data-ttu-id="55135-104">Liste Übermittlungen</span><span class="sxs-lookup"><span data-stu-id="55135-104">List submissions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55135-105">Listen Sie alle Übermittlungen, die diese Zuordnung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="55135-105">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="55135-106">Lehrer erhalten alle Übermittlungen, während nur ein Schüler Übermittlungen erhalten, denen sie zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="55135-106">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="55135-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="55135-107">Permissions</span></span>
<span data-ttu-id="55135-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55135-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55135-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="55135-110">Permission type</span></span>      | <span data-ttu-id="55135-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="55135-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55135-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="55135-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="55135-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55135-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="55135-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="55135-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="55135-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55135-115">Not supported.</span></span>  |
|<span data-ttu-id="55135-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="55135-116">Application</span></span> | <span data-ttu-id="55135-117">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55135-117">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="55135-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55135-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="55135-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="55135-119">Optional query parameters</span></span>
<span data-ttu-id="55135-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="55135-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55135-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55135-121">Request headers</span></span>
| <span data-ttu-id="55135-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="55135-122">Header</span></span>       | <span data-ttu-id="55135-123">Wert</span><span class="sxs-lookup"><span data-stu-id="55135-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55135-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="55135-124">Authorization</span></span>  | <span data-ttu-id="55135-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55135-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55135-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55135-127">Request body</span></span>
<span data-ttu-id="55135-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="55135-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="55135-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="55135-129">Response</span></span>
<span data-ttu-id="55135-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [EducationSubmission](../resources/educationsubmission.md) .</span><span class="sxs-lookup"><span data-stu-id="55135-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55135-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55135-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55135-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55135-132">Request</span></span>
<span data-ttu-id="55135-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="55135-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="55135-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="55135-134">Response</span></span>
<span data-ttu-id="55135-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="55135-135">The following is an example of the response.</span></span> 

><span data-ttu-id="55135-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="55135-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55135-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55135-137">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "feedback": {
        "text": {
          "content": "Good work!",
          "contentType": "Text"
        },
        "feedbackDateTime": "2014-01-01T00:00:00Z",
        "feedbackBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
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
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-submissions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

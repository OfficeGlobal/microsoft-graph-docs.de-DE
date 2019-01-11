---
title: Liste Übermittlungen
description: Listen Sie alle Übermittlungen, die diese Zuordnung zugeordnet. Lehrer erhalten alle Übermittlungen, während nur ein Schüler Übermittlungen erhalten, denen sie zugeordnet sind.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 0b807a1b19bdb47e3b184ffdce4a15b38740c574
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883212"
---
# <a name="list-submissions"></a><span data-ttu-id="7f133-104">Liste Übermittlungen</span><span class="sxs-lookup"><span data-stu-id="7f133-104">List submissions</span></span>

> <span data-ttu-id="7f133-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7f133-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f133-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f133-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f133-107">Listen Sie alle Übermittlungen, die diese Zuordnung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="7f133-107">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="7f133-108">Lehrer erhalten alle Übermittlungen, während nur ein Schüler Übermittlungen erhalten, denen sie zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="7f133-108">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f133-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f133-109">Permissions</span></span>
<span data-ttu-id="7f133-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f133-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f133-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f133-112">Permission type</span></span>      | <span data-ttu-id="7f133-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f133-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f133-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f133-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="7f133-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f133-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7f133-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f133-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7f133-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f133-117">Not supported.</span></span>  |
|<span data-ttu-id="7f133-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f133-118">Application</span></span> | <span data-ttu-id="7f133-119">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f133-119">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7f133-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f133-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f133-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7f133-121">Optional query parameters</span></span>
<span data-ttu-id="7f133-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7f133-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f133-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f133-123">Request headers</span></span>
| <span data-ttu-id="7f133-124">Header</span><span class="sxs-lookup"><span data-stu-id="7f133-124">Header</span></span>       | <span data-ttu-id="7f133-125">Wert</span><span class="sxs-lookup"><span data-stu-id="7f133-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f133-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f133-126">Authorization</span></span>  | <span data-ttu-id="7f133-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f133-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f133-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f133-129">Request body</span></span>
<span data-ttu-id="7f133-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7f133-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7f133-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f133-131">Response</span></span>
<span data-ttu-id="7f133-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [EducationSubmission](../resources/educationsubmission.md) .</span><span class="sxs-lookup"><span data-stu-id="7f133-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f133-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f133-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f133-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f133-134">Request</span></span>
<span data-ttu-id="7f133-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f133-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="7f133-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f133-136">Response</span></span>
<span data-ttu-id="7f133-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7f133-137">The following is an example of the response.</span></span> 

><span data-ttu-id="7f133-138">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="7f133-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7f133-139">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f133-139">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Abrufen von educationSubmittedSubmissionResource
description: Gibt eine gesendete Ressource. Dadurch wird eine Lehrer verfügbar sein, nachdem eine Student übermittelt wurde, und wird den Teilnehmern werden, nachdem der Lehrer die Übermittlung freigegeben hat.  Beachten Sie, dass Lehrer Notizen in einige Ressourcen lassen können.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bc7b6f9f0a224cf7a9c1e1c069756d8c83e08ba8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926232"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="f7652-105">Abrufen von educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="f7652-105">Get educationSubmittedSubmissionResource</span></span>

> <span data-ttu-id="f7652-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7652-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7652-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7652-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7652-108">Gibt eine gesendete Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7652-108">Returns a submitted resource.</span></span> <span data-ttu-id="f7652-109">Dadurch wird eine Lehrer verfügbar sein, nachdem eine Student übermittelt wurde, und wird den Teilnehmern werden, nachdem der Lehrer die Übermittlung freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="f7652-109">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="f7652-110">Beachten Sie, dass Lehrer Notizen in einige Ressourcen lassen können.</span><span class="sxs-lookup"><span data-stu-id="f7652-110">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7652-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7652-111">Permissions</span></span>
<span data-ttu-id="f7652-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7652-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7652-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7652-114">Permission type</span></span>      | <span data-ttu-id="f7652-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7652-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7652-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7652-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="f7652-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7652-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f7652-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7652-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f7652-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7652-119">Not supported.</span></span>  |
|<span data-ttu-id="f7652-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7652-120">Application</span></span> | <span data-ttu-id="f7652-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7652-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f7652-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7652-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7652-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f7652-123">Optional query parameters</span></span>
<span data-ttu-id="f7652-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7652-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7652-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7652-125">Request headers</span></span>
| <span data-ttu-id="f7652-126">Header</span><span class="sxs-lookup"><span data-stu-id="f7652-126">Header</span></span>       | <span data-ttu-id="f7652-127">Wert</span><span class="sxs-lookup"><span data-stu-id="f7652-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7652-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7652-128">Authorization</span></span>  | <span data-ttu-id="f7652-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f7652-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7652-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7652-131">Request body</span></span>
<span data-ttu-id="f7652-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f7652-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f7652-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7652-133">Response</span></span>
<span data-ttu-id="f7652-134">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationSubmissionResource](../resources/educationsubmissionresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f7652-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7652-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7652-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7652-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7652-136">Request</span></span>
<span data-ttu-id="f7652-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7652-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="f7652-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7652-138">Response</span></span>
<span data-ttu-id="f7652-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7652-139">The following is an example of the response.</span></span> 

><span data-ttu-id="f7652-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f7652-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
      "@odata.type": "microsoft.graph.educationResource"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmittedSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

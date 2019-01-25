---
title: Abrufen von educationSubmittedSubmissionResource
description: Gibt eine gesendete Ressource. Dadurch wird eine Lehrer verfügbar sein, nachdem eine Student übermittelt wurde, und wird den Teilnehmern werden, nachdem der Lehrer die Übermittlung freigegeben hat.  Beachten Sie, dass Lehrer Notizen in einige Ressourcen lassen können.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e529231e6503b67390b7248228af84dc59b5f633
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513277"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="7b037-105">Abrufen von educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="7b037-105">Get educationSubmittedSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b037-106">Gibt eine gesendete Ressource.</span><span class="sxs-lookup"><span data-stu-id="7b037-106">Returns a submitted resource.</span></span> <span data-ttu-id="7b037-107">Dadurch wird eine Lehrer verfügbar sein, nachdem eine Student übermittelt wurde, und wird den Teilnehmern werden, nachdem der Lehrer die Übermittlung freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="7b037-107">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="7b037-108">Beachten Sie, dass Lehrer Notizen in einige Ressourcen lassen können.</span><span class="sxs-lookup"><span data-stu-id="7b037-108">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b037-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b037-109">Permissions</span></span>
<span data-ttu-id="7b037-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b037-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b037-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b037-112">Permission type</span></span>      | <span data-ttu-id="7b037-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b037-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b037-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b037-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="7b037-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b037-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7b037-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b037-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7b037-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b037-117">Not supported.</span></span>  |
|<span data-ttu-id="7b037-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b037-118">Application</span></span> | <span data-ttu-id="7b037-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b037-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7b037-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b037-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b037-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7b037-121">Optional query parameters</span></span>
<span data-ttu-id="7b037-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b037-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b037-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b037-123">Request headers</span></span>
| <span data-ttu-id="7b037-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b037-124">Header</span></span>       | <span data-ttu-id="7b037-125">Wert</span><span class="sxs-lookup"><span data-stu-id="7b037-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7b037-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b037-126">Authorization</span></span>  | <span data-ttu-id="7b037-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b037-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b037-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b037-129">Request body</span></span>
<span data-ttu-id="7b037-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b037-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7b037-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b037-131">Response</span></span>
<span data-ttu-id="7b037-132">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationSubmissionResource](../resources/educationsubmissionresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7b037-132">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b037-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b037-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b037-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b037-134">Request</span></span>
<span data-ttu-id="7b037-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b037-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="7b037-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b037-136">Response</span></span>
<span data-ttu-id="7b037-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b037-137">The following is an example of the response.</span></span> 

><span data-ttu-id="7b037-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7b037-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmittedSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmittedsubmissionresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

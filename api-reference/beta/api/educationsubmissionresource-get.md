---
title: Abrufen von educationSubmissionResource
description: Ruft die Eigenschaften einer bestimmten Ressource der Übermittlung zugeordnet. Diese Ressource ist in der Liste 'Arbeit' Ressource und sollte in Bearbeitung durch einen Schüler berücksichtigt werden. Diese Ressource mit einem möglichen Zeiger an die Zuordnung Ressource umbrochen werden, wenn es die Zuordnung kopiert wurde.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b76d697afa842fe5315792d803e9b704a628a0b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518366"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="31bd1-105">Abrufen von educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="31bd1-105">Get educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31bd1-106">Ruft die Eigenschaften einer bestimmten Ressource der Übermittlung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="31bd1-106">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="31bd1-107">Diese Ressource ist in der Liste "Working" Ressource und sollte in Bearbeitung durch einen Schüler berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="31bd1-107">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="31bd1-108">Diese Ressource mit einem möglichen Zeiger an die Zuordnung Ressource umbrochen werden, wenn es die Zuordnung kopiert wurde.</span><span class="sxs-lookup"><span data-stu-id="31bd1-108">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="31bd1-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="31bd1-109">Permissions</span></span>
<span data-ttu-id="31bd1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31bd1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31bd1-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31bd1-112">Permission type</span></span>      | <span data-ttu-id="31bd1-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31bd1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31bd1-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31bd1-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="31bd1-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31bd1-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="31bd1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31bd1-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="31bd1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31bd1-117">Not supported.</span></span>  |
|<span data-ttu-id="31bd1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31bd1-118">Application</span></span> | <span data-ttu-id="31bd1-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31bd1-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="31bd1-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31bd1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="31bd1-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="31bd1-121">Optional query parameters</span></span>
<span data-ttu-id="31bd1-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="31bd1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31bd1-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31bd1-123">Request headers</span></span>
| <span data-ttu-id="31bd1-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="31bd1-124">Header</span></span>       | <span data-ttu-id="31bd1-125">Wert</span><span class="sxs-lookup"><span data-stu-id="31bd1-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31bd1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="31bd1-126">Authorization</span></span>  | <span data-ttu-id="31bd1-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="31bd1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31bd1-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31bd1-129">Request body</span></span>
<span data-ttu-id="31bd1-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="31bd1-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="31bd1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="31bd1-131">Response</span></span>
<span data-ttu-id="31bd1-132">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [EducationSubmissionResource](../resources/educationsubmissionresource.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="31bd1-132">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31bd1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31bd1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31bd1-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31bd1-134">Request</span></span>
<span data-ttu-id="31bd1-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31bd1-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="31bd1-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="31bd1-136">Response</span></span>
<span data-ttu-id="31bd1-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="31bd1-137">The following is an example of the response.</span></span> 

><span data-ttu-id="31bd1-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="31bd1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

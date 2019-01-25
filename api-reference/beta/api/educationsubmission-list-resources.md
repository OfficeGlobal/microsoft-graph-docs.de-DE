---
title: List-Ressourcen
description: Listen Sie die Ressourcen dieses Übermittlung zugeordnet. Das **SubmissionResource** -Objekt ist ein Wrapper für die tatsächliche Resource-Objekt der Student gearbeitet wird. Der Wrapper enthält auch einen Zeiger auf die Ressourcen für die Zuordnung, wenn dies in der Zuweisung während des Aktivierungsvorgangs zuweisen kopiert wurde. Diese Ressourcen sind die Arbeitskopie der Zuordnung. Die **SubmittedResources** sind die Ressourcen, die offiziell gesendet wurden, sortiert werden.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b9069cb6ec20f65b82cacca8f862a05ff0af7b5d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526186"
---
# <a name="list-resources"></a><span data-ttu-id="29cad-107">List-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="29cad-107">List resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29cad-108">Listen Sie die Ressourcen dieses Übermittlung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="29cad-108">List the resources associated with this submission.</span></span> <span data-ttu-id="29cad-109">Das **SubmissionResource** -Objekt ist ein Wrapper für die tatsächliche Resource-Objekt der Student gearbeitet wird.</span><span class="sxs-lookup"><span data-stu-id="29cad-109">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="29cad-110">Der Wrapper enthält auch einen Zeiger auf die Ressourcen für die Zuordnung, wenn dies in der Zuweisung während des Aktivierungsvorgangs zuweisen kopiert wurde.</span><span class="sxs-lookup"><span data-stu-id="29cad-110">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="29cad-111">Diese Ressourcen sind die Arbeitskopie der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="29cad-111">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="29cad-112">Die **SubmittedResources** sind die Ressourcen, die offiziell gesendet wurden, sortiert werden.</span><span class="sxs-lookup"><span data-stu-id="29cad-112">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="29cad-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29cad-113">Permissions</span></span>
<span data-ttu-id="29cad-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29cad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29cad-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29cad-116">Permission type</span></span>      | <span data-ttu-id="29cad-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29cad-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29cad-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29cad-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="29cad-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29cad-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="29cad-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29cad-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29cad-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29cad-121">Not supported.</span></span>   |
|<span data-ttu-id="29cad-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29cad-122">Application</span></span> | <span data-ttu-id="29cad-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29cad-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="29cad-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29cad-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29cad-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="29cad-125">Optional query parameters</span></span>
<span data-ttu-id="29cad-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29cad-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29cad-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29cad-127">Request headers</span></span>
| <span data-ttu-id="29cad-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="29cad-128">Header</span></span>       | <span data-ttu-id="29cad-129">Wert</span><span class="sxs-lookup"><span data-stu-id="29cad-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29cad-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="29cad-130">Authorization</span></span>  | <span data-ttu-id="29cad-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29cad-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29cad-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29cad-133">Request body</span></span>
<span data-ttu-id="29cad-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="29cad-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="29cad-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="29cad-135">Response</span></span>
<span data-ttu-id="29cad-136">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationSubmissionResource](../resources/educationsubmissionresource.md) .</span><span class="sxs-lookup"><span data-stu-id="29cad-136">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29cad-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29cad-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29cad-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29cad-138">Request</span></span>
<span data-ttu-id="29cad-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29cad-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="29cad-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="29cad-140">Response</span></span>
<span data-ttu-id="29cad-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29cad-141">The following is an example of the response.</span></span> 

><span data-ttu-id="29cad-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="29cad-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-list-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

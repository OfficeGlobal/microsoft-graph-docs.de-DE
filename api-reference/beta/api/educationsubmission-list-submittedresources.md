---
title: Liste submittedResources
description: Listen Sie die Ressourcen, die zum Sortieren der offiziell gesendet wurden. Der Besitzer die Übermittlung Student kann nicht die übermittelte Liste ändern, ohne die erneute Übermittlung der Zuordnung. Dies ist ein Wrapper für die Ressource real und kann einen Zeiger an die aktuelle Zuordnung Ressource enthalten, wenn diese Ressource aus die Zuordnung kopiert wurde.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a798ea45ca88520954bbde20a264fff9455f3102
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934989"
---
# <a name="list-submittedresources"></a><span data-ttu-id="12734-105">Liste submittedResources</span><span class="sxs-lookup"><span data-stu-id="12734-105">List submittedResources</span></span>

> <span data-ttu-id="12734-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12734-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12734-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12734-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12734-108">Listen Sie die Ressourcen, die zum Sortieren der offiziell gesendet wurden.</span><span class="sxs-lookup"><span data-stu-id="12734-108">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="12734-109">Der Besitzer die Übermittlung Student kann nicht die übermittelte Liste ändern, ohne die erneute Übermittlung der Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="12734-109">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="12734-110">Dies ist ein Wrapper für die Ressource real und kann einen Zeiger an die aktuelle Zuordnung Ressource enthalten, wenn diese Ressource aus die Zuordnung kopiert wurde.</span><span class="sxs-lookup"><span data-stu-id="12734-110">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="12734-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12734-111">Permissions</span></span>
<span data-ttu-id="12734-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12734-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12734-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12734-114">Permission type</span></span>      | <span data-ttu-id="12734-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12734-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12734-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12734-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="12734-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12734-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="12734-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12734-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="12734-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12734-119">Not supported.</span></span>  |
|<span data-ttu-id="12734-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12734-120">Application</span></span> | <span data-ttu-id="12734-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12734-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="12734-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12734-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12734-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="12734-123">Optional query parameters</span></span>
<span data-ttu-id="12734-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="12734-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12734-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12734-125">Request headers</span></span>
| <span data-ttu-id="12734-126">Header</span><span class="sxs-lookup"><span data-stu-id="12734-126">Header</span></span>       | <span data-ttu-id="12734-127">Wert</span><span class="sxs-lookup"><span data-stu-id="12734-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12734-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="12734-128">Authorization</span></span>  | <span data-ttu-id="12734-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12734-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12734-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12734-131">Request body</span></span>
<span data-ttu-id="12734-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="12734-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="12734-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="12734-133">Response</span></span>
<span data-ttu-id="12734-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationSubmissionResource](../resources/educationsubmissionresource.md) .</span><span class="sxs-lookup"><span data-stu-id="12734-134">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12734-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12734-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12734-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12734-136">Request</span></span>
<span data-ttu-id="12734-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="12734-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="12734-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="12734-138">Response</span></span>
<span data-ttu-id="12734-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="12734-139">The following is an example of the response.</span></span> 

><span data-ttu-id="12734-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="12734-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource",
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
        "link": "https://www.microsoft.com
        },
        "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource" 
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

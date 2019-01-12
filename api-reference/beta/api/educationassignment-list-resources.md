---
title: Liste educationAssignmentResources
description: Rufen Sie alle Ressourcen, die diese Zuordnung zugeordnet.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0fa0a5b46d7f40b1d1e8b6d265b12f84384e2c50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936200"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="cc9c9-103">Liste educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="cc9c9-103">List educationAssignmentResources</span></span>

> <span data-ttu-id="cc9c9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc9c9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc9c9-106">Rufen Sie alle Ressourcen, die diese Zuordnung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-106">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc9c9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cc9c9-107">Permissions</span></span>
<span data-ttu-id="cc9c9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc9c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc9c9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cc9c9-110">Permission type</span></span>      | <span data-ttu-id="cc9c9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cc9c9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc9c9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cc9c9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="cc9c9-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc9c9-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="cc9c9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cc9c9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cc9c9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cc9c9-115">Not supported.</span></span>  |
|<span data-ttu-id="cc9c9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cc9c9-116">Application</span></span> | <span data-ttu-id="cc9c9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cc9c9-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cc9c9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc9c9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc9c9-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cc9c9-119">Optional query parameters</span></span>
<span data-ttu-id="cc9c9-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc9c9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cc9c9-121">Request headers</span></span>
| <span data-ttu-id="cc9c9-122">Header</span><span class="sxs-lookup"><span data-stu-id="cc9c9-122">Header</span></span>       | <span data-ttu-id="cc9c9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="cc9c9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc9c9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc9c9-124">Authorization</span></span>  | <span data-ttu-id="cc9c9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc9c9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cc9c9-127">Request body</span></span>
<span data-ttu-id="cc9c9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cc9c9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc9c9-129">Response</span></span>
<span data-ttu-id="cc9c9-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationAssignmentResource](../resources/educationassignmentresource.md) .</span><span class="sxs-lookup"><span data-stu-id="cc9c9-130">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc9c9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cc9c9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc9c9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc9c9-132">Request</span></span>
<span data-ttu-id="cc9c9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="cc9c9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc9c9-134">Response</span></span>
<span data-ttu-id="cc9c9-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-135">The following is an example of the response.</span></span> 

><span data-ttu-id="cc9c9-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cc9c9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
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
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
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
      },
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

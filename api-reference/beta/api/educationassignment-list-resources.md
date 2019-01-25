---
title: Liste educationAssignmentResources
description: Rufen Sie alle Ressourcen, die diese Zuordnung zugeordnet.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5556210604ce6b0c273a0e4d89e1a792d2639b12
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518569"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="b215a-103">Liste educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="b215a-103">List educationAssignmentResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b215a-104">Rufen Sie alle Ressourcen, die diese Zuordnung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="b215a-104">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="b215a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b215a-105">Permissions</span></span>
<span data-ttu-id="b215a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b215a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b215a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b215a-108">Permission type</span></span>      | <span data-ttu-id="b215a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b215a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b215a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b215a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b215a-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b215a-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b215a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b215a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b215a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b215a-113">Not supported.</span></span>  |
|<span data-ttu-id="b215a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b215a-114">Application</span></span> | <span data-ttu-id="b215a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b215a-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b215a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b215a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b215a-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b215a-117">Optional query parameters</span></span>
<span data-ttu-id="b215a-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b215a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b215a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b215a-119">Request headers</span></span>
| <span data-ttu-id="b215a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b215a-120">Header</span></span>       | <span data-ttu-id="b215a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b215a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b215a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b215a-122">Authorization</span></span>  | <span data-ttu-id="b215a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b215a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b215a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b215a-125">Request body</span></span>
<span data-ttu-id="b215a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b215a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b215a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b215a-127">Response</span></span>
<span data-ttu-id="b215a-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EducationAssignmentResource](../resources/educationassignmentresource.md) .</span><span class="sxs-lookup"><span data-stu-id="b215a-128">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b215a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b215a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b215a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b215a-130">Request</span></span>
<span data-ttu-id="b215a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b215a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="b215a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b215a-132">Response</span></span>
<span data-ttu-id="b215a-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b215a-133">The following is an example of the response.</span></span> 

><span data-ttu-id="b215a-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b215a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

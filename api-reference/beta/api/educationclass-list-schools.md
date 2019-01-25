---
title: Schulen auflisten
description: Abrufen einer Liste von Schulen, in denen der Kurs unterrichtet wird.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8e79825a4c31ef6c6d4910dd3826d24176d17c71
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509882"
---
# <a name="list-schools"></a><span data-ttu-id="3d029-103">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="3d029-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d029-104">Abrufen einer Liste von Schulen, in denen der Kurs unterrichtet wird.</span><span class="sxs-lookup"><span data-stu-id="3d029-104">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d029-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3d029-105">Permissions</span></span>
<span data-ttu-id="3d029-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d029-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d029-108">Permission type</span></span>      | <span data-ttu-id="3d029-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d029-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d029-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d029-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3d029-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="3d029-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="3d029-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d029-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3d029-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d029-113">Not supported</span></span>  |
|<span data-ttu-id="3d029-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d029-114">Application</span></span> | <span data-ttu-id="3d029-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d029-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3d029-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d029-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d029-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3d029-117">Optional query parameters</span></span>
<span data-ttu-id="3d029-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3d029-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d029-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d029-119">Request headers</span></span>
| <span data-ttu-id="3d029-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3d029-120">Header</span></span>       | <span data-ttu-id="3d029-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3d029-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3d029-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d029-122">Authorization</span></span>  | <span data-ttu-id="3d029-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3d029-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="3d029-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d029-125">Request body</span></span>
<span data-ttu-id="3d029-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3d029-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3d029-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d029-127">Response</span></span>
<span data-ttu-id="3d029-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationSchool](../resources/educationschool.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d029-128">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d029-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d029-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d029-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d029-130">Request</span></span>
<span data-ttu-id="3d029-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d029-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/schools
```
##### <a name="response"></a><span data-ttu-id="3d029-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d029-132">Response</span></span>
<span data-ttu-id="3d029-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3d029-133">The following is an example of the response.</span></span> 

><span data-ttu-id="3d029-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3d029-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10002",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-list-schools.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

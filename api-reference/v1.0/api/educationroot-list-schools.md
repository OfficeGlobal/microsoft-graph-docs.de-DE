---
title: EducationSchools auflisten
description: Abrufen einer Liste aller school-Objekte.
ms.openlocfilehash: 5b2108d1c6f42f1d8967abcdd95941321da33dca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017282"
---
# <a name="list-educationschools"></a><span data-ttu-id="d1b72-103">EducationSchools auflisten</span><span class="sxs-lookup"><span data-stu-id="d1b72-103">List educationSchools</span></span>

<span data-ttu-id="d1b72-104">Abrufen einer Liste aller school-Objekte.</span><span class="sxs-lookup"><span data-stu-id="d1b72-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1b72-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d1b72-105">Permissions</span></span>
<span data-ttu-id="d1b72-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1b72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1b72-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d1b72-108">Permission type</span></span>      | <span data-ttu-id="d1b72-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d1b72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1b72-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d1b72-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d1b72-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d1b72-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="d1b72-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d1b72-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d1b72-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d1b72-113">Not supported.</span></span>  |
|<span data-ttu-id="d1b72-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d1b72-114">Application</span></span> | <span data-ttu-id="d1b72-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1b72-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d1b72-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1b72-116">HTTP request</span></span>
<span data-ttu-id="d1b72-117"><!-- { "blockType": "ignored" } -->'''http GET/Education/Schulen</span><span class="sxs-lookup"><span data-stu-id="d1b72-117"><!-- { "blockType": "ignored" } --> \`\`\`http GET /education/schools</span></span>
```
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.

## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |

## Request body
Do not supply a request body for this method.
## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.
## Example
##### Request
The following is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools
```
##### <a name="response"></a><span data-ttu-id="d1b72-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1b72-118">Response</span></span>
<span data-ttu-id="d1b72-119">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d1b72-119">The following is an example of the response.</span></span> 

><span data-ttu-id="d1b72-p102">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d1b72-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
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
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
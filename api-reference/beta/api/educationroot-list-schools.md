---
title: EducationSchools auflisten
description: Abrufen einer Liste aller school-Objekte.
ms.openlocfilehash: 88ba9591b305c62ce40e059f422cc674f445500d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058350"
---
# <a name="list-educationschools"></a><span data-ttu-id="34b64-103">EducationSchools auflisten</span><span class="sxs-lookup"><span data-stu-id="34b64-103">List educationSchools</span></span>

> <span data-ttu-id="34b64-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34b64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34b64-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34b64-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34b64-106">Abrufen einer Liste aller school-Objekte.</span><span class="sxs-lookup"><span data-stu-id="34b64-106">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="34b64-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="34b64-107">Permissions</span></span>
<span data-ttu-id="34b64-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34b64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34b64-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34b64-110">Permission type</span></span>      | <span data-ttu-id="34b64-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34b64-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34b64-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34b64-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="34b64-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="34b64-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="34b64-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34b64-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="34b64-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34b64-115">Not supported.</span></span>  |
|<span data-ttu-id="34b64-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34b64-116">Application</span></span> | <span data-ttu-id="34b64-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34b64-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="34b64-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34b64-118">HTTP request</span></span>
<span data-ttu-id="34b64-119"><!-- { "blockType": "ignored" } -->'''http GET/Education/Schulen</span><span class="sxs-lookup"><span data-stu-id="34b64-119"><!-- { "blockType": "ignored" } --> \`\`\`http GET /education/schools</span></span>
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
GET https://graph.microsoft.com/beta/education/schools
```
##### <a name="response"></a><span data-ttu-id="34b64-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="34b64-120">Response</span></span>
<span data-ttu-id="34b64-121">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34b64-121">The following is an example of the response.</span></span> 

><span data-ttu-id="34b64-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="34b64-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

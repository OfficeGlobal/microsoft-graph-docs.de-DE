# <a name="list-educationschools"></a><span data-ttu-id="294c4-101">EducationSchools auflisten</span><span class="sxs-lookup"><span data-stu-id="294c4-101">List educationSchools</span></span>

<span data-ttu-id="294c4-102">Abrufen einer Liste aller school-Objekte.</span><span class="sxs-lookup"><span data-stu-id="294c4-102">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="294c4-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="294c4-103">Permissions</span></span>
<span data-ttu-id="294c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="294c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="294c4-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="294c4-106">Permission type</span></span>      | <span data-ttu-id="294c4-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="294c4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="294c4-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="294c4-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="294c4-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="294c4-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="294c4-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="294c4-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="294c4-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="294c4-111">Not supported.</span></span>  |
|<span data-ttu-id="294c4-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="294c4-112">Application</span></span> | <span data-ttu-id="294c4-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294c4-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="294c4-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="294c4-114">HTTP request</span></span>
<span data-ttu-id="294c4-115"><!-- { "blockType": "ignored" } -->'''http GET/Education/Schulen</span><span class="sxs-lookup"><span data-stu-id="294c4-115"><!-- { "blockType": "ignored" } --> \`\`\`http GET /education/schools</span></span>
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
##### <a name="response"></a><span data-ttu-id="294c4-116">Antwort</span><span class="sxs-lookup"><span data-stu-id="294c4-116">Response</span></span>
<span data-ttu-id="294c4-117">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="294c4-117">The following is an example of the response.</span></span> 

><span data-ttu-id="294c4-p102">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="294c4-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

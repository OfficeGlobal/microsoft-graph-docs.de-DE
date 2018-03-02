# <a name="list-schools"></a><span data-ttu-id="09ad7-101">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="09ad7-101">List schools</span></span>

<span data-ttu-id="09ad7-102">Dient zum Abrufen einer Liste von Schulen für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="09ad7-102">Retrieve a list of licenseDetails objects for a user.</span></span>

><span data-ttu-id="09ad7-103">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="09ad7-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="09ad7-104">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="09ad7-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="09ad7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="09ad7-105">Permissions</span></span>
<span data-ttu-id="09ad7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="09ad7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="09ad7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09ad7-108">Permission type</span></span>      | <span data-ttu-id="09ad7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09ad7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09ad7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09ad7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="09ad7-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="09ad7-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="09ad7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09ad7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="09ad7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09ad7-113">Not supported.</span></span>  |
|<span data-ttu-id="09ad7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09ad7-114">Application</span></span> | <span data-ttu-id="09ad7-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09ad7-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="09ad7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09ad7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09ad7-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="09ad7-117">Optional query parameters</span></span>
<span data-ttu-id="09ad7-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09ad7-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09ad7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09ad7-119">Request headers</span></span>
| <span data-ttu-id="09ad7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="09ad7-120">Header</span></span>       | <span data-ttu-id="09ad7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="09ad7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09ad7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09ad7-122">Authorization</span></span>  | <span data-ttu-id="09ad7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="09ad7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09ad7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09ad7-125">Request body</span></span>
<span data-ttu-id="09ad7-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="09ad7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="09ad7-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="09ad7-127">Response</span></span>
<span data-ttu-id="09ad7-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationSchool](../resources/educationschool.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09ad7-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09ad7-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09ad7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09ad7-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09ad7-130">Request</span></span>
<span data-ttu-id="09ad7-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09ad7-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="09ad7-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="09ad7-132">Response</span></span>
<span data-ttu-id="09ad7-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09ad7-133">The following is an example of the response.</span></span> 

><span data-ttu-id="09ad7-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="09ad7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
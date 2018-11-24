# <a name="list-users"></a><span data-ttu-id="87c94-101">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="87c94-101">List users</span></span>

<span data-ttu-id="87c94-102">Dient zum Abrufen einer Liste von Benutzerobjekten.</span><span class="sxs-lookup"><span data-stu-id="87c94-102">Retrieve a list of user objects.</span></span> <span data-ttu-id="87c94-103">Diese Benutzerobjekte enthalten schulungsspezifische Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="87c94-103">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="87c94-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87c94-104">Permissions</span></span>
<span data-ttu-id="87c94-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87c94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87c94-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87c94-107">Permission type</span></span>      | <span data-ttu-id="87c94-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87c94-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c94-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87c94-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="87c94-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87c94-110">Not supported.</span></span>  |
|<span data-ttu-id="87c94-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87c94-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="87c94-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87c94-112">Not supported.</span></span>  |
|<span data-ttu-id="87c94-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87c94-113">Application</span></span> | <span data-ttu-id="87c94-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87c94-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="87c94-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c94-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87c94-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="87c94-116">Optional query parameters</span></span>
<span data-ttu-id="87c94-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87c94-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87c94-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87c94-118">Request headers</span></span>
| <span data-ttu-id="87c94-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87c94-119">Header</span></span>       | <span data-ttu-id="87c94-120">Wert</span><span class="sxs-lookup"><span data-stu-id="87c94-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87c94-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87c94-121">Authorization</span></span>  | <span data-ttu-id="87c94-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87c94-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87c94-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87c94-124">Request body</span></span>
<span data-ttu-id="87c94-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87c94-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="87c94-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c94-126">Response</span></span>
<span data-ttu-id="87c94-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationUser](../resources/educationuser.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87c94-127">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87c94-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87c94-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87c94-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c94-129">Request</span></span>
<span data-ttu-id="87c94-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87c94-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users
```
##### <a name="response"></a><span data-ttu-id="87c94-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c94-131">Response</span></span>
<span data-ttu-id="87c94-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87c94-132">The following is an example of the response.</span></span> 

><span data-ttu-id="87c94-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="87c94-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": null,
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

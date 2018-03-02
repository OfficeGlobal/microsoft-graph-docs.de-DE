# <a name="list-teachers"></a><span data-ttu-id="aa34a-101">Lehrer auflisten</span><span class="sxs-lookup"><span data-stu-id="aa34a-101">List teachers</span></span>

<span data-ttu-id="aa34a-102">Abrufen einer Liste der Lehrer für eine Klasse.</span><span class="sxs-lookup"><span data-stu-id="aa34a-102">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="aa34a-103">Delegierte Token müssen zum Abrufen der Liste der Lehrer Mitglieder der Klasse sein.</span><span class="sxs-lookup"><span data-stu-id="aa34a-103">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa34a-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa34a-104">Permissions</span></span>
<span data-ttu-id="aa34a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa34a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa34a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa34a-107">Permission type</span></span>      | <span data-ttu-id="aa34a-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa34a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa34a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa34a-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="aa34a-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="aa34a-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="aa34a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa34a-111">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="aa34a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa34a-112">Not supported.</span></span>  |
|<span data-ttu-id="aa34a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa34a-113">Application</span></span> | <span data-ttu-id="aa34a-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa34a-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aa34a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa34a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa34a-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="aa34a-116">Optional query parameters</span></span>
<span data-ttu-id="aa34a-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa34a-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa34a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa34a-118">Request headers</span></span>
| <span data-ttu-id="aa34a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="aa34a-119">Header</span></span>       | <span data-ttu-id="aa34a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="aa34a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa34a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa34a-121">Authorization</span></span>  | <span data-ttu-id="aa34a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa34a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa34a-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa34a-124">Request body</span></span>
<span data-ttu-id="aa34a-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aa34a-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="aa34a-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa34a-126">Response</span></span>
<span data-ttu-id="aa34a-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationUser](../resources/educationuser.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa34a-127">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa34a-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa34a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa34a-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa34a-129">Request</span></span>
<span data-ttu-id="aa34a-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa34a-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/11023/teachers
```
##### <a name="response"></a><span data-ttu-id="aa34a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa34a-131">Response</span></span>
<span data-ttu-id="aa34a-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa34a-132">The following is an example of the response.</span></span> 

><span data-ttu-id="aa34a-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="aa34a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
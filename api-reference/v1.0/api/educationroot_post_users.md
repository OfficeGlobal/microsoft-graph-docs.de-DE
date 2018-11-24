# <a name="create-educationuser"></a><span data-ttu-id="afef7-101">EducationUser erstellen</span><span class="sxs-lookup"><span data-stu-id="afef7-101">Create educationUser</span></span>

<span data-ttu-id="afef7-102">Erstellen eines neuen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="afef7-102">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="afef7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="afef7-103">Permissions</span></span>
<span data-ttu-id="afef7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="afef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="afef7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="afef7-106">Permission type</span></span>      | <span data-ttu-id="afef7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="afef7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afef7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="afef7-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="afef7-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afef7-109">Not supported.</span></span>  |
|<span data-ttu-id="afef7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="afef7-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="afef7-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afef7-111">Not supported.</span></span>  |
|<span data-ttu-id="afef7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="afef7-112">Application</span></span> | <span data-ttu-id="afef7-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afef7-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="afef7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afef7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="afef7-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afef7-115">Request headers</span></span>
| <span data-ttu-id="afef7-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="afef7-116">Header</span></span>       | <span data-ttu-id="afef7-117">Wert</span><span class="sxs-lookup"><span data-stu-id="afef7-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="afef7-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="afef7-118">Authorization</span></span>  | <span data-ttu-id="afef7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="afef7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="afef7-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afef7-121">Content-Type</span></span>  | <span data-ttu-id="afef7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="afef7-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="afef7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="afef7-123">Request body</span></span>
<span data-ttu-id="afef7-124">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationUser](../resources/educationuser.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="afef7-124">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="afef7-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="afef7-125">Response</span></span>
<span data-ttu-id="afef7-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afef7-126">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afef7-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afef7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afef7-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afef7-128">Request</span></span>
<span data-ttu-id="afef7-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="afef7-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/users
Content-type: application/json
Content-length: 508

{
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
```

##### <a name="response"></a><span data-ttu-id="afef7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="afef7-130">Response</span></span>
<span data-ttu-id="afef7-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="afef7-131">The following is an example of the response.</span></span> 

><span data-ttu-id="afef7-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="afef7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
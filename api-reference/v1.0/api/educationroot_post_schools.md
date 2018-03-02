# <a name="create-educationschool"></a><span data-ttu-id="d2b91-101">EducationSchool erstellen</span><span class="sxs-lookup"><span data-stu-id="d2b91-101">Create educationSchool</span></span>

<span data-ttu-id="d2b91-102">Erstellt eine Bildungseinrichtung.</span><span class="sxs-lookup"><span data-stu-id="d2b91-102">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2b91-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d2b91-103">Permissions</span></span>
<span data-ttu-id="d2b91-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d2b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2b91-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2b91-106">Permission type</span></span>      | <span data-ttu-id="d2b91-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2b91-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2b91-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2b91-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="d2b91-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2b91-109">Not supported.</span></span>  |
|<span data-ttu-id="d2b91-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2b91-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d2b91-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2b91-111">Not supported.</span></span>  |
|<span data-ttu-id="d2b91-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2b91-112">Application</span></span> | <span data-ttu-id="d2b91-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2b91-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d2b91-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2b91-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="d2b91-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2b91-115">Request headers</span></span>
| <span data-ttu-id="d2b91-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d2b91-116">Header</span></span>       | <span data-ttu-id="d2b91-117">Wert</span><span class="sxs-lookup"><span data-stu-id="d2b91-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2b91-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2b91-118">Authorization</span></span>  | <span data-ttu-id="d2b91-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d2b91-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2b91-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2b91-121">Content-Type</span></span>  | <span data-ttu-id="d2b91-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d2b91-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2b91-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2b91-123">Request body</span></span>
<span data-ttu-id="d2b91-124">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationSchool](../resources/educationschool.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d2b91-124">In the request body, supply a JSON representation of an [invitation](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d2b91-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2b91-125">Response</span></span>
<span data-ttu-id="d2b91-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2b91-126">If successful, this method returns a `201 Created` response code and an [event](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2b91-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2b91-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2b91-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2b91-128">Request</span></span>
<span data-ttu-id="d2b91-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d2b91-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-type: application/json
Content-length: 292

{
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
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

##### <a name="response"></a><span data-ttu-id="d2b91-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2b91-130">Response</span></span>
<span data-ttu-id="d2b91-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d2b91-131">The following is an example of the response.</span></span> 

><span data-ttu-id="d2b91-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d2b91-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 292

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
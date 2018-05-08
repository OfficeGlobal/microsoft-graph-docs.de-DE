# <a name="get-organization"></a><span data-ttu-id="fccac-101">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="fccac-101">Get organization</span></span>

<span data-ttu-id="fccac-102">Mit dieser API können Sie die Eigenschaften und Beziehungen der jeweils aktuell authentifizierten Organisation abrufen.</span><span class="sxs-lookup"><span data-stu-id="fccac-102">Retrieve the properties and relationships of currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="fccac-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fccac-103">Permissions</span></span>
<span data-ttu-id="fccac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fccac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fccac-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fccac-106">Permission type</span></span>      | <span data-ttu-id="fccac-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fccac-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fccac-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fccac-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fccac-109">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fccac-109">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="fccac-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fccac-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fccac-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fccac-111">Not supported.</span></span>    |
|<span data-ttu-id="fccac-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fccac-112">Application</span></span> | <span data-ttu-id="fccac-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fccac-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="fccac-114">Hinweis: Anwendungen, denen die User.Read-Berechtigung gewährt wurde, können nur die *id*-, *displayName*- und *verifiedDomains*-Eigenschaften der Organisation lesen.</span><span class="sxs-lookup"><span data-stu-id="fccac-114">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="fccac-115">Alle anderen Eigenschaften geben `null`-Werte zurück.</span><span class="sxs-lookup"><span data-stu-id="fccac-115">All other properties will return with `null` values.</span></span> <span data-ttu-id="fccac-116">Verwenden Sie zum Lesen aller Eigenschaften Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="fccac-116">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="fccac-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fccac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization

```
## <a name="optional-query-parameters"></a><span data-ttu-id="fccac-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fccac-118">Optional query parameters</span></span>
<span data-ttu-id="fccac-119">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fccac-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fccac-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fccac-120">Request headers</span></span>
| <span data-ttu-id="fccac-121">Name</span><span class="sxs-lookup"><span data-stu-id="fccac-121">Name</span></span>       | <span data-ttu-id="fccac-122">Typ</span><span class="sxs-lookup"><span data-stu-id="fccac-122">Type</span></span> | <span data-ttu-id="fccac-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fccac-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fccac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fccac-124">Authorization</span></span>  | <span data-ttu-id="fccac-125">string</span><span class="sxs-lookup"><span data-stu-id="fccac-125">string</span></span>  | <span data-ttu-id="fccac-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fccac-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fccac-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fccac-128">Request body</span></span>
<span data-ttu-id="fccac-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fccac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fccac-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="fccac-130">Response</span></span>

<span data-ttu-id="fccac-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [organization](../resources/organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fccac-131">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fccac-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fccac-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fccac-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fccac-133">Request</span></span>
<span data-ttu-id="fccac-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fccac-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/v1.0/organization
```
##### <a name="response"></a><span data-ttu-id="fccac-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="fccac-135">Response</span></span>
<span data-ttu-id="fccac-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fccac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
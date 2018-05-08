# <a name="list-organization"></a><span data-ttu-id="7c6be-101">Organisation auflisten</span><span class="sxs-lookup"><span data-stu-id="7c6be-101">List organization</span></span>

> <span data-ttu-id="7c6be-102">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7c6be-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c6be-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c6be-103">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c6be-104">Mit dieser API können Sie eine Liste von Organisationsobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="7c6be-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c6be-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c6be-105">Permissions</span></span>
<span data-ttu-id="7c6be-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c6be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c6be-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c6be-108">Permission type</span></span>      | <span data-ttu-id="7c6be-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c6be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c6be-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c6be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c6be-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c6be-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="7c6be-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c6be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c6be-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c6be-113">Not supported.</span></span>    |
|<span data-ttu-id="7c6be-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c6be-114">Application</span></span> | <span data-ttu-id="7c6be-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c6be-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="7c6be-116">Hinweis: Anwendungen, denen die User.Read-Berechtigung gewährt wurde, können nur die *id*-, *displayName*- und *verifiedDomains*-Eigenschaften der Organisation lesen.</span><span class="sxs-lookup"><span data-stu-id="7c6be-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="7c6be-117">Alle anderen Eigenschaften geben `null`-Werte zurück.</span><span class="sxs-lookup"><span data-stu-id="7c6be-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="7c6be-118">Verwenden Sie zum Lesen aller Eigenschaften Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="7c6be-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="7c6be-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c6be-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7c6be-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7c6be-120">Optional query parameters</span></span>
<span data-ttu-id="7c6be-121">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c6be-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7c6be-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c6be-122">Request headers</span></span>
| <span data-ttu-id="7c6be-123">Name</span><span class="sxs-lookup"><span data-stu-id="7c6be-123">Name</span></span>       | <span data-ttu-id="7c6be-124">Typ</span><span class="sxs-lookup"><span data-stu-id="7c6be-124">Type</span></span> | <span data-ttu-id="7c6be-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c6be-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7c6be-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c6be-126">Authorization</span></span>  | <span data-ttu-id="7c6be-127">string</span><span class="sxs-lookup"><span data-stu-id="7c6be-127">string</span></span>  | <span data-ttu-id="7c6be-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c6be-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c6be-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c6be-130">Request body</span></span>
<span data-ttu-id="7c6be-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7c6be-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c6be-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c6be-132">Response</span></span>

<span data-ttu-id="7c6be-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [organization](../resources/organization.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c6be-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7c6be-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c6be-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c6be-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c6be-135">Request</span></span>
<span data-ttu-id="7c6be-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c6be-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="7c6be-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c6be-137">Response</span></span>
<span data-ttu-id="7c6be-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c6be-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
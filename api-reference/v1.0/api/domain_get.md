# <a name="get-domain"></a><span data-ttu-id="5d5f0-101">Domäne abrufen</span><span class="sxs-lookup"><span data-stu-id="5d5f0-101">Get domain</span></span>

<span data-ttu-id="5d5f0-102">Mit dieser API können Sie die Eigenschaften und Beziehungen von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="5d5f0-102">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d5f0-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d5f0-103">Permissions</span></span>

<span data-ttu-id="5d5f0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d5f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5d5f0-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d5f0-106">Permission type</span></span>      | <span data-ttu-id="5d5f0-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d5f0-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="5d5f0-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d5f0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5d5f0-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d5f0-109">Directory.Read.All</span></span>    | 
|<span data-ttu-id="5d5f0-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d5f0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d5f0-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d5f0-111">Not supported.</span></span>    | 
|<span data-ttu-id="5d5f0-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d5f0-112">Application</span></span> | <span data-ttu-id="5d5f0-113">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d5f0-113">Directory.Read.All, Domain.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5d5f0-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d5f0-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="5d5f0-115">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="5d5f0-115">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="5d5f0-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5d5f0-116">Optional query parameters</span></span>

<span data-ttu-id="5d5f0-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d5f0-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d5f0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d5f0-118">Request headers</span></span>

| <span data-ttu-id="5d5f0-119">Name</span><span class="sxs-lookup"><span data-stu-id="5d5f0-119">Name</span></span>      |<span data-ttu-id="5d5f0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d5f0-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d5f0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d5f0-121">Authorization</span></span>  | <span data-ttu-id="5d5f0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d5f0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d5f0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d5f0-124">Content-Type</span></span>  | <span data-ttu-id="5d5f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d5f0-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d5f0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d5f0-126">Request body</span></span>
<span data-ttu-id="5d5f0-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5d5f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d5f0-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d5f0-128">Response</span></span>

<span data-ttu-id="5d5f0-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d5f0-129">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d5f0-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d5f0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d5f0-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d5f0-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="5d5f0-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d5f0-132">Response</span></span>
<span data-ttu-id="5d5f0-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d5f0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
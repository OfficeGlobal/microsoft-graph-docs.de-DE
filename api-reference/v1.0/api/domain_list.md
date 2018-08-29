# <a name="list-domains"></a><span data-ttu-id="6393c-101">Domänen auflisten</span><span class="sxs-lookup"><span data-stu-id="6393c-101">List domains</span></span>

<span data-ttu-id="6393c-102">Mit dieser API können Sie eine Liste von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="6393c-102">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6393c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6393c-103">Permissions</span></span>
<span data-ttu-id="6393c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6393c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6393c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6393c-106">Permission type</span></span>      | <span data-ttu-id="6393c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6393c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6393c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6393c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6393c-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6393c-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="6393c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6393c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6393c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6393c-111">Not supported.</span></span>    |
|<span data-ttu-id="6393c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6393c-112">Application</span></span> | <span data-ttu-id="6393c-113">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6393c-113">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6393c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6393c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6393c-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6393c-115">Optional query parameters</span></span>
<span data-ttu-id="6393c-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6393c-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6393c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6393c-117">Request headers</span></span>
| <span data-ttu-id="6393c-118">Name</span><span class="sxs-lookup"><span data-stu-id="6393c-118">Name</span></span>      |<span data-ttu-id="6393c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6393c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6393c-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6393c-120">Authorization</span></span>  | <span data-ttu-id="6393c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6393c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="6393c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6393c-123">Accept</span></span>         | <span data-ttu-id="6393c-124">application/json;</span><span class="sxs-lookup"><span data-stu-id="6393c-124">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="6393c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6393c-125">Request body</span></span>
<span data-ttu-id="6393c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6393c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6393c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6393c-127">Response</span></span>

<span data-ttu-id="6393c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domain](../resources/domain.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6393c-128">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6393c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6393c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6393c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6393c-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="6393c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6393c-131">Response</span></span>
<span data-ttu-id="6393c-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6393c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "id": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
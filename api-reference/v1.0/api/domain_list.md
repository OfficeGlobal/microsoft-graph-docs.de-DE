# <a name="list-domains"></a><span data-ttu-id="918e7-101">Domänen auflisten</span><span class="sxs-lookup"><span data-stu-id="918e7-101">List domains</span></span>

<span data-ttu-id="918e7-102">Mit dieser API können Sie eine Liste von Domänenobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="918e7-102">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="918e7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="918e7-103">Permissions</span></span>
<span data-ttu-id="918e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="918e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="918e7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="918e7-106">Permission type</span></span>      | <span data-ttu-id="918e7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="918e7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="918e7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="918e7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="918e7-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="918e7-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="918e7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="918e7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="918e7-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="918e7-111">Not supported.</span></span>    |
|<span data-ttu-id="918e7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="918e7-112">Application</span></span> | <span data-ttu-id="918e7-113">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="918e7-113">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="918e7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="918e7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="918e7-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="918e7-115">Optional query parameters</span></span>
<span data-ttu-id="918e7-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="918e7-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="918e7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="918e7-117">Request headers</span></span>
| <span data-ttu-id="918e7-118">Name</span><span class="sxs-lookup"><span data-stu-id="918e7-118">Name</span></span>      |<span data-ttu-id="918e7-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="918e7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="918e7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="918e7-120">Authorization</span></span>  | <span data-ttu-id="918e7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="918e7-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="918e7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="918e7-123">Accept</span></span>         | <span data-ttu-id="918e7-124">application/json;</span><span class="sxs-lookup"><span data-stu-id="918e7-124">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="918e7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="918e7-125">Request body</span></span>
<span data-ttu-id="918e7-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="918e7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="918e7-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="918e7-127">Response</span></span>

<span data-ttu-id="918e7-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domain](../resources/domain.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="918e7-128">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="918e7-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="918e7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="918e7-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="918e7-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains
```
##### <a name="response"></a><span data-ttu-id="918e7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="918e7-131">Response</span></span>
<span data-ttu-id="918e7-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="918e7-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "name": "contoso.com",
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
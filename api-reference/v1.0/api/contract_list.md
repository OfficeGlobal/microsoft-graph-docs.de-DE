# <a name="list-contracts"></a><span data-ttu-id="82494-101">Verträge auflisten</span><span class="sxs-lookup"><span data-stu-id="82494-101">List contracts</span></span>

<span data-ttu-id="82494-102">Mit dieser API können Sie eine Liste der einem Partnermandanten zugeordneten Objekte des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="82494-102">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="82494-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="82494-103">Permissions</span></span>

<span data-ttu-id="82494-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="82494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="82494-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82494-106">Permission type</span></span>      | <span data-ttu-id="82494-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82494-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82494-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82494-108">Delegated (work or school account)</span></span> | <span data-ttu-id="82494-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82494-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82494-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82494-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82494-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82494-111">Not supported.</span></span>    |
|<span data-ttu-id="82494-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82494-112">Application</span></span> | <span data-ttu-id="82494-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82494-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82494-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82494-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82494-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="82494-115">Optional query parameters</span></span>

<span data-ttu-id="82494-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="82494-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="82494-117">Für „customerId“, „defaultDomainName“ und „displayName“ wird Filterung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="82494-117">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82494-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82494-118">Request headers</span></span>

| <span data-ttu-id="82494-119">Name</span><span class="sxs-lookup"><span data-stu-id="82494-119">Name</span></span>      |<span data-ttu-id="82494-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82494-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82494-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="82494-121">Authorization</span></span>  | <span data-ttu-id="82494-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="82494-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82494-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82494-124">Request body</span></span>

<span data-ttu-id="82494-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="82494-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82494-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="82494-126">Response</span></span>

<span data-ttu-id="82494-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contract](../resources/contract.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82494-127">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82494-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82494-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82494-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82494-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="82494-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="82494-130">Response</span></span>

<span data-ttu-id="82494-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82494-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
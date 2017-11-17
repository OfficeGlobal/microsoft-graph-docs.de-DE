# <a name="get-contract"></a><span data-ttu-id="ae82d-101">Vertrag abrufen</span><span class="sxs-lookup"><span data-stu-id="ae82d-101">Get Contract</span></span>

<span data-ttu-id="ae82d-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs [contract](../resources/contract.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="ae82d-102">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae82d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae82d-103">Permissions</span></span>

<span data-ttu-id="ae82d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae82d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="ae82d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae82d-106">Permission type</span></span>      | <span data-ttu-id="ae82d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae82d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae82d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae82d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ae82d-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae82d-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae82d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae82d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae82d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae82d-111">Not supported.</span></span>    |
|<span data-ttu-id="ae82d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae82d-112">Application</span></span> | <span data-ttu-id="ae82d-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae82d-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae82d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae82d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae82d-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ae82d-115">Optional query parameters</span></span>

<span data-ttu-id="ae82d-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ae82d-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae82d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae82d-117">Request headers</span></span>

| <span data-ttu-id="ae82d-118">Name</span><span class="sxs-lookup"><span data-stu-id="ae82d-118">Name</span></span>      |<span data-ttu-id="ae82d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae82d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae82d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae82d-120">Authorization</span></span>  | <span data-ttu-id="ae82d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae82d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae82d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae82d-123">Request body</span></span>

<span data-ttu-id="ae82d-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ae82d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae82d-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae82d-125">Response</span></span>

<span data-ttu-id="ae82d-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [contract](../resources/contract.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae82d-126">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae82d-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae82d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae82d-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae82d-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="ae82d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae82d-129">Response</span></span>
<span data-ttu-id="ae82d-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae82d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
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
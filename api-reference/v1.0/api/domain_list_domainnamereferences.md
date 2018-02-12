# <a name="list-domainnamereferences"></a><span data-ttu-id="20033-101">domainNameReferences auflisten</span><span class="sxs-lookup"><span data-stu-id="20033-101">List domainNameReferences</span></span>

<span data-ttu-id="20033-p101">Dient zum Abrufen einer Liste von [directoryObject](../resources/directoryobject.md)-Objekten mit einem Verweis auf die Domäne. Die zurückgegebene Liste enthält alle Directory-Objekte, die von der Domäne abhängig sind.</span><span class="sxs-lookup"><span data-stu-id="20033-p101">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="20033-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="20033-104">Permissions</span></span>

<span data-ttu-id="20033-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="20033-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="20033-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20033-107">Permission type</span></span>      | <span data-ttu-id="20033-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20033-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20033-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20033-109">Delegated (work or school account)</span></span> | <span data-ttu-id="20033-110">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="20033-110">Directory.Read.All</span></span>    |
|<span data-ttu-id="20033-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20033-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20033-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20033-112">Not supported.</span></span>    |
|<span data-ttu-id="20033-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20033-113">Application</span></span> | <span data-ttu-id="20033-114">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20033-114">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20033-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20033-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="20033-116">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="20033-116">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="20033-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="20033-117">Optional query parameters</span></span>

<span data-ttu-id="20033-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="20033-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20033-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20033-119">Request headers</span></span>

| <span data-ttu-id="20033-120">Name</span><span class="sxs-lookup"><span data-stu-id="20033-120">Name</span></span>      |<span data-ttu-id="20033-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20033-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20033-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20033-122">Authorization</span></span>  | <span data-ttu-id="20033-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="20033-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20033-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20033-125">Request body</span></span>

<span data-ttu-id="20033-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="20033-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20033-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="20033-127">Response</span></span>

<span data-ttu-id="20033-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20033-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20033-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20033-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20033-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20033-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="20033-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="20033-131">Response</span></span>
<span data-ttu-id="20033-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20033-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
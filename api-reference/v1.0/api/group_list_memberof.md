# <a name="list-memberof"></a><span data-ttu-id="56db6-101">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="56db6-101">List memberOf</span></span>

<span data-ttu-id="56db6-102">Dient zum Abrufen von Gruppen, von denen die Gruppe ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="56db6-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="56db6-p101">Dieser Vorgang ist nicht transitiv. Im Gegensatz zum Abrufen der Office 365-Gruppen eines Benutzers werden hier alle Typen von Gruppen zurückgegeben, nicht nur Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="56db6-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="56db6-105">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="56db6-105">Prerequisites</span></span>
<span data-ttu-id="56db6-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="56db6-106">One of the following **scopes** is required to execute this API: *Group.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="56db6-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56db6-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56db6-108">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="56db6-108">Optional query parameters</span></span>
<span data-ttu-id="56db6-109">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="56db6-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56db6-110">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56db6-110">Request headers</span></span>
| <span data-ttu-id="56db6-111">Name</span><span class="sxs-lookup"><span data-stu-id="56db6-111">Name</span></span>       | <span data-ttu-id="56db6-112">Typ</span><span class="sxs-lookup"><span data-stu-id="56db6-112">Type</span></span> | <span data-ttu-id="56db6-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56db6-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56db6-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="56db6-114">Authorization</span></span>  | <span data-ttu-id="56db6-115">string</span><span class="sxs-lookup"><span data-stu-id="56db6-115">string</span></span>  | <span data-ttu-id="56db6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56db6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56db6-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56db6-118">Request body</span></span>
<span data-ttu-id="56db6-119">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="56db6-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56db6-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="56db6-120">Response</span></span>

<span data-ttu-id="56db6-121">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56db6-121">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56db6-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56db6-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56db6-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56db6-123">Request</span></span>
<span data-ttu-id="56db6-124">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56db6-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="56db6-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="56db6-125">Response</span></span>
<span data-ttu-id="56db6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56db6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
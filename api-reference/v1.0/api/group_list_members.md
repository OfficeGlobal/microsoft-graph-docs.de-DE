# <a name="list-members"></a><span data-ttu-id="f86a5-101">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="f86a5-101">List members</span></span>

<span data-ttu-id="f86a5-p101">Dient zum Abrufen einer Liste der direkten Mitglieder einer Gruppe. Eine Gruppe kann Benutzer, Kontakten und andere Gruppen als Mitglieder haben. Dieser Vorgang ist nicht transitiv.</span><span class="sxs-lookup"><span data-stu-id="f86a5-p101">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>
## <a name="permissions"></a><span data-ttu-id="f86a5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f86a5-105">Permissions</span></span>
<span data-ttu-id="f86a5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f86a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f86a5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f86a5-108">Permission type</span></span>      | <span data-ttu-id="f86a5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f86a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f86a5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f86a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f86a5-111">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f86a5-111">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="f86a5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f86a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f86a5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f86a5-113">Not supported.</span></span>    |
|<span data-ttu-id="f86a5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f86a5-114">Application</span></span> | <span data-ttu-id="f86a5-115">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f86a5-115">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f86a5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f86a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f86a5-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f86a5-117">Optional query parameters</span></span>
<span data-ttu-id="f86a5-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f86a5-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f86a5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f86a5-119">Request headers</span></span>
| <span data-ttu-id="f86a5-120">Name</span><span class="sxs-lookup"><span data-stu-id="f86a5-120">Name</span></span>       | <span data-ttu-id="f86a5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f86a5-121">Type</span></span> | <span data-ttu-id="f86a5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f86a5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f86a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f86a5-123">Authorization</span></span>  | <span data-ttu-id="f86a5-124">string</span><span class="sxs-lookup"><span data-stu-id="f86a5-124">string</span></span>  | <span data-ttu-id="f86a5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f86a5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f86a5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f86a5-127">Request body</span></span>
<span data-ttu-id="f86a5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f86a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f86a5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f86a5-129">Response</span></span>

<span data-ttu-id="f86a5-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f86a5-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f86a5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f86a5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f86a5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f86a5-132">Request</span></span>
<span data-ttu-id="f86a5-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f86a5-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="f86a5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f86a5-134">Response</span></span>
<span data-ttu-id="f86a5-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f86a5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
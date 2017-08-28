# <a name="get-permission"></a><span data-ttu-id="57b8f-101">Berechtigung abrufen</span><span class="sxs-lookup"><span data-stu-id="57b8f-101">Get permission</span></span>

<span data-ttu-id="57b8f-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Berechtigungsobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="57b8f-102">Retrieve the properties and relationships of permission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57b8f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="57b8f-103">Permissions</span></span>
<span data-ttu-id="57b8f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57b8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57b8f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57b8f-106">Permission type</span></span>      | <span data-ttu-id="57b8f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57b8f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57b8f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57b8f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="57b8f-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b8f-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="57b8f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57b8f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57b8f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b8f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="57b8f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57b8f-112">Application</span></span> | <span data-ttu-id="57b8f-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b8f-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57b8f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57b8f-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/root:/{path}:/permissions/{perm-id}
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57b8f-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="57b8f-115">Optional query parameters</span></span>
<span data-ttu-id="57b8f-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="57b8f-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="57b8f-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57b8f-117">Request body</span></span>
<span data-ttu-id="57b8f-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="57b8f-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57b8f-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="57b8f-119">Response</span></span>

<span data-ttu-id="57b8f-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [Berechtigungs](../resources/permission.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57b8f-120">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57b8f-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57b8f-121">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57b8f-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57b8f-122">Request</span></span>

<span data-ttu-id="57b8f-123">Nachfolgend finden Sie ein Beispiel der Anforderung für den Zugriff auf eine Berechtigung im Stammordner.</span><span class="sxs-lookup"><span data-stu-id="57b8f-123">Here is an example of the request to access a permission on the root folder.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_permission"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
```
##### <a name="response"></a><span data-ttu-id="57b8f-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="57b8f-124">Response</span></span>
<span data-ttu-id="57b8f-125">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="57b8f-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 762

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="57b8f-126">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="57b8f-126">Remarks</span></span>

<span data-ttu-id="57b8f-127">Die [Permission](../resources/permission.md)-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die die Ressource dargestellt.</span><span class="sxs-lookup"><span data-stu-id="57b8f-127">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="57b8f-p102">Berechtigungen für ein [**link**](../resources/sharinglink.md)-Facet stellen Freigabe-Links dar, die für das Element erstellt wurden. Freigabelinks enthalten ein eindeutiges Token, mit dem alle Benutzer, die über den Link verfügen, Zugriff auf das Element haben.</span><span class="sxs-lookup"><span data-stu-id="57b8f-p102">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="57b8f-130">Berechtigungen mit einem [**invitation**](../resources/sharinginvitation.md)-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen für Zugriff auf die Datei hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="57b8f-130">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->

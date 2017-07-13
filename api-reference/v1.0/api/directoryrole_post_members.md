<span data-ttu-id="49355-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49355-p101">Bearer token. Required.</span></span>  | Bearer {token}. Erforderlich. |
| <span data-ttu-id="49355-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49355-114">Content-Type</span></span>  | <span data-ttu-id="49355-115">application/json</span><span class="sxs-lookup"><span data-stu-id="49355-115">application/json</span></span>  |

## <span data-ttu-id="49355-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49355-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="49355-117">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="49355-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <span data-ttu-id="49355-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="49355-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="49355-119">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49355-119">If successful, this method returns `204, No Content` response code.</span></span>

## <span data-ttu-id="49355-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49355-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="49355-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49355-121">Request</span></span>
<a id="request" class="xliff"></a>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <span data-ttu-id="49355-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="49355-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="49355-123">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="49355-123">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
<span data-ttu-id="9da30-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9da30-p101">Bearer {token}. Required.</span></span>  | Bearer {token}. Erforderlich. |
| <span data-ttu-id="9da30-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9da30-114">Content-Type</span></span>  | <span data-ttu-id="9da30-115">application/json</span><span class="sxs-lookup"><span data-stu-id="9da30-115">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9da30-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9da30-116">Request body</span></span>
<span data-ttu-id="9da30-117">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9da30-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9da30-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="9da30-118">Response</span></span>

<span data-ttu-id="9da30-119">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9da30-119">If successful, this method returns `204, No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9da30-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9da30-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9da30-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9da30-121">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="9da30-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="9da30-122">Response</span></span>
<span data-ttu-id="9da30-123">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="9da30-123">Note: The response object shown here may be truncated for brevity.</span></span> 
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
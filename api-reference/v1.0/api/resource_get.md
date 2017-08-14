<span data-ttu-id="dcd41-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcd41-p101">Bearer {token}. Required.</span></span>  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a><span data-ttu-id="dcd41-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dcd41-115">Request body</span></span>
<span data-ttu-id="dcd41-116">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dcd41-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcd41-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcd41-117">Response</span></span>

<span data-ttu-id="dcd41-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die Binärdaten des Bilds oder der Datei im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dcd41-118">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="dcd41-119">Hinweis: Bilder werden nicht direkt in einem Browser gerendert, da zum Abrufen eine Autorisierung erforderlich ist, ebenso wie für den Rest des Seiteninhalts.</span><span class="sxs-lookup"><span data-stu-id="dcd41-119">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="dcd41-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dcd41-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcd41-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcd41-121">Request</span></span>
<span data-ttu-id="dcd41-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dcd41-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="dcd41-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcd41-123">Response</span></span>
<span data-ttu-id="dcd41-124">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dcd41-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

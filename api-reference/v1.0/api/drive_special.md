<span data-ttu-id="8b1ed-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b1ed-p103">Bearer {token}. Required.</span></span> | Bearer {token}. Erforderlich. |


## <a name="request-body"></a><span data-ttu-id="8b1ed-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b1ed-128">Request body</span></span>
<span data-ttu-id="8b1ed-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8b1ed-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b1ed-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b1ed-130">Response</span></span>

<span data-ttu-id="8b1ed-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [driveItem](../resources/driveitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b1ed-131">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b1ed-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b1ed-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8b1ed-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b1ed-133">Request</span></span>
<span data-ttu-id="8b1ed-134">Hier ist ein Beispiel für die Anforderung der Laufwerke des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="8b1ed-134">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="8b1ed-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b1ed-135">Response</span></span>
<span data-ttu-id="8b1ed-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b1ed-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a><span data-ttu-id="8b1ed-137">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="8b1ed-137">Remarks</span></span>

<span data-ttu-id="8b1ed-138">Um die untergeordneten Elemente eines speziellen Ordners anzufordern, können Sie die `children`-Sammlung anfordern oder die Option [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) verwenden, um die Sammlung untergeordneter Elemente zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="8b1ed-138">To request the children of a special folder, you can request the `children` collection or use the [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->

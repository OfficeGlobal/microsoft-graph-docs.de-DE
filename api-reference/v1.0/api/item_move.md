<span data-ttu-id="ae113-p103">**Hinweis:** Die `"id:" "root"`-Syntax kann nicht beim Verschieben von Elementen in den Stammordner einer OneDrive-Umgebung verwendet werden. Sie müssen entweder die echte ID des Stammordners oder `{"path": "/drive/root"}` für die übergeordnete Referenz verwenden.</span><span class="sxs-lookup"><span data-stu-id="ae113-p103">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

**Hinweis:** Die `"id:" "root"`-Syntax kann nicht beim Verschieben von Elementen in den Stammordner einer OneDrive-Umgebung verwendet werden. Sie müssen entweder die echte ID des Stammordners oder `{"path": "/drive/root"}` für die übergeordnete Referenz verwenden.

## <span data-ttu-id="ae113-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae113-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ae113-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae113-126">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="ae113-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae113-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="ae113-128">In diesem Beispiel wird ein durch {item-id} angegebenes Element in den Ordner **Dokumente** in der OneDrive-Umgebung des Benutzers verschoben.</span><span class="sxs-lookup"><span data-stu-id="ae113-128">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

## <span data-ttu-id="ae113-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae113-129">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ae113-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ae113-130">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

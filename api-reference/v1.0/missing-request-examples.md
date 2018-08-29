# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="52712-101">Hilfsprogramme (Beispiele, die nicht in den Dokumenten enthalten sind)</span><span class="sxs-lookup"><span data-stu-id="52712-101">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="52712-102">Dies sind Dinge, die ich in den Dokumenten hinzufügen musste, damit das Markdown-Scannertool die Graph-Dokumente ordnungsgemäß verarbeiten kann.</span><span class="sxs-lookup"><span data-stu-id="52712-102">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="52712-103">Definieren von /me als Singleton</span><span class="sxs-lookup"><span data-stu-id="52712-103">Define the /me as singleton</span></span>

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="52712-104">Definieren von Laufwerken als abfragbares Entityset</span><span class="sxs-lookup"><span data-stu-id="52712-104">Define drives as an queryable entityset</span></span>
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="52712-105">Definieren von Benutzern als abfragbares Entityset</span><span class="sxs-lookup"><span data-stu-id="52712-105">define users as an queryable entityset</span></span>

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```

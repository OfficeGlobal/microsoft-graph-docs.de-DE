# <span data-ttu-id="e7e53-101">Einen neuen Ordner erstellen</span><span class="sxs-lookup"><span data-stu-id="e7e53-101">Create a new folder</span></span>
<a id="create-a-new-folder" class="xliff"></a>

<span data-ttu-id="e7e53-102">Erstellt einen neuen Ordner oder ein [DriveItem](../resources/driveitem.md)-Element in einem [Laufwerk](../resources/drive.md) mit einem angegebenen übergeordneten Element oder Pfad.</span><span class="sxs-lookup"><span data-stu-id="e7e53-102">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <span data-ttu-id="e7e53-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e7e53-103">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="e7e53-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="e7e53-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="e7e53-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7e53-105">Files.ReadWrite</span></span>
* <span data-ttu-id="e7e53-106">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7e53-106">Files.ReadWrite.All</span></span>
* <span data-ttu-id="e7e53-107">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7e53-107">Sites.ReadWrite.All</span></span>


## <span data-ttu-id="e7e53-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7e53-108">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/children
POST /me/drive/items/{parent-item-id}/children
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
```

## <span data-ttu-id="e7e53-109">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7e53-109">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="e7e53-110">Geben Sie im Anforderungstext eine JSON-Darstellung der zu erstellenden [DriveItem](../resources/driveitem.md)-Ressource an.</span><span class="sxs-lookup"><span data-stu-id="e7e53-110">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>


## <span data-ttu-id="e7e53-111">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7e53-111">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="e7e53-112">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und die [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7e53-112">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="e7e53-113">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7e53-113">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="e7e53-114">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7e53-114">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="e7e53-115">Nachfolgend finden Sie ein Beispiel der Anforderung zum Erstellen eines neues Ordners am OneDrive-Stamm des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e7e53-115">Here is an example of the request to create a new folder in the user's OneDrive root.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_from_item"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { }
}
```

##### <span data-ttu-id="e7e53-116">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7e53-116">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="e7e53-117">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e7e53-117">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "createdDateTime": "20160920T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "20160920T14:34:00Z",
  "name": "New Folder",
  "parentReference": {
    "driveId": "5FE38E3C-051C-4D55-9B83-8A437658275B",
    "id": "E67A8F34-B0AA-46E1-8FF7-0750A29553DF",
    "path": "/drive/root:/"
  },
  "size": 0,
  "folder": {
    "childCount": 0
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create children",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

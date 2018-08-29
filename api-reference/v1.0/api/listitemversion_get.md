# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="9a6a6-101">ListItemVersion-Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="9a6a6-101">Get a ListItemVersion resource (preview)</span></span>

<span data-ttu-id="9a6a6-102">Rufen Sie die Metadaten für eine bestimmte Version eines [ListItem](../resources/listitem.md) ab.</span><span class="sxs-lookup"><span data-stu-id="9a6a6-102">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a6a6-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a6a6-103">Permissions</span></span>

<span data-ttu-id="9a6a6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a6a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="9a6a6-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a6a6-106">Permission type</span></span>             | <span data-ttu-id="9a6a6-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a6a6-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9a6a6-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a6a6-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a6a6-109">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a6a6-109">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="9a6a6-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a6a6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a6a6-111">N/V</span><span class="sxs-lookup"><span data-stu-id="9a6a6-111">n/a</span></span>                                         |
| <span data-ttu-id="9a6a6-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a6a6-112">Application</span></span>                            | <span data-ttu-id="9a6a6-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a6a6-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="9a6a6-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a6a6-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="9a6a6-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a6a6-115">Response</span></span>

<span data-ttu-id="9a6a6-116">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ListItemVersion](../resources/listitemversion.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a6a6-116">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="9a6a6-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a6a6-117">Example</span></span>

<span data-ttu-id="9a6a6-118">In diesem Beispiel wird eine Version eines listItem abgerufen und die Fields-Auflistung erweitert, um die Werte der Felder im listItem anzufordern.</span><span class="sxs-lookup"><span data-stu-id="9a6a6-118">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="9a6a6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a6a6-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="9a6a6-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a6a6-120">Response</span></span>

<span data-ttu-id="9a6a6-121">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="9a6a6-121">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->

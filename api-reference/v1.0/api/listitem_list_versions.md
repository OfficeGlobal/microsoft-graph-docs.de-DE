# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="5e821-101">Auflisten von einer ListItem-Versionen</span><span class="sxs-lookup"><span data-stu-id="5e821-101">Listing versions of a ListItem (preview)</span></span>

<span data-ttu-id="5e821-102">SharePoint kann auch so konfiguriert werden, dass für Listenelemente ein Verlauf beibehalten wird.</span><span class="sxs-lookup"><span data-stu-id="5e821-102">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="5e821-103">Vorherige Versionen können je nach Administratoreinstellungen für einen begrenzten Zeitraum beibehalten werden, diese können pro Benutzer oder Speicherort eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="5e821-103">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e821-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5e821-104">Permissions</span></span>

<span data-ttu-id="5e821-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="5e821-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5e821-107">Permission type</span></span>             | <span data-ttu-id="5e821-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5e821-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5e821-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5e821-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e821-110">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e821-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="5e821-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5e821-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e821-112">N/V</span><span class="sxs-lookup"><span data-stu-id="5e821-112">n/a</span></span>                                         |
| <span data-ttu-id="5e821-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5e821-113">Application</span></span>                            | <span data-ttu-id="5e821-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e821-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="5e821-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e821-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="5e821-116">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e821-116">Response</span></span>

<span data-ttu-id="5e821-117">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ListItemVersion](../resources/listitemversion.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e821-117">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="5e821-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e821-118">Example</span></span>

<span data-ttu-id="5e821-119">In diesem Beispiel werden die Versionen eines ListItem in einer SharePoint-Liste abgerufen:</span><span class="sxs-lookup"><span data-stu-id="5e821-119">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="5e821-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e821-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="5e821-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e821-121">Response</span></span>

<span data-ttu-id="5e821-122">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="5e821-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->

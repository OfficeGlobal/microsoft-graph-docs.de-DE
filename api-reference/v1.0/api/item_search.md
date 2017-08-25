# <a name="search-for-a-driveitem-within-a-drive"></a><span data-ttu-id="48e61-101">DriveItem in einem Laufwerk suchen</span><span class="sxs-lookup"><span data-stu-id="48e61-101">Search for a DriveItem within a drive</span></span>

<span data-ttu-id="48e61-p101">Durchsuchen Sie die Hierarchie der Elemente nach Elementen, die mit einer Abfrage übereinstimmen. Sie können eine Ordnerhierarchie, ein gesamtes Laufwerk oder die für den aktuellen Benutzer freigegebenen Dateien durchsuchen.</span><span class="sxs-lookup"><span data-stu-id="48e61-p101">Search the hierarchy of items for items matching a query. You can search within a folder hierarhcy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="48e61-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48e61-104">Permissions</span></span>
<span data-ttu-id="48e61-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48e61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48e61-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48e61-107">Permission type</span></span>      | <span data-ttu-id="48e61-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48e61-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="48e61-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48e61-109">Delegated (work or school account)</span></span> | <span data-ttu-id="48e61-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e61-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="48e61-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48e61-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48e61-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e61-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="48e61-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48e61-113">Application</span></span> | <span data-ttu-id="48e61-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e61-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="48e61-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48e61-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```
GET /me/drive/root/search(q='{search-text}')
GET /me/drive/items/{item-id}/search(q='{search-text}')
GET /me/drive/root:/{item-path}:/search(q='{search-text}')
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48e61-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="48e61-116">Optional query parameters</span></span>
<span data-ttu-id="48e61-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48e61-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="48e61-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48e61-118">Request body</span></span>
<span data-ttu-id="48e61-119">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="48e61-119">Do not supply a request body for this method.</span></span>

#### <a name="function-parameters"></a><span data-ttu-id="48e61-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="48e61-120">Function parameters</span></span>

| <span data-ttu-id="48e61-121">Name</span><span class="sxs-lookup"><span data-stu-id="48e61-121">Name</span></span> | <span data-ttu-id="48e61-122">Wert</span><span class="sxs-lookup"><span data-stu-id="48e61-122">Value</span></span>  | <span data-ttu-id="48e61-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48e61-123">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| `q`  | <span data-ttu-id="48e61-124">string</span><span class="sxs-lookup"><span data-stu-id="48e61-124">string</span></span> | <span data-ttu-id="48e61-p103">Der zum Durchsuchen der Elemente verwendete Abfragetext. Werte werden möglicherweise mit mehreren Feldern wie Dateiname, Metadaten und Dateiinhalt abgeglichen.</span><span class="sxs-lookup"><span data-stu-id="48e61-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="48e61-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48e61-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="48e61-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48e61-128">Request</span></span>

<span data-ttu-id="48e61-129">Es folgt ein Beispiel für die Anforderung zum Durchsuchen von OneDrive des aktuellen Benutzers</span><span class="sxs-lookup"><span data-stu-id="48e61-129">Here is an example of the request searching the current user's OneDrive</span></span>
<!-- {
  "blockType": "request",
  "name": "item_search"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/search(q='{search-query}')
```

##### <a name="response"></a><span data-ttu-id="48e61-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="48e61-130">Response</span></span>
<span data-ttu-id="48e61-p104">Diese Methode gibt ein Objekt mit einer Sammlung von [DriveItems](../resources/driveitem.md)-Elementen zurück, die den Suchkriterien entsprechen. Wenn keine Elemente gefunden werden, wird eine leere Sammlung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48e61-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="48e61-p105">Wenn diese Methode zu viele Ergebnisse zurückgibt, ist die Antwort seitennummeriert und enthält eine **@odata.nextLink**-Eigenschaft mit einer URL zur nächsten Ergebnisseite. Sie können den `$top`-Abfrageparameter zum Angeben der Anzahl der Elemente auf einer Seite verwenden.</span><span class="sxs-lookup"><span data-stu-id="48e61-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="48e61-135">Suchen nach Elementen, auf die Benutzer zugreifen können</span><span class="sxs-lookup"><span data-stu-id="48e61-135">Searching for items a user can access</span></span>

<span data-ttu-id="48e61-p106">Neben Elementen in einem Laufwerk kann Ihre App die Suche auf Elemente erweitern, die für den aktuellen Benutzer freigegeben wurden. Verwenden Sie zum Erweitern des Suchbereichs die **search**-Methode für die [Laufwerk](../resources/drive.md)ressource.</span><span class="sxs-lookup"><span data-stu-id="48e61-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

##### <a name="request"></a><span data-ttu-id="48e61-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48e61-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "item_search_all"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/search(q='{search-query}')
```

##### <a name="response"></a><span data-ttu-id="48e61-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="48e61-139">Response</span></span>
<span data-ttu-id="48e61-p107">Die Antworten können beim Durchsuchen der **Laufwerk**ressource Elemente enthalten, die sich außerhalb des Laufwerks befinden (Elemente, die für den aktuellen Benutzer freigegeben sind). Diese Elemente enthalten das [**remoteItem**](../resources/remoteitem.md)-Facet, das angibt, dass sie außerhalb des Ziellaufwerks gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="48e61-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: search",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Items/Search items"
}-->

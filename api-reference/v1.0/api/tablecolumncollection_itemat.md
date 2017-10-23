# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="a91d0-101">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="a91d0-101">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="a91d0-102">Ruft eine Spalte anhand ihrer Position in der Auflistung ab.</span><span class="sxs-lookup"><span data-stu-id="a91d0-102">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="a91d0-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a91d0-103">Permissions</span></span>
<span data-ttu-id="a91d0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a91d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a91d0-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a91d0-106">Permission type</span></span>      | <span data-ttu-id="a91d0-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a91d0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a91d0-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a91d0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a91d0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a91d0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a91d0-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a91d0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a91d0-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a91d0-111">Not supported.</span></span>    |
|<span data-ttu-id="a91d0-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a91d0-112">Application</span></span> | <span data-ttu-id="a91d0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a91d0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a91d0-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a91d0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="a91d0-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a91d0-115">Request headers</span></span>
| <span data-ttu-id="a91d0-116">Name</span><span class="sxs-lookup"><span data-stu-id="a91d0-116">Name</span></span>       | <span data-ttu-id="a91d0-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a91d0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a91d0-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a91d0-118">Authorization</span></span>  | <span data-ttu-id="a91d0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a91d0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a91d0-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a91d0-121">Request body</span></span>
<span data-ttu-id="a91d0-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a91d0-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a91d0-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="a91d0-123">Parameter</span></span>    | <span data-ttu-id="a91d0-124">Typ</span><span class="sxs-lookup"><span data-stu-id="a91d0-124">Type</span></span>   |<span data-ttu-id="a91d0-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a91d0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a91d0-126">Index</span><span class="sxs-lookup"><span data-stu-id="a91d0-126">index</span></span>|<span data-ttu-id="a91d0-127">number</span><span class="sxs-lookup"><span data-stu-id="a91d0-127">number</span></span>|<span data-ttu-id="a91d0-p103">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="a91d0-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="a91d0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a91d0-130">Response</span></span>

<span data-ttu-id="a91d0-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableColumn](../resources/tablecolumn.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a91d0-131">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a91d0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a91d0-132">Example</span></span>
<span data-ttu-id="a91d0-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a91d0-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a91d0-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a91d0-134">Request</span></span>
<span data-ttu-id="a91d0-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a91d0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="a91d0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a91d0-136">Response</span></span>
<span data-ttu-id="a91d0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a91d0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
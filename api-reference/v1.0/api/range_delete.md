# <a name="range-delete"></a><span data-ttu-id="236f9-101">Range: delete</span><span class="sxs-lookup"><span data-stu-id="236f9-101">Range: delete</span></span>

<span data-ttu-id="236f9-102">Löscht die einem Bereich zugeordneten Zellen.</span><span class="sxs-lookup"><span data-stu-id="236f9-102">Deletes the cells associated with the range.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="236f9-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="236f9-103">Prerequisites</span></span>
<span data-ttu-id="236f9-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="236f9-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="236f9-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="236f9-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="236f9-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="236f9-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(<address>)/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="236f9-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="236f9-107">Request headers</span></span>
| <span data-ttu-id="236f9-108">Name</span><span class="sxs-lookup"><span data-stu-id="236f9-108">Name</span></span>       | <span data-ttu-id="236f9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="236f9-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="236f9-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="236f9-110">Authorization</span></span>  | <span data-ttu-id="236f9-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f9-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="236f9-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="236f9-113">Request body</span></span>
<span data-ttu-id="236f9-114">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="236f9-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="236f9-115">Parameter</span><span class="sxs-lookup"><span data-stu-id="236f9-115">Parameter</span></span>    | <span data-ttu-id="236f9-116">Typ</span><span class="sxs-lookup"><span data-stu-id="236f9-116">Type</span></span>   |<span data-ttu-id="236f9-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="236f9-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="236f9-118">Shift</span><span class="sxs-lookup"><span data-stu-id="236f9-118">shift</span></span>|<span data-ttu-id="236f9-119">string</span><span class="sxs-lookup"><span data-stu-id="236f9-119">string</span></span>|<span data-ttu-id="236f9-p102">Gibt an, wohin die Zellen verschoben werden.  Mögliche Werte: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="236f9-p102">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="236f9-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="236f9-122">Response</span></span>

<span data-ttu-id="236f9-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="236f9-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="236f9-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="236f9-125">Example</span></span>
<span data-ttu-id="236f9-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="236f9-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="236f9-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="236f9-127">Request</span></span>
<span data-ttu-id="236f9-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="236f9-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="236f9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="236f9-129">Response</span></span>
<span data-ttu-id="236f9-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="236f9-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
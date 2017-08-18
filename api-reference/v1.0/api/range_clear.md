# <a name="range-clear"></a><span data-ttu-id="f0d93-101">Range: clear</span><span class="sxs-lookup"><span data-stu-id="f0d93-101">Range: clear</span></span>

<span data-ttu-id="f0d93-102">Löscht Bereichswerte, Format, Füllung, Rahmen usw.</span><span class="sxs-lookup"><span data-stu-id="f0d93-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0d93-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f0d93-103">Prerequisites</span></span>
<span data-ttu-id="f0d93-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="f0d93-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="f0d93-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0d93-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="f0d93-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0d93-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/clear
GET /workbook/worksheets/{id|name}/range(<address>)/clear
GET /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="f0d93-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f0d93-107">Request headers</span></span>
| <span data-ttu-id="f0d93-108">Name</span><span class="sxs-lookup"><span data-stu-id="f0d93-108">Name</span></span>       | <span data-ttu-id="f0d93-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0d93-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0d93-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0d93-110">Authorization</span></span>  | <span data-ttu-id="f0d93-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f0d93-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f0d93-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f0d93-113">Request body</span></span>
<span data-ttu-id="f0d93-114">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f0d93-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f0d93-115">Parameter</span><span class="sxs-lookup"><span data-stu-id="f0d93-115">Parameter</span></span>    | <span data-ttu-id="f0d93-116">Typ</span><span class="sxs-lookup"><span data-stu-id="f0d93-116">Type</span></span>   |<span data-ttu-id="f0d93-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0d93-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0d93-118">applyTo</span><span class="sxs-lookup"><span data-stu-id="f0d93-118">applyTo</span></span>|<span data-ttu-id="f0d93-119">string</span><span class="sxs-lookup"><span data-stu-id="f0d93-119">string</span></span>|<span data-ttu-id="f0d93-p102">Optional. Bestimmt den Typ der Löschaktion.  Mögliche Werte: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="f0d93-p102">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="f0d93-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0d93-123">Response</span></span>

<span data-ttu-id="f0d93-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0d93-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0d93-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f0d93-126">Example</span></span>
<span data-ttu-id="f0d93-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f0d93-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f0d93-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0d93-128">Request</span></span>
<span data-ttu-id="f0d93-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f0d93-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="f0d93-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0d93-130">Response</span></span>
<span data-ttu-id="f0d93-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f0d93-131">Here is an example of the response.</span></span> 
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
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
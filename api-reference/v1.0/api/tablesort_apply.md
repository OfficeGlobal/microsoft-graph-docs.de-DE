# <a name="tablesort-apply"></a><span data-ttu-id="9b5b5-101">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="9b5b5-101">TableSort: apply</span></span>

<span data-ttu-id="9b5b5-102">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b5b5-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b5b5-103">Prerequisites</span></span>
<span data-ttu-id="9b5b5-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="9b5b5-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="9b5b5-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b5b5-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="9b5b5-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b5b5-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="9b5b5-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b5b5-107">Request headers</span></span>
| <span data-ttu-id="9b5b5-108">Name</span><span class="sxs-lookup"><span data-stu-id="9b5b5-108">Name</span></span>       | <span data-ttu-id="9b5b5-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b5b5-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b5b5-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b5b5-110">Authorization</span></span>  | <span data-ttu-id="9b5b5-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9b5b5-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b5b5-113">Request body</span></span>
<span data-ttu-id="9b5b5-114">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b5b5-115">Parameter</span><span class="sxs-lookup"><span data-stu-id="9b5b5-115">Parameter</span></span>    | <span data-ttu-id="9b5b5-116">Typ</span><span class="sxs-lookup"><span data-stu-id="9b5b5-116">Type</span></span>   |<span data-ttu-id="9b5b5-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b5b5-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b5b5-118">fields</span><span class="sxs-lookup"><span data-stu-id="9b5b5-118">fields</span></span>|<span data-ttu-id="9b5b5-119">SortField</span><span class="sxs-lookup"><span data-stu-id="9b5b5-119">SortField</span></span>|<span data-ttu-id="9b5b5-120">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="9b5b5-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="9b5b5-121">matchCase</span></span>|<span data-ttu-id="9b5b5-122">boolean</span><span class="sxs-lookup"><span data-stu-id="9b5b5-122">boolean</span></span>|<span data-ttu-id="9b5b5-p102">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="9b5b5-125">method</span><span class="sxs-lookup"><span data-stu-id="9b5b5-125">method</span></span>|<span data-ttu-id="9b5b5-126">string</span><span class="sxs-lookup"><span data-stu-id="9b5b5-126">string</span></span>|<span data-ttu-id="9b5b5-p103">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-p103">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="9b5b5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b5b5-130">Response</span></span>

<span data-ttu-id="9b5b5-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b5b5-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b5b5-133">Example</span></span>
<span data-ttu-id="9b5b5-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b5b5-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b5b5-135">Request</span></span>
<span data-ttu-id="9b5b5-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="9b5b5-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b5b5-137">Response</span></span>
<span data-ttu-id="9b5b5-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9b5b5-138">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
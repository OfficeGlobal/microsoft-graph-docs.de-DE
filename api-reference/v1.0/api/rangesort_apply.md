# <a name="rangesort-apply"></a><span data-ttu-id="c5c18-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="c5c18-101">RangeSort: apply</span></span>

<span data-ttu-id="c5c18-102">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="c5c18-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5c18-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5c18-103">Prerequisites</span></span>
<span data-ttu-id="c5c18-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="c5c18-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="c5c18-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5c18-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="c5c18-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5c18-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(<address>)/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="c5c18-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5c18-107">Request headers</span></span>
| <span data-ttu-id="c5c18-108">Name</span><span class="sxs-lookup"><span data-stu-id="c5c18-108">Name</span></span>       | <span data-ttu-id="c5c18-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5c18-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5c18-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5c18-110">Authorization</span></span>  | <span data-ttu-id="c5c18-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5c18-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c5c18-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5c18-113">Request body</span></span>
<span data-ttu-id="c5c18-114">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c5c18-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5c18-115">Parameter</span><span class="sxs-lookup"><span data-stu-id="c5c18-115">Parameter</span></span>    | <span data-ttu-id="c5c18-116">Typ</span><span class="sxs-lookup"><span data-stu-id="c5c18-116">Type</span></span>   |<span data-ttu-id="c5c18-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5c18-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5c18-118">fields</span><span class="sxs-lookup"><span data-stu-id="c5c18-118">fields</span></span>|<span data-ttu-id="c5c18-119">SortField</span><span class="sxs-lookup"><span data-stu-id="c5c18-119">SortField</span></span>|<span data-ttu-id="c5c18-120">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c5c18-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="c5c18-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="c5c18-121">matchCase</span></span>|<span data-ttu-id="c5c18-122">boolean</span><span class="sxs-lookup"><span data-stu-id="c5c18-122">boolean</span></span>|<span data-ttu-id="c5c18-p102">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="c5c18-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="c5c18-125">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="c5c18-125">hasHeaders</span></span>|<span data-ttu-id="c5c18-126">boolean</span><span class="sxs-lookup"><span data-stu-id="c5c18-126">boolean</span></span>|<span data-ttu-id="c5c18-p103">Optional. Gibt an, ob der Bereich eine Kopfzeile aufweist.</span><span class="sxs-lookup"><span data-stu-id="c5c18-p103">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="c5c18-129">orientation</span><span class="sxs-lookup"><span data-stu-id="c5c18-129">orientation</span></span>|<span data-ttu-id="c5c18-130">string</span><span class="sxs-lookup"><span data-stu-id="c5c18-130">string</span></span>|<span data-ttu-id="c5c18-p104">Optional. Gibt an, ob der Vorgang Zeilen oder Spalten sortiert.  Die folgenden Werte sind möglich: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="c5c18-p104">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="c5c18-134">method</span><span class="sxs-lookup"><span data-stu-id="c5c18-134">method</span></span>|<span data-ttu-id="c5c18-135">string</span><span class="sxs-lookup"><span data-stu-id="c5c18-135">string</span></span>|<span data-ttu-id="c5c18-p105">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="c5c18-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="c5c18-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5c18-139">Response</span></span>

<span data-ttu-id="c5c18-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5c18-p106">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5c18-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5c18-142">Example</span></span>
<span data-ttu-id="c5c18-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c5c18-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5c18-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5c18-144">Request</span></span>
<span data-ttu-id="c5c18-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5c18-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="c5c18-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5c18-146">Response</span></span>
<span data-ttu-id="c5c18-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c5c18-147">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="worksheet-usedrange"></a><span data-ttu-id="8a123-101">Arbeitsblatt: UsedRange</span><span class="sxs-lookup"><span data-stu-id="8a123-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="8a123-p101">Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.</span><span class="sxs-lookup"><span data-stu-id="8a123-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a123-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8a123-104">Prerequisites</span></span>
<span data-ttu-id="8a123-105">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="8a123-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="8a123-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a123-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="8a123-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a123-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="optional-request-parameter"></a><span data-ttu-id="8a123-108">Optionaler Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="8a123-108">Optional request parameter</span></span>
<span data-ttu-id="8a123-109">Stellen Sie in der Anforderungs-URL einen optionalen Abfrageparameter bereit.</span><span class="sxs-lookup"><span data-stu-id="8a123-109">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="8a123-110">Parameter</span><span class="sxs-lookup"><span data-stu-id="8a123-110">Parameter</span></span>    | <span data-ttu-id="8a123-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8a123-111">Type</span></span>   |<span data-ttu-id="8a123-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a123-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a123-113">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="8a123-113">valuesOnly</span></span>|<span data-ttu-id="8a123-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8a123-114">Boolean</span></span>|<span data-ttu-id="8a123-p102">Optional. Betrachtet nur Zellen mit Werten als verwendet (ignoriert die Formatierung).</span><span class="sxs-lookup"><span data-stu-id="8a123-p102">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|


## <a name="request-headers"></a><span data-ttu-id="8a123-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a123-117">Request headers</span></span>
| <span data-ttu-id="8a123-118">Name</span><span class="sxs-lookup"><span data-stu-id="8a123-118">Name</span></span>       | <span data-ttu-id="8a123-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a123-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a123-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a123-120">Authorization</span></span>  | <span data-ttu-id="8a123-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a123-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8a123-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a123-123">Response</span></span>

<span data-ttu-id="8a123-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a123-124">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a123-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a123-125">Example</span></span>
<span data-ttu-id="8a123-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8a123-126">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a123-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a123-127">Request</span></span>
<span data-ttu-id="8a123-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a123-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
Content-type: application/json

```

##### <a name="response"></a><span data-ttu-id="8a123-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a123-129">Response</span></span>
<span data-ttu-id="8a123-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a123-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="rangesort-apply"></a><span data-ttu-id="18474-101">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="18474-101">RangeSort: apply</span></span>

<span data-ttu-id="18474-102">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="18474-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="18474-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18474-103">Permissions</span></span>
<span data-ttu-id="18474-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="18474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18474-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18474-106">Permission type</span></span>      | <span data-ttu-id="18474-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18474-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18474-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18474-108">Delegated (work or school account)</span></span> | <span data-ttu-id="18474-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18474-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="18474-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18474-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18474-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18474-111">Not supported.</span></span>    |
|<span data-ttu-id="18474-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18474-112">Application</span></span> | <span data-ttu-id="18474-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18474-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18474-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18474-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(<address>)/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="18474-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18474-115">Request headers</span></span>
| <span data-ttu-id="18474-116">Name</span><span class="sxs-lookup"><span data-stu-id="18474-116">Name</span></span>       | <span data-ttu-id="18474-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18474-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="18474-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="18474-118">Authorization</span></span>  | <span data-ttu-id="18474-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18474-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18474-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18474-121">Request body</span></span>
<span data-ttu-id="18474-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="18474-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18474-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="18474-123">Parameter</span></span>    | <span data-ttu-id="18474-124">Typ</span><span class="sxs-lookup"><span data-stu-id="18474-124">Type</span></span>   |<span data-ttu-id="18474-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18474-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18474-126">fields</span><span class="sxs-lookup"><span data-stu-id="18474-126">fields</span></span>|<span data-ttu-id="18474-127">SortField</span><span class="sxs-lookup"><span data-stu-id="18474-127">SortField</span></span>|<span data-ttu-id="18474-128">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="18474-128">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="18474-129">matchCase</span><span class="sxs-lookup"><span data-stu-id="18474-129">matchCase</span></span>|<span data-ttu-id="18474-130">boolean</span><span class="sxs-lookup"><span data-stu-id="18474-130">boolean</span></span>|<span data-ttu-id="18474-p103">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="18474-p103">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="18474-133">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="18474-133">hasHeaders</span></span>|<span data-ttu-id="18474-134">boolean</span><span class="sxs-lookup"><span data-stu-id="18474-134">boolean</span></span>|<span data-ttu-id="18474-p104">Optional. Gibt an, ob der Bereich eine Kopfzeile aufweist.</span><span class="sxs-lookup"><span data-stu-id="18474-p104">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="18474-137">orientation</span><span class="sxs-lookup"><span data-stu-id="18474-137">orientation</span></span>|<span data-ttu-id="18474-138">string</span><span class="sxs-lookup"><span data-stu-id="18474-138">string</span></span>|<span data-ttu-id="18474-p105">Optional. Gibt an, ob der Vorgang Zeilen oder Spalten sortiert.  Die folgenden Werte sind möglich: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="18474-p105">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="18474-142">Methode</span><span class="sxs-lookup"><span data-stu-id="18474-142">method</span></span>|<span data-ttu-id="18474-143">string</span><span class="sxs-lookup"><span data-stu-id="18474-143">string</span></span>|<span data-ttu-id="18474-p106">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="18474-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="18474-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="18474-147">Response</span></span>

<span data-ttu-id="18474-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18474-p107">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18474-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18474-150">Example</span></span>
<span data-ttu-id="18474-151">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="18474-151">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18474-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18474-152">Request</span></span>
<span data-ttu-id="18474-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18474-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="18474-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="18474-154">Response</span></span>
<span data-ttu-id="18474-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18474-155">Here is an example of the response.</span></span> 
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
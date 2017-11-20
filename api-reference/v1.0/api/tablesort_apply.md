# <a name="tablesort-apply"></a><span data-ttu-id="7a4c4-101">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="7a4c4-101">TableSort: apply</span></span>

<span data-ttu-id="7a4c4-102">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a4c4-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7a4c4-103">Permissions</span></span>
<span data-ttu-id="7a4c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a4c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7a4c4-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a4c4-106">Permission type</span></span>      | <span data-ttu-id="7a4c4-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a4c4-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7a4c4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a4c4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7a4c4-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a4c4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a4c4-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a4c4-111">Not supported.</span></span>    |
|<span data-ttu-id="7a4c4-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a4c4-112">Application</span></span> | <span data-ttu-id="7a4c4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a4c4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a4c4-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a4c4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="7a4c4-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a4c4-115">Request headers</span></span>
| <span data-ttu-id="7a4c4-116">Name</span><span class="sxs-lookup"><span data-stu-id="7a4c4-116">Name</span></span>       | <span data-ttu-id="7a4c4-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a4c4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7a4c4-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a4c4-118">Authorization</span></span>  | <span data-ttu-id="7a4c4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a4c4-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7a4c4-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="7a4c4-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a4c4-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a4c4-124">Request body</span></span>
<span data-ttu-id="7a4c4-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7a4c4-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="7a4c4-126">Parameter</span></span>    | <span data-ttu-id="7a4c4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7a4c4-127">Type</span></span>   |<span data-ttu-id="7a4c4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a4c4-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a4c4-129">fields</span><span class="sxs-lookup"><span data-stu-id="7a4c4-129">fields</span></span>|<span data-ttu-id="7a4c4-130">SortField</span><span class="sxs-lookup"><span data-stu-id="7a4c4-130">SortField</span></span>|<span data-ttu-id="7a4c4-131">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-131">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="7a4c4-132">matchCase</span><span class="sxs-lookup"><span data-stu-id="7a4c4-132">matchCase</span></span>|<span data-ttu-id="7a4c4-133">boolean</span><span class="sxs-lookup"><span data-stu-id="7a4c4-133">boolean</span></span>|<span data-ttu-id="7a4c4-p104">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="7a4c4-136">method</span><span class="sxs-lookup"><span data-stu-id="7a4c4-136">method</span></span>|<span data-ttu-id="7a4c4-137">string</span><span class="sxs-lookup"><span data-stu-id="7a4c4-137">string</span></span>|<span data-ttu-id="7a4c4-p105">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="7a4c4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a4c4-141">Response</span></span>

<span data-ttu-id="7a4c4-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a4c4-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a4c4-144">Example</span></span>
<span data-ttu-id="7a4c4-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7a4c4-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a4c4-146">Request</span></span>
<span data-ttu-id="7a4c4-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7a4c4-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a4c4-148">Response</span></span>
<span data-ttu-id="7a4c4-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7a4c4-149">Here is an example of the response.</span></span> 
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
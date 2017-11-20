# <a name="range-merge"></a><span data-ttu-id="b81f3-101">Range: merge</span><span class="sxs-lookup"><span data-stu-id="b81f3-101">Range: merge</span></span>

<span data-ttu-id="b81f3-102">Führt die Zellen des Bereichs in einen Bereich im Arbeitsblatt zusammen.</span><span class="sxs-lookup"><span data-stu-id="b81f3-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="b81f3-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b81f3-103">Permissions</span></span>
<span data-ttu-id="b81f3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b81f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b81f3-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b81f3-106">Permission type</span></span>      | <span data-ttu-id="b81f3-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b81f3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b81f3-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b81f3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b81f3-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b81f3-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b81f3-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b81f3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b81f3-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b81f3-111">Not supported.</span></span>    |
|<span data-ttu-id="b81f3-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b81f3-112">Application</span></span> | <span data-ttu-id="b81f3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b81f3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b81f3-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b81f3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="b81f3-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b81f3-115">Request headers</span></span>
| <span data-ttu-id="b81f3-116">Name</span><span class="sxs-lookup"><span data-stu-id="b81f3-116">Name</span></span>       | <span data-ttu-id="b81f3-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b81f3-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b81f3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="b81f3-118">Authorization</span></span>  | <span data-ttu-id="b81f3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b81f3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b81f3-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b81f3-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="b81f3-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b81f3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b81f3-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b81f3-124">Request body</span></span>
<span data-ttu-id="b81f3-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b81f3-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b81f3-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="b81f3-126">Parameter</span></span>    | <span data-ttu-id="b81f3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b81f3-127">Type</span></span>   |<span data-ttu-id="b81f3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b81f3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b81f3-129">across</span><span class="sxs-lookup"><span data-stu-id="b81f3-129">across</span></span>|<span data-ttu-id="b81f3-130">boolean</span><span class="sxs-lookup"><span data-stu-id="b81f3-130">boolean</span></span>|<span data-ttu-id="b81f3-p104">Optional. Mit „true“ werden Zellen in allen Zeilen des angegebenen Bereichs als einzelne zusammengeführte Zellen zusammengeführt. Der Standardwert lautet „false“.</span><span class="sxs-lookup"><span data-stu-id="b81f3-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="b81f3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b81f3-134">Response</span></span>

<span data-ttu-id="b81f3-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b81f3-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b81f3-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b81f3-137">Example</span></span>
<span data-ttu-id="b81f3-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b81f3-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b81f3-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b81f3-139">Request</span></span>
<span data-ttu-id="b81f3-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b81f3-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="b81f3-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b81f3-141">Response</span></span>
<span data-ttu-id="b81f3-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b81f3-142">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
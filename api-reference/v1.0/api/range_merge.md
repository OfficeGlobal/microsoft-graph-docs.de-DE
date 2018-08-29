# <a name="range-merge"></a><span data-ttu-id="c1f2b-101">Range: merge</span><span class="sxs-lookup"><span data-stu-id="c1f2b-101">Range: merge</span></span>

<span data-ttu-id="c1f2b-102">Führt die Zellen des Bereichs in einen Bereich im Arbeitsblatt zusammen.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1f2b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1f2b-103">Permissions</span></span>
<span data-ttu-id="c1f2b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1f2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1f2b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1f2b-106">Permission type</span></span>      | <span data-ttu-id="c1f2b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1f2b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1f2b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1f2b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c1f2b-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1f2b-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1f2b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1f2b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1f2b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1f2b-111">Not supported.</span></span>    |
|<span data-ttu-id="c1f2b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1f2b-112">Application</span></span> | <span data-ttu-id="c1f2b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1f2b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1f2b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1f2b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="c1f2b-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1f2b-115">Request headers</span></span>
| <span data-ttu-id="c1f2b-116">Name</span><span class="sxs-lookup"><span data-stu-id="c1f2b-116">Name</span></span>       | <span data-ttu-id="c1f2b-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1f2b-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1f2b-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c1f2b-118">Authorization</span></span>  | <span data-ttu-id="c1f2b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1f2b-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c1f2b-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="c1f2b-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1f2b-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1f2b-124">Request body</span></span>
<span data-ttu-id="c1f2b-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1f2b-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="c1f2b-126">Parameter</span></span>    | <span data-ttu-id="c1f2b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c1f2b-127">Type</span></span>   |<span data-ttu-id="c1f2b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1f2b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1f2b-129">across</span><span class="sxs-lookup"><span data-stu-id="c1f2b-129">across</span></span>|<span data-ttu-id="c1f2b-130">boolean</span><span class="sxs-lookup"><span data-stu-id="c1f2b-130">boolean</span></span>|<span data-ttu-id="c1f2b-p104">Optional. Mit „true“ werden Zellen in allen Zeilen des angegebenen Bereichs als einzelne zusammengeführte Zellen zusammengeführt. Der Standardwert lautet „false“.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="c1f2b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1f2b-134">Response</span></span>

<span data-ttu-id="c1f2b-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1f2b-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1f2b-137">Example</span></span>
<span data-ttu-id="c1f2b-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1f2b-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1f2b-139">Request</span></span>
<span data-ttu-id="c1f2b-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="c1f2b-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1f2b-141">Response</span></span>
<span data-ttu-id="c1f2b-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c1f2b-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
# <a name="range-usedrange"></a><span data-ttu-id="8b497-101">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="8b497-101">Range: UsedRange</span></span>

<span data-ttu-id="8b497-102">Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.</span><span class="sxs-lookup"><span data-stu-id="8b497-102">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b497-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b497-103">Permissions</span></span>
<span data-ttu-id="8b497-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b497-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b497-106">Permission type</span></span>      | <span data-ttu-id="8b497-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b497-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b497-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b497-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8b497-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b497-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b497-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b497-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b497-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b497-111">Not supported.</span></span>    |
|<span data-ttu-id="8b497-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b497-112">Application</span></span> | <span data-ttu-id="8b497-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b497-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b497-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b497-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(<address>)/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="8b497-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b497-115">Request headers</span></span>
| <span data-ttu-id="8b497-116">Name</span><span class="sxs-lookup"><span data-stu-id="8b497-116">Name</span></span>       | <span data-ttu-id="8b497-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b497-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b497-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b497-118">Authorization</span></span>  | <span data-ttu-id="8b497-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b497-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b497-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b497-121">Request body</span></span>
<span data-ttu-id="8b497-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8b497-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b497-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="8b497-123">Parameter</span></span>    | <span data-ttu-id="8b497-124">Typ</span><span class="sxs-lookup"><span data-stu-id="8b497-124">Type</span></span>   |<span data-ttu-id="8b497-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b497-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b497-126">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="8b497-126">valuesOnly</span></span>|<span data-ttu-id="8b497-127">boolean</span><span class="sxs-lookup"><span data-stu-id="8b497-127">boolean</span></span>|<span data-ttu-id="8b497-p103">Optional. Betrachtet nur Zellen mit Werten als verwendet.</span><span class="sxs-lookup"><span data-stu-id="8b497-p103">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="8b497-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b497-130">Response</span></span>

<span data-ttu-id="8b497-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b497-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b497-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b497-132">Example</span></span>
<span data-ttu-id="8b497-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8b497-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8b497-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b497-134">Request</span></span>
<span data-ttu-id="8b497-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b497-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="8b497-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b497-136">Response</span></span>
<span data-ttu-id="8b497-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b497-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
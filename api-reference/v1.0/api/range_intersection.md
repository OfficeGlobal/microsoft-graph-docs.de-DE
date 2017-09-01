# <a name="range-intersection"></a><span data-ttu-id="02c94-101">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="02c94-101">Range: Intersection</span></span>

<span data-ttu-id="02c94-102">Ruft das Bereichsobjekt ab, das die rechteckige Schnittmenge der angegebenen Bereiche darstellt.</span><span class="sxs-lookup"><span data-stu-id="02c94-102">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="02c94-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="02c94-103">Permissions</span></span>
<span data-ttu-id="02c94-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="02c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="02c94-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02c94-106">Permission type</span></span>      | <span data-ttu-id="02c94-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02c94-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02c94-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02c94-108">Delegated (work or school account)</span></span> | <span data-ttu-id="02c94-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02c94-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="02c94-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02c94-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02c94-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02c94-111">Not supported.</span></span>    |
|<span data-ttu-id="02c94-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02c94-112">Application</span></span> | <span data-ttu-id="02c94-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02c94-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02c94-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02c94-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(<address>)/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="02c94-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02c94-115">Request headers</span></span>
| <span data-ttu-id="02c94-116">Name</span><span class="sxs-lookup"><span data-stu-id="02c94-116">Name</span></span>       | <span data-ttu-id="02c94-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02c94-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="02c94-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="02c94-118">Authorization</span></span>  | <span data-ttu-id="02c94-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02c94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02c94-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02c94-121">Request body</span></span>
<span data-ttu-id="02c94-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="02c94-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="02c94-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="02c94-123">Parameter</span></span>    | <span data-ttu-id="02c94-124">Typ</span><span class="sxs-lookup"><span data-stu-id="02c94-124">Type</span></span>   |<span data-ttu-id="02c94-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02c94-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02c94-126">anotherRange</span><span class="sxs-lookup"><span data-stu-id="02c94-126">anotherRange</span></span>|<span data-ttu-id="02c94-127">string</span><span class="sxs-lookup"><span data-stu-id="02c94-127">string</span></span>|<span data-ttu-id="02c94-128">Das Bereichsobjekt oder die Bereichsadresse, die verwendet wird, um die Schnittmenge der Bereiche zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="02c94-128">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="02c94-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="02c94-129">Response</span></span>

<span data-ttu-id="02c94-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02c94-130">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02c94-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02c94-131">Example</span></span>
<span data-ttu-id="02c94-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="02c94-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="02c94-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02c94-133">Request</span></span>
<span data-ttu-id="02c94-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02c94-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="02c94-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="02c94-135">Response</span></span>
<span data-ttu-id="02c94-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02c94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
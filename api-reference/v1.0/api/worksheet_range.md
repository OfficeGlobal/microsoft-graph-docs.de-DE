# <a name="worksheet-range"></a><span data-ttu-id="999bd-101">Arbeitsblatt: Range</span><span class="sxs-lookup"><span data-stu-id="999bd-101">Worksheet: Range</span></span>

<span data-ttu-id="999bd-102">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="999bd-102">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="999bd-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="999bd-103">Permissions</span></span>
<span data-ttu-id="999bd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="999bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="999bd-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="999bd-106">Permission type</span></span>      | <span data-ttu-id="999bd-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="999bd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="999bd-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="999bd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="999bd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="999bd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="999bd-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="999bd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="999bd-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="999bd-111">Not supported.</span></span>    |
|<span data-ttu-id="999bd-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="999bd-112">Application</span></span> | <span data-ttu-id="999bd-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="999bd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="999bd-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="999bd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="999bd-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="999bd-115">Request headers</span></span>
| <span data-ttu-id="999bd-116">Name</span><span class="sxs-lookup"><span data-stu-id="999bd-116">Name</span></span>       | <span data-ttu-id="999bd-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="999bd-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="999bd-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="999bd-118">Authorization</span></span>  | <span data-ttu-id="999bd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="999bd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="999bd-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="999bd-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="999bd-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="999bd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="999bd-124">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="999bd-124">Function parameters</span></span>

| <span data-ttu-id="999bd-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="999bd-125">Parameter</span></span>    | <span data-ttu-id="999bd-126">Typ</span><span class="sxs-lookup"><span data-stu-id="999bd-126">Type</span></span>   |<span data-ttu-id="999bd-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="999bd-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="999bd-128">Adresse</span><span class="sxs-lookup"><span data-stu-id="999bd-128">address</span></span>|<span data-ttu-id="999bd-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="999bd-129">string</span></span>|<span data-ttu-id="999bd-p104">Optional. Die Adresse oder der Name des Bereichs. Wenn nichts angegeben ist, wird der gesamte Arbeitsblattbereich zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="999bd-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="999bd-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="999bd-133">Response</span></span>

<span data-ttu-id="999bd-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="999bd-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="999bd-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="999bd-135">Example</span></span>
<span data-ttu-id="999bd-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="999bd-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="999bd-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="999bd-137">Request</span></span>
<span data-ttu-id="999bd-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="999bd-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="999bd-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="999bd-139">Response</span></span>
<span data-ttu-id="999bd-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="999bd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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

<span data-ttu-id="999bd-143">Wenn die optionalen `address` Parameter nicht angegeben ist, diese Funktion gibt den gesamte Arbeitsblattbereich zurück.</span><span class="sxs-lookup"><span data-stu-id="999bd-143">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="999bd-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="999bd-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="999bd-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="999bd-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
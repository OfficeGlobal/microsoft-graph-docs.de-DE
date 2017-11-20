# <a name="worksheet-range"></a><span data-ttu-id="72232-101">Arbeitsblatt: Range</span><span class="sxs-lookup"><span data-stu-id="72232-101">Worksheet: Range</span></span>

<span data-ttu-id="72232-102">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="72232-102">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="72232-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="72232-103">Permissions</span></span>
<span data-ttu-id="72232-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="72232-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="72232-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="72232-106">Permission type</span></span>      | <span data-ttu-id="72232-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="72232-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72232-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="72232-108">Delegated (work or school account)</span></span> | <span data-ttu-id="72232-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72232-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="72232-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="72232-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72232-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72232-111">Not supported.</span></span>    |
|<span data-ttu-id="72232-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="72232-112">Application</span></span> | <span data-ttu-id="72232-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72232-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72232-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="72232-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="72232-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="72232-115">Request headers</span></span>
| <span data-ttu-id="72232-116">Name</span><span class="sxs-lookup"><span data-stu-id="72232-116">Name</span></span>       | <span data-ttu-id="72232-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72232-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72232-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="72232-118">Authorization</span></span>  | <span data-ttu-id="72232-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="72232-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72232-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="72232-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="72232-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="72232-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72232-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="72232-124">Request body</span></span>
<span data-ttu-id="72232-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="72232-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="72232-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="72232-126">Parameter</span></span>    | <span data-ttu-id="72232-127">Typ</span><span class="sxs-lookup"><span data-stu-id="72232-127">Type</span></span>   |<span data-ttu-id="72232-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72232-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72232-129">address</span><span class="sxs-lookup"><span data-stu-id="72232-129">address</span></span>|<span data-ttu-id="72232-130">string</span><span class="sxs-lookup"><span data-stu-id="72232-130">string</span></span>|<span data-ttu-id="72232-p104">Optional. Die Adresse oder der Name des Bereichs. Wenn nichts angegeben ist, wird der gesamte Arbeitsblattbereich zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="72232-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="72232-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="72232-134">Response</span></span>

<span data-ttu-id="72232-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="72232-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72232-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="72232-136">Example</span></span>
<span data-ttu-id="72232-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="72232-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="72232-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="72232-138">Request</span></span>
<span data-ttu-id="72232-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="72232-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="72232-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="72232-140">Response</span></span>
<span data-ttu-id="72232-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="72232-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
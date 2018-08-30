# <a name="worksheet-usedrange"></a><span data-ttu-id="aa3f6-101">Arbeitsblatt: UsedRange</span><span class="sxs-lookup"><span data-stu-id="aa3f6-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="aa3f6-p101">Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa3f6-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa3f6-104">Permissions</span></span>
<span data-ttu-id="aa3f6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa3f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa3f6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa3f6-107">Permission type</span></span>      | <span data-ttu-id="aa3f6-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa3f6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa3f6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa3f6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="aa3f6-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa3f6-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa3f6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa3f6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa3f6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa3f6-112">Not supported.</span></span>    |
|<span data-ttu-id="aa3f6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa3f6-113">Application</span></span> | <span data-ttu-id="aa3f6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa3f6-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa3f6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa3f6-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="parameters"></a><span data-ttu-id="aa3f6-116">Parameter</span><span class="sxs-lookup"><span data-stu-id="aa3f6-116">Parameters</span></span>
<span data-ttu-id="aa3f6-117">In der Anforderungs-URL können Sie optionale Parameter angeben.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-117">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="aa3f6-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="aa3f6-118">Parameter</span></span>    | <span data-ttu-id="aa3f6-119">Typ</span><span class="sxs-lookup"><span data-stu-id="aa3f6-119">Type</span></span>   |<span data-ttu-id="aa3f6-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa3f6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa3f6-121">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="aa3f6-121">valuesOnly</span></span>|<span data-ttu-id="aa3f6-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="aa3f6-122">Boolean</span></span>|<span data-ttu-id="aa3f6-p103">Optional. Betrachtet nur Zellen mit Werten als verwendet (ignoriert die Formatierung).</span><span class="sxs-lookup"><span data-stu-id="aa3f6-p103">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="aa3f6-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa3f6-125">Request headers</span></span>
| <span data-ttu-id="aa3f6-126">Name</span><span class="sxs-lookup"><span data-stu-id="aa3f6-126">Name</span></span>       | <span data-ttu-id="aa3f6-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa3f6-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa3f6-128">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="aa3f6-128">Authorization</span></span>  | <span data-ttu-id="aa3f6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa3f6-131">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="aa3f6-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa3f6-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="aa3f6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa3f6-134">Response</span></span>

<span data-ttu-id="aa3f6-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa3f6-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa3f6-136">Example</span></span>
<span data-ttu-id="aa3f6-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-137">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="aa3f6-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa3f6-138">Request</span></span>
<span data-ttu-id="aa3f6-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="aa3f6-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa3f6-140">Response</span></span>
<span data-ttu-id="aa3f6-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="aa3f6-144">Alternativ kann diese Funktion mit dem optionalen `valuesOnly` Parameter aufgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-144">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="aa3f6-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa3f6-145">Request</span></span>
<span data-ttu-id="aa3f6-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-146">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="aa3f6-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa3f6-147">Response</span></span>
<span data-ttu-id="aa3f6-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa3f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
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

# <a name="rangebordercollection-itemat"></a><span data-ttu-id="11553-101">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="11553-101">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="11553-102">Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.</span><span class="sxs-lookup"><span data-stu-id="11553-102">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="11553-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="11553-103">Permissions</span></span>
<span data-ttu-id="11553-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="11553-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="11553-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11553-106">Permission type</span></span>      | <span data-ttu-id="11553-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11553-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11553-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11553-108">Delegated (work or school account)</span></span> | <span data-ttu-id="11553-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11553-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11553-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11553-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11553-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11553-111">Not supported.</span></span>    |
|<span data-ttu-id="11553-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11553-112">Application</span></span> | <span data-ttu-id="11553-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11553-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11553-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11553-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="11553-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11553-115">Request headers</span></span>
| <span data-ttu-id="11553-116">Name</span><span class="sxs-lookup"><span data-stu-id="11553-116">Name</span></span>       | <span data-ttu-id="11553-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11553-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11553-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="11553-118">Authorization</span></span>  | <span data-ttu-id="11553-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11553-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11553-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="11553-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="11553-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="11553-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11553-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11553-124">Request body</span></span>
<span data-ttu-id="11553-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="11553-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11553-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="11553-126">Parameter</span></span>    | <span data-ttu-id="11553-127">Typ</span><span class="sxs-lookup"><span data-stu-id="11553-127">Type</span></span>   |<span data-ttu-id="11553-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11553-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11553-129">Index</span><span class="sxs-lookup"><span data-stu-id="11553-129">index</span></span>|<span data-ttu-id="11553-130">Int32</span><span class="sxs-lookup"><span data-stu-id="11553-130">Int32</span></span>|<span data-ttu-id="11553-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="11553-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="11553-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="11553-133">Response</span></span>

<span data-ttu-id="11553-134">Wenn diese Methode erfolgreich verläuft, gibt diese im Antworttext einen Antwortcode `200 OK` und das [WorkbookRangeBorder](../resources/rangeborder.md)-Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="11553-134">If successful, this method returns `200 OK` response code and [groupSetting](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11553-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11553-135">Example</span></span>
<span data-ttu-id="11553-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="11553-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="11553-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11553-137">Request</span></span>
<span data-ttu-id="11553-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11553-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "rangebordercollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 1
}
```

##### <a name="response"></a><span data-ttu-id="11553-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="11553-139">Response</span></span>
<span data-ttu-id="11553-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11553-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
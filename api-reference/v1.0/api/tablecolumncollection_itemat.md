# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="97a63-101">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="97a63-101">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="97a63-102">Ruft eine Spalte anhand ihrer Position in der Auflistung ab.</span><span class="sxs-lookup"><span data-stu-id="97a63-102">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="97a63-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97a63-103">Permissions</span></span>
<span data-ttu-id="97a63-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97a63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97a63-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97a63-106">Permission type</span></span>      | <span data-ttu-id="97a63-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97a63-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97a63-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97a63-108">Delegated (work or school account)</span></span> | <span data-ttu-id="97a63-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97a63-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="97a63-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97a63-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97a63-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97a63-111">Not supported.</span></span>    |
|<span data-ttu-id="97a63-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97a63-112">Application</span></span> | <span data-ttu-id="97a63-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97a63-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97a63-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a63-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="97a63-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97a63-115">Request headers</span></span>
| <span data-ttu-id="97a63-116">Name</span><span class="sxs-lookup"><span data-stu-id="97a63-116">Name</span></span>       | <span data-ttu-id="97a63-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97a63-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97a63-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="97a63-118">Authorization</span></span>  | <span data-ttu-id="97a63-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97a63-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97a63-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="97a63-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="97a63-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="97a63-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97a63-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97a63-124">Request body</span></span>
<span data-ttu-id="97a63-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="97a63-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="97a63-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="97a63-126">Parameter</span></span>    | <span data-ttu-id="97a63-127">Typ</span><span class="sxs-lookup"><span data-stu-id="97a63-127">Type</span></span>   |<span data-ttu-id="97a63-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97a63-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97a63-129">Index</span><span class="sxs-lookup"><span data-stu-id="97a63-129">index</span></span>|<span data-ttu-id="97a63-130">Int32</span><span class="sxs-lookup"><span data-stu-id="97a63-130">Int32</span></span>|<span data-ttu-id="97a63-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="97a63-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="97a63-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a63-133">Response</span></span>

<span data-ttu-id="97a63-134">Wenn erfolgreich, gibt dieses Verfahren einen `200 OK` Antwortcode und ein[WorkbookTableColumn](../resources/tablecolumn.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="97a63-134">If successful, this method returns `200 OK` response code and [groupSetting](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97a63-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97a63-135">Example</span></span>
<span data-ttu-id="97a63-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="97a63-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="97a63-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97a63-137">Request</span></span>
<span data-ttu-id="97a63-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97a63-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumncollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 3
}
```

##### <a name="response"></a><span data-ttu-id="97a63-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="97a63-139">Response</span></span>
<span data-ttu-id="97a63-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97a63-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
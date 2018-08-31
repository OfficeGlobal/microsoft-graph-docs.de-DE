# <a name="tablecolumncollection-add"></a><span data-ttu-id="74231-101">TableColumnCollection: hinzufügen</span><span class="sxs-lookup"><span data-stu-id="74231-101">TableColumnCollection: add</span></span>

<span data-ttu-id="74231-102">Fügt der Tabelle eine neue Spalte hinzu.</span><span class="sxs-lookup"><span data-stu-id="74231-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="74231-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="74231-103">Permissions</span></span>
<span data-ttu-id="74231-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="74231-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="74231-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74231-106">Permission type</span></span>      | <span data-ttu-id="74231-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74231-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74231-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74231-108">Delegated (work or school account)</span></span> | <span data-ttu-id="74231-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74231-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74231-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74231-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74231-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74231-111">Not supported.</span></span>    |
|<span data-ttu-id="74231-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74231-112">Application</span></span> | <span data-ttu-id="74231-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74231-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74231-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74231-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="74231-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74231-115">Request headers</span></span>
| <span data-ttu-id="74231-116">Name</span><span class="sxs-lookup"><span data-stu-id="74231-116">Name</span></span>       | <span data-ttu-id="74231-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74231-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74231-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="74231-118">Authorization</span></span>  | <span data-ttu-id="74231-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74231-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74231-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="74231-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="74231-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="74231-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74231-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74231-124">Request body</span></span>
<span data-ttu-id="74231-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="74231-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74231-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="74231-126">Parameter</span></span>    | <span data-ttu-id="74231-127">Typ</span><span class="sxs-lookup"><span data-stu-id="74231-127">Type</span></span>   |<span data-ttu-id="74231-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74231-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74231-129">Index</span><span class="sxs-lookup"><span data-stu-id="74231-129">index</span></span>|<span data-ttu-id="74231-130">Int32</span><span class="sxs-lookup"><span data-stu-id="74231-130">Int32</span></span>|<span data-ttu-id="74231-p104">Gibt die relative Position der neuen Spalte an. Die vorherige Spalte an dieser Position wird nach rechts verschoben. Der Indexwert sollte gleich oder kleiner als der letzten Spalten-Indexwert sein, damit er nicht dazu verwendet werden kann, eine Spalte an das Ende der Tabelle anzuhängen. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="74231-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="74231-135">Werte</span><span class="sxs-lookup"><span data-stu-id="74231-135">values</span></span>|<span data-ttu-id="74231-136">Json</span><span class="sxs-lookup"><span data-stu-id="74231-136">Json</span></span>|<span data-ttu-id="74231-p105">Optional. Ein 2-dimensionales Array von unformatierten Werten der Tabellenspalte.</span><span class="sxs-lookup"><span data-stu-id="74231-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="74231-139">Name</span><span class="sxs-lookup"><span data-stu-id="74231-139">name</span></span>|<span data-ttu-id="74231-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74231-140">string</span></span>|<span data-ttu-id="74231-141">Name</span><span class="sxs-lookup"><span data-stu-id="74231-141">name</span></span>
## <a name="response"></a><span data-ttu-id="74231-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="74231-142">Response</span></span>

<span data-ttu-id="74231-143">Wenn erfolgreich, gibt dieses Verfahren im Antworttext einen `200 OK` Antwortcode und ein[WorkbookTableColumn](../resources/tablecolumn.md)-Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="74231-143">If successful, this method returns `200 OK` response code and [groupSetting](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74231-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74231-144">Example</span></span>
<span data-ttu-id="74231-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="74231-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74231-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74231-146">Request</span></span>
<span data-ttu-id="74231-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74231-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": 3,
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="74231-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="74231-148">Response</span></span>
<span data-ttu-id="74231-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74231-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablecolumncollection_add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection_add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
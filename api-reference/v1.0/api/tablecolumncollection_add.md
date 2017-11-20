# <a name="tablecolumncollection-add"></a><span data-ttu-id="6aaac-101">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="6aaac-101">TableColumnCollection: add</span></span>

<span data-ttu-id="6aaac-102">Fügt der Tabelle eine neue Spalte hinzu.</span><span class="sxs-lookup"><span data-stu-id="6aaac-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="6aaac-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6aaac-103">Permissions</span></span>
<span data-ttu-id="6aaac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6aaac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6aaac-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6aaac-106">Permission type</span></span>      | <span data-ttu-id="6aaac-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6aaac-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6aaac-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6aaac-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6aaac-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6aaac-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6aaac-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6aaac-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aaac-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6aaac-111">Not supported.</span></span>    |
|<span data-ttu-id="6aaac-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6aaac-112">Application</span></span> | <span data-ttu-id="6aaac-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6aaac-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aaac-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6aaac-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="6aaac-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6aaac-115">Request headers</span></span>
| <span data-ttu-id="6aaac-116">Name</span><span class="sxs-lookup"><span data-stu-id="6aaac-116">Name</span></span>       | <span data-ttu-id="6aaac-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6aaac-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6aaac-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aaac-118">Authorization</span></span>  | <span data-ttu-id="6aaac-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6aaac-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6aaac-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="6aaac-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="6aaac-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="6aaac-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aaac-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6aaac-124">Request body</span></span>
<span data-ttu-id="6aaac-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6aaac-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6aaac-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="6aaac-126">Parameter</span></span>    | <span data-ttu-id="6aaac-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6aaac-127">Type</span></span>   |<span data-ttu-id="6aaac-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6aaac-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6aaac-129">Index</span><span class="sxs-lookup"><span data-stu-id="6aaac-129">index</span></span>|<span data-ttu-id="6aaac-130">number</span><span class="sxs-lookup"><span data-stu-id="6aaac-130">number</span></span>|<span data-ttu-id="6aaac-p104">Gibt die relative Position der neuen Spalte an. Die vorherige Spalte an dieser Position wird nach rechts verschoben. Der Indexwert sollte gleich oder kleiner als der letzten Spalten-Indexwert sein, damit er nicht dazu verwendet werden kann, eine Spalte an das Ende der Tabelle anzuhängen. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="6aaac-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="6aaac-135">values</span><span class="sxs-lookup"><span data-stu-id="6aaac-135">values</span></span>|<span data-ttu-id="6aaac-136">(boolean or string or number)</span><span class="sxs-lookup"><span data-stu-id="6aaac-136">(boolean or string or number)</span></span>|<span data-ttu-id="6aaac-p105">Optional. Ein 2-dimensionales Array von unformatierten Werten der Tabellenspalte.</span><span class="sxs-lookup"><span data-stu-id="6aaac-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="6aaac-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6aaac-139">Response</span></span>

<span data-ttu-id="6aaac-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableColumn](../resources/tablecolumn.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6aaac-140">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aaac-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6aaac-141">Example</span></span>
<span data-ttu-id="6aaac-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6aaac-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6aaac-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6aaac-143">Request</span></span>
<span data-ttu-id="6aaac-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6aaac-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="6aaac-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="6aaac-145">Response</span></span>
<span data-ttu-id="6aaac-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6aaac-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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
  "tocPath": ""
}-->
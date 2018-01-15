# <a name="tablerowcollection-add"></a><span data-ttu-id="c8604-101">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="c8604-101">TableRowCollection: add</span></span>

<span data-ttu-id="c8604-102">Fügt der Tabelle eine neue Zeile hinzu.</span><span class="sxs-lookup"><span data-stu-id="c8604-102">Adds a new row to the table.</span></span>

## <a name="error-handling"></a><span data-ttu-id="c8604-103">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="c8604-103">Error Handling</span></span>

<span data-ttu-id="c8604-104">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="c8604-104">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="c8604-105">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8604-105">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8604-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8604-106">Permissions</span></span>
<span data-ttu-id="c8604-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8604-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c8604-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8604-109">Permission type</span></span>      | <span data-ttu-id="c8604-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8604-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8604-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8604-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c8604-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8604-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8604-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8604-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8604-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8604-114">Not supported.</span></span>    |
|<span data-ttu-id="c8604-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8604-115">Application</span></span> | <span data-ttu-id="c8604-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8604-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8604-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8604-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="c8604-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8604-118">Request headers</span></span>
| <span data-ttu-id="c8604-119">Name</span><span class="sxs-lookup"><span data-stu-id="c8604-119">Name</span></span>       | <span data-ttu-id="c8604-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8604-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8604-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8604-121">Authorization</span></span>  | <span data-ttu-id="c8604-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8604-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8604-124">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c8604-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8604-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c8604-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8604-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8604-127">Request body</span></span>
<span data-ttu-id="c8604-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c8604-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8604-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="c8604-129">Parameter</span></span>    | <span data-ttu-id="c8604-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c8604-130">Type</span></span>   |<span data-ttu-id="c8604-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8604-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8604-132">Index</span><span class="sxs-lookup"><span data-stu-id="c8604-132">index</span></span>|<span data-ttu-id="c8604-133">number</span><span class="sxs-lookup"><span data-stu-id="c8604-133">number</span></span>|<span data-ttu-id="c8604-p105">Optional. Gibt die relative Position der neuen Zeile an. Bei Null erfolgt die Erweiterung am Ende. Alle Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="c8604-p105">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="c8604-139">values</span><span class="sxs-lookup"><span data-stu-id="c8604-139">values</span></span>|<span data-ttu-id="c8604-140">(boolean or string or number)</span><span class="sxs-lookup"><span data-stu-id="c8604-140">(boolean or string or number)</span></span>|<span data-ttu-id="c8604-p106">Optional. Ein 2-dimensionales Array von unformatierten Werten der Tabellenzeile.</span><span class="sxs-lookup"><span data-stu-id="c8604-p106">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="c8604-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8604-143">Response</span></span>

<span data-ttu-id="c8604-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8604-144">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8604-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8604-145">Example</span></span>
<span data-ttu-id="c8604-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c8604-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8604-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8604-147">Request</span></span>
<span data-ttu-id="c8604-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8604-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="c8604-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8604-149">Response</span></span>
<span data-ttu-id="c8604-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8604-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

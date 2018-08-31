# <a name="create-tablerow"></a><span data-ttu-id="38847-101">TableRow erstellen</span><span class="sxs-lookup"><span data-stu-id="38847-101">Create TableRow</span></span>

<span data-ttu-id="38847-102">Fügt Zeilen an das Ende der Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="38847-102">Adds a row to the end of the table.</span></span> <span data-ttu-id="38847-103">Beachten Sie, dass die API mehrere Zeilen von Daten mit dieser API akzeptieren kann.</span><span class="sxs-lookup"><span data-stu-id="38847-103">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="38847-104">Hinzufügen von jeweils einer Zeile zur Zeit kann zu Leistungsbeeinträchtigungen führen.</span><span class="sxs-lookup"><span data-stu-id="38847-104">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="38847-105">Die empfohlene Vorgehensweise wäre die Zeilen in einem einzigen Aufruf zu batchen anstatt einzelne Zeilen einzufügen.</span><span class="sxs-lookup"><span data-stu-id="38847-105">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="38847-106">Um optimale Ergebnisse zu erhalten, sammeln Sie die Zeilen, die auf der Anwendungsseite eingefügt werden sollen, und führen Sie den Vorgang zum Hinzufügen von einzelnen Zeilen aus.</span><span class="sxs-lookup"><span data-stu-id="38847-106">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="38847-107">Experimentieren Sie mit der Anzahl der Zeilen, um die ideale Anzahl der Zeilen zu bestimmen, die in einem einzelnen API-Aufruf verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="38847-107">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="38847-108">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="38847-108">Error Handling</span></span>

<span data-ttu-id="38847-109">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="38847-109">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="38847-110">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38847-110">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="38847-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38847-111">Permissions</span></span>
<span data-ttu-id="38847-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38847-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="38847-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38847-114">Permission type</span></span>      | <span data-ttu-id="38847-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38847-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38847-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38847-116">Delegated (work or school account)</span></span> | <span data-ttu-id="38847-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38847-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="38847-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38847-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38847-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38847-119">Not supported.</span></span>    |
|<span data-ttu-id="38847-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38847-120">Application</span></span> | <span data-ttu-id="38847-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38847-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38847-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38847-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="38847-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38847-123">Request headers</span></span>
| <span data-ttu-id="38847-124">Name</span><span class="sxs-lookup"><span data-stu-id="38847-124">Name</span></span>       | <span data-ttu-id="38847-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38847-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="38847-126">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="38847-126">Authorization</span></span>  | <span data-ttu-id="38847-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38847-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38847-129">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="38847-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="38847-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="38847-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38847-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38847-132">Request body</span></span>
<span data-ttu-id="38847-133">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="38847-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="38847-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="38847-134">Parameter</span></span>    | <span data-ttu-id="38847-135">Typ</span><span class="sxs-lookup"><span data-stu-id="38847-135">Type</span></span>   |<span data-ttu-id="38847-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38847-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38847-137">Index</span><span class="sxs-lookup"><span data-stu-id="38847-137">index</span></span>|<span data-ttu-id="38847-138">number</span><span class="sxs-lookup"><span data-stu-id="38847-138">number</span></span>|<span data-ttu-id="38847-p106">Optional. Gibt die relative Position der neuen Zeile an. Bei Null erfolgt die Erweiterung am Ende. Alle Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="38847-p106">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="38847-144">values</span><span class="sxs-lookup"><span data-stu-id="38847-144">values</span></span>|<span data-ttu-id="38847-145">Json</span><span class="sxs-lookup"><span data-stu-id="38847-145">Json</span></span>|<span data-ttu-id="38847-146">Ein 2-dimensionales Array der unformatierten Werte der Tabellenzeilen (boolescher Wert oder Zeichenfolge oder Zahl).</span><span class="sxs-lookup"><span data-stu-id="38847-146">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="38847-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="38847-147">Response</span></span>

<span data-ttu-id="38847-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38847-148">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38847-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38847-149">Example</span></span>
<span data-ttu-id="38847-150">In diesem Beispiel werden zwei Zeilen mit Daten an das Ende der Tabelle eingefügt.</span><span class="sxs-lookup"><span data-stu-id="38847-150">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="38847-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38847-151">Request</span></span>
<span data-ttu-id="38847-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38847-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
##### <a name="response"></a><span data-ttu-id="38847-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="38847-153">Response</span></span>
<span data-ttu-id="38847-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38847-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
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
  "suppressions": [
    "Error: /api-reference/v1.0/api/table_post_rows.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Warning: /api-reference/v1.0/api/table_post_rows.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)"
  ],
  "tocPath": ""
}-->

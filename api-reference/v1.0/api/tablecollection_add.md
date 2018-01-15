# <a name="tablecollection-add"></a><span data-ttu-id="18b44-101">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="18b44-101">TableCollection: add</span></span>

<span data-ttu-id="18b44-p101">Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="18b44-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="18b44-105">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="18b44-105">Error Handling</span></span>

<span data-ttu-id="18b44-106">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="18b44-106">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="18b44-107">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18b44-107">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="18b44-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18b44-108">Permissions</span></span>
<span data-ttu-id="18b44-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="18b44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18b44-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18b44-111">Permission type</span></span>      | <span data-ttu-id="18b44-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18b44-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18b44-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18b44-113">Delegated (work or school account)</span></span> | <span data-ttu-id="18b44-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18b44-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="18b44-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18b44-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18b44-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18b44-116">Not supported.</span></span>    |
|<span data-ttu-id="18b44-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18b44-117">Application</span></span> | <span data-ttu-id="18b44-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18b44-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18b44-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18b44-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="18b44-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18b44-120">Request headers</span></span>
| <span data-ttu-id="18b44-121">Name</span><span class="sxs-lookup"><span data-stu-id="18b44-121">Name</span></span>       | <span data-ttu-id="18b44-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18b44-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="18b44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b44-123">Authorization</span></span>  | <span data-ttu-id="18b44-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18b44-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18b44-126">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="18b44-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="18b44-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="18b44-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18b44-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18b44-129">Request body</span></span>
<span data-ttu-id="18b44-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="18b44-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18b44-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="18b44-131">Parameter</span></span>    | <span data-ttu-id="18b44-132">Typ</span><span class="sxs-lookup"><span data-stu-id="18b44-132">Type</span></span>   |<span data-ttu-id="18b44-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18b44-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18b44-134">address</span><span class="sxs-lookup"><span data-stu-id="18b44-134">address</span></span>|<span data-ttu-id="18b44-135">string</span><span class="sxs-lookup"><span data-stu-id="18b44-135">string</span></span>|<span data-ttu-id="18b44-p106">Adresse oder der Name des Bereichobjekts, das die Datenquelle darstellt. Wenn die Adresse keinen Arbeitsblattnamen enthält, wird das aktuell aktive Blatt verwendet.</span><span class="sxs-lookup"><span data-stu-id="18b44-p106">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="18b44-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="18b44-138">hasHeaders</span></span>|<span data-ttu-id="18b44-139">boolean</span><span class="sxs-lookup"><span data-stu-id="18b44-139">boolean</span></span>|<span data-ttu-id="18b44-p107">Boolescher Wert, der angibt, ob die importierten Daten Spaltenüberschriften besitzen. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf falsch festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="18b44-p107">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="18b44-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="18b44-143">Response</span></span>

<span data-ttu-id="18b44-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18b44-144">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b44-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18b44-145">Example</span></span>
<span data-ttu-id="18b44-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="18b44-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18b44-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18b44-147">Request</span></span>
<span data-ttu-id="18b44-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18b44-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="18b44-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="18b44-149">Response</span></span>
<span data-ttu-id="18b44-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18b44-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

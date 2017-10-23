# <a name="tablecollection-add"></a><span data-ttu-id="2b252-101">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="2b252-101">TableCollection: add</span></span>

<span data-ttu-id="2b252-p101">Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="2b252-p101">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b252-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b252-105">Permissions</span></span>
<span data-ttu-id="2b252-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b252-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2b252-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b252-108">Permission type</span></span>      | <span data-ttu-id="2b252-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b252-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b252-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b252-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b252-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b252-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2b252-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b252-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b252-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b252-113">Not supported.</span></span>    |
|<span data-ttu-id="2b252-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b252-114">Application</span></span> | <span data-ttu-id="2b252-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b252-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b252-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b252-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="2b252-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b252-117">Request headers</span></span>
| <span data-ttu-id="2b252-118">Name</span><span class="sxs-lookup"><span data-stu-id="2b252-118">Name</span></span>       | <span data-ttu-id="2b252-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b252-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2b252-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b252-120">Authorization</span></span>  | <span data-ttu-id="2b252-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b252-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b252-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b252-123">Request body</span></span>
<span data-ttu-id="2b252-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2b252-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2b252-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="2b252-125">Parameter</span></span>    | <span data-ttu-id="2b252-126">Typ</span><span class="sxs-lookup"><span data-stu-id="2b252-126">Type</span></span>   |<span data-ttu-id="2b252-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b252-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b252-128">address</span><span class="sxs-lookup"><span data-stu-id="2b252-128">address</span></span>|<span data-ttu-id="2b252-129">string</span><span class="sxs-lookup"><span data-stu-id="2b252-129">string</span></span>|<span data-ttu-id="2b252-p104">Adresse oder der Name des Bereichobjekts, das die Datenquelle darstellt. Wenn die Adresse keinen Arbeitsblattnamen enthält, wird das aktuell aktive Blatt verwendet.</span><span class="sxs-lookup"><span data-stu-id="2b252-p104">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="2b252-132">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="2b252-132">hasHeaders</span></span>|<span data-ttu-id="2b252-133">boolean</span><span class="sxs-lookup"><span data-stu-id="2b252-133">boolean</span></span>|<span data-ttu-id="2b252-p105">Boolescher Wert, der angibt, ob die importierten Daten Spaltenüberschriften besitzen. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf falsch festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="2b252-p105">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="2b252-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b252-137">Response</span></span>

<span data-ttu-id="2b252-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b252-138">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b252-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b252-139">Example</span></span>
<span data-ttu-id="2b252-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2b252-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2b252-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b252-141">Request</span></span>
<span data-ttu-id="2b252-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b252-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2b252-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b252-143">Response</span></span>
<span data-ttu-id="2b252-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b252-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

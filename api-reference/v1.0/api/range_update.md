# <a name="update-range"></a><span data-ttu-id="23845-101">range aktualisieren</span><span class="sxs-lookup"><span data-stu-id="23845-101">Update range</span></span>

<span data-ttu-id="23845-102">Dient zum Aktualisieren der Eigenschaften des Bereichsobjekts.</span><span class="sxs-lookup"><span data-stu-id="23845-102">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="23845-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="23845-103">Permissions</span></span>
<span data-ttu-id="23845-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="23845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23845-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23845-106">Permission type</span></span>      | <span data-ttu-id="23845-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23845-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23845-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23845-108">Delegated (work or school account)</span></span> | <span data-ttu-id="23845-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23845-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23845-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23845-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23845-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23845-111">Not supported.</span></span>    |
|<span data-ttu-id="23845-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23845-112">Application</span></span> | <span data-ttu-id="23845-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23845-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23845-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23845-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="23845-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23845-115">Optional request headers</span></span>
| <span data-ttu-id="23845-116">Name</span><span class="sxs-lookup"><span data-stu-id="23845-116">Name</span></span>       | <span data-ttu-id="23845-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23845-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="23845-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="23845-118">Authorization</span></span>  | <span data-ttu-id="23845-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23845-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23845-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="23845-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="23845-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="23845-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23845-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23845-124">Request body</span></span>
<span data-ttu-id="23845-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="23845-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="23845-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23845-128">Property</span></span>     | <span data-ttu-id="23845-129">Typ</span><span class="sxs-lookup"><span data-stu-id="23845-129">Type</span></span>   |<span data-ttu-id="23845-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23845-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23845-131">columnHidden</span><span class="sxs-lookup"><span data-stu-id="23845-131">columnHidden</span></span>|<span data-ttu-id="23845-132">boolean</span><span class="sxs-lookup"><span data-stu-id="23845-132">boolean</span></span>|<span data-ttu-id="23845-133">Stellt dar, ob alle Spalten des aktuellen Bereichs ausgeblendet sind.</span><span class="sxs-lookup"><span data-stu-id="23845-133">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="23845-134">formulas</span><span class="sxs-lookup"><span data-stu-id="23845-134">formulas</span></span>|<span data-ttu-id="23845-135">json</span><span class="sxs-lookup"><span data-stu-id="23845-135">json</span></span>|<span data-ttu-id="23845-136">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="23845-136">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="23845-137">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="23845-137">formulasLocal</span></span>|<span data-ttu-id="23845-138">json</span><span class="sxs-lookup"><span data-stu-id="23845-138">json</span></span>|<span data-ttu-id="23845-p105">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar.  Beispielsweise würde die englische Formel „= SUM(A1, 1.5)“ in Deutsch „= SUMME(A1; 1,5)“ werden.</span><span class="sxs-lookup"><span data-stu-id="23845-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="23845-141">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="23845-141">formulasR1C1</span></span>|<span data-ttu-id="23845-142">json</span><span class="sxs-lookup"><span data-stu-id="23845-142">json</span></span>|<span data-ttu-id="23845-143">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="23845-143">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="23845-144">numberFormat</span><span class="sxs-lookup"><span data-stu-id="23845-144">numberFormat</span></span>|<span data-ttu-id="23845-145">json</span><span class="sxs-lookup"><span data-stu-id="23845-145">json</span></span>|<span data-ttu-id="23845-146">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar.</span><span class="sxs-lookup"><span data-stu-id="23845-146">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="23845-147">rowHidden</span><span class="sxs-lookup"><span data-stu-id="23845-147">rowHidden</span></span>|<span data-ttu-id="23845-148">boolean</span><span class="sxs-lookup"><span data-stu-id="23845-148">boolean</span></span>|<span data-ttu-id="23845-149">Stellt dar, ob alle Zeilen des aktuellen Bereichs ausgeblendet sind.</span><span class="sxs-lookup"><span data-stu-id="23845-149">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="23845-150">values</span><span class="sxs-lookup"><span data-stu-id="23845-150">values</span></span>|<span data-ttu-id="23845-151">json</span><span class="sxs-lookup"><span data-stu-id="23845-151">json</span></span>|<span data-ttu-id="23845-p106">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="23845-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="23845-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="23845-155">Response</span></span>

<span data-ttu-id="23845-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23845-156">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23845-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23845-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23845-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23845-158">Request</span></span>
<span data-ttu-id="23845-p107">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es wird ein Bereich aktualisiert (Werte, Zahlenformate und Formeln) aktualisiert. Die `null`-Eingabe dient dazu, die API anzuweisen, die Zelle für diese bestimmte Eingabe zu ignorieren. Die Werte, Zahlenformate und Formeln können unabhängig aktualisiert im gleichen API-Aufruf miteinander kombiniert werden.</span><span class="sxs-lookup"><span data-stu-id="23845-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="23845-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="23845-163">Response</span></span>
<span data-ttu-id="23845-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23845-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

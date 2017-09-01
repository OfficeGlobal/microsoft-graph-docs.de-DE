# <a name="update-range"></a><span data-ttu-id="22a29-101">range aktualisieren</span><span class="sxs-lookup"><span data-stu-id="22a29-101">Update range</span></span>

<span data-ttu-id="22a29-102">Dient zum Aktualisieren der Eigenschaften des Bereichsobjekts.</span><span class="sxs-lookup"><span data-stu-id="22a29-102">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="22a29-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="22a29-103">Permissions</span></span>
<span data-ttu-id="22a29-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="22a29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="22a29-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22a29-106">Permission type</span></span>      | <span data-ttu-id="22a29-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22a29-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22a29-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22a29-108">Delegated (work or school account)</span></span> | <span data-ttu-id="22a29-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22a29-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22a29-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22a29-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22a29-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22a29-111">Not supported.</span></span>    |
|<span data-ttu-id="22a29-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22a29-112">Application</span></span> | <span data-ttu-id="22a29-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22a29-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22a29-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22a29-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address=<range-address>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="22a29-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22a29-115">Optional request headers</span></span>
| <span data-ttu-id="22a29-116">Name</span><span class="sxs-lookup"><span data-stu-id="22a29-116">Name</span></span>       | <span data-ttu-id="22a29-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22a29-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="22a29-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="22a29-118">Authorization</span></span>  | <span data-ttu-id="22a29-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22a29-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22a29-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22a29-121">Request body</span></span>
<span data-ttu-id="22a29-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="22a29-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="22a29-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="22a29-125">Property</span></span>     | <span data-ttu-id="22a29-126">Typ</span><span class="sxs-lookup"><span data-stu-id="22a29-126">Type</span></span>   |<span data-ttu-id="22a29-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22a29-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22a29-128">columnHidden</span><span class="sxs-lookup"><span data-stu-id="22a29-128">columnHidden</span></span>|<span data-ttu-id="22a29-129">boolean</span><span class="sxs-lookup"><span data-stu-id="22a29-129">boolean</span></span>|<span data-ttu-id="22a29-130">Stellt dar, ob alle Spalten des aktuellen Bereichs ausgeblendet sind.</span><span class="sxs-lookup"><span data-stu-id="22a29-130">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="22a29-131">formulas</span><span class="sxs-lookup"><span data-stu-id="22a29-131">formulas</span></span>|<span data-ttu-id="22a29-132">json</span><span class="sxs-lookup"><span data-stu-id="22a29-132">json</span></span>|<span data-ttu-id="22a29-133">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="22a29-133">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="22a29-134">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="22a29-134">formulasLocal</span></span>|<span data-ttu-id="22a29-135">json</span><span class="sxs-lookup"><span data-stu-id="22a29-135">json</span></span>|<span data-ttu-id="22a29-p104">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar.  Beispielsweise würde die englische Formel „= SUM(A1, 1.5)“ in Deutsch „= SUMME(A1; 1,5)“ werden.</span><span class="sxs-lookup"><span data-stu-id="22a29-p104">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="22a29-138">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="22a29-138">formulasR1C1</span></span>|<span data-ttu-id="22a29-139">json</span><span class="sxs-lookup"><span data-stu-id="22a29-139">json</span></span>|<span data-ttu-id="22a29-140">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="22a29-140">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="22a29-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="22a29-141">numberFormat</span></span>|<span data-ttu-id="22a29-142">json</span><span class="sxs-lookup"><span data-stu-id="22a29-142">json</span></span>|<span data-ttu-id="22a29-143">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar.</span><span class="sxs-lookup"><span data-stu-id="22a29-143">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="22a29-144">rowHidden</span><span class="sxs-lookup"><span data-stu-id="22a29-144">rowHidden</span></span>|<span data-ttu-id="22a29-145">boolean</span><span class="sxs-lookup"><span data-stu-id="22a29-145">boolean</span></span>|<span data-ttu-id="22a29-146">Stellt dar, ob alle Zeilen des aktuellen Bereichs ausgeblendet sind.</span><span class="sxs-lookup"><span data-stu-id="22a29-146">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="22a29-147">values</span><span class="sxs-lookup"><span data-stu-id="22a29-147">values</span></span>|<span data-ttu-id="22a29-148">json</span><span class="sxs-lookup"><span data-stu-id="22a29-148">json</span></span>|<span data-ttu-id="22a29-p105">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="22a29-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="22a29-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="22a29-152">Response</span></span>

<span data-ttu-id="22a29-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22a29-153">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="22a29-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22a29-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22a29-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22a29-155">Request</span></span>
<span data-ttu-id="22a29-p106">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es wird ein Bereich aktualisiert (Werte, Zahlenformate und Formeln) aktualisiert. Die `null`-Eingabe dient dazu, die API anzuweisen, die Zelle für diese bestimmte Eingabe zu ignorieren. Die Werte, Zahlenformate und Formeln können unabhängig aktualisiert im gleichen API-Aufruf miteinander kombiniert werden.</span><span class="sxs-lookup"><span data-stu-id="22a29-p106">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="22a29-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="22a29-160">Response</span></span>
<span data-ttu-id="22a29-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22a29-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

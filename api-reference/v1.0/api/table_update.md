# <a name="update-table"></a><span data-ttu-id="75bba-101">Tabelle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="75bba-101">Update table</span></span>

<span data-ttu-id="75bba-102">Dient zum Aktualisieren der Eigenschaften des Tabellenobjekts.</span><span class="sxs-lookup"><span data-stu-id="75bba-102">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="75bba-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="75bba-103">Permissions</span></span>
<span data-ttu-id="75bba-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75bba-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75bba-106">Permission type</span></span>      | <span data-ttu-id="75bba-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75bba-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75bba-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75bba-108">Delegated (work or school account)</span></span> | <span data-ttu-id="75bba-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75bba-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75bba-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75bba-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75bba-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75bba-111">Not supported.</span></span>    |
|<span data-ttu-id="75bba-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75bba-112">Application</span></span> | <span data-ttu-id="75bba-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75bba-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75bba-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75bba-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="75bba-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75bba-115">Optional request headers</span></span>
| <span data-ttu-id="75bba-116">Name</span><span class="sxs-lookup"><span data-stu-id="75bba-116">Name</span></span>       | <span data-ttu-id="75bba-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75bba-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="75bba-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="75bba-118">Authorization</span></span>  | <span data-ttu-id="75bba-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="75bba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75bba-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75bba-121">Request body</span></span>
<span data-ttu-id="75bba-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="75bba-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="75bba-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75bba-125">Property</span></span>     | <span data-ttu-id="75bba-126">Typ</span><span class="sxs-lookup"><span data-stu-id="75bba-126">Type</span></span>   |<span data-ttu-id="75bba-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75bba-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75bba-128">name</span><span class="sxs-lookup"><span data-stu-id="75bba-128">name</span></span>|<span data-ttu-id="75bba-129">string</span><span class="sxs-lookup"><span data-stu-id="75bba-129">string</span></span>|<span data-ttu-id="75bba-130">Der Name der Tabelle.</span><span class="sxs-lookup"><span data-stu-id="75bba-130">Name of the table.</span></span>|
|<span data-ttu-id="75bba-131">showHeaders</span><span class="sxs-lookup"><span data-stu-id="75bba-131">showHeaders</span></span>|<span data-ttu-id="75bba-132">boolean</span><span class="sxs-lookup"><span data-stu-id="75bba-132">boolean</span></span>|<span data-ttu-id="75bba-p104">Gibt an, ob die Kopfzeile sichtbar oder nicht sichtbar ist. Dieser Wert kann festgelegt werden, um die Kopfzeile anzuzeigen, oder sie zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="75bba-p104">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="75bba-135">showTotals</span><span class="sxs-lookup"><span data-stu-id="75bba-135">showTotals</span></span>|<span data-ttu-id="75bba-136">boolean</span><span class="sxs-lookup"><span data-stu-id="75bba-136">boolean</span></span>|<span data-ttu-id="75bba-p105">Gibt an, ob die Ergebniszeile sichtbar ist oder nicht. Dieser Wert kann so festgelegt werden, dass die Ergebniszeile angezeigt oder ausgeblendet wird.</span><span class="sxs-lookup"><span data-stu-id="75bba-p105">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="75bba-139">style</span><span class="sxs-lookup"><span data-stu-id="75bba-139">style</span></span>|<span data-ttu-id="75bba-140">string</span><span class="sxs-lookup"><span data-stu-id="75bba-140">string</span></span>|<span data-ttu-id="75bba-p106">Konstanter Wert, der das Tabellenformat darstellt. Die folgenden Werte sind möglich: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. Es kann ebenfalls eine in der Arbeitsmappe vorhandene benutzerdefinierte Formatierung angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="75bba-p106">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="75bba-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="75bba-144">Response</span></span>

<span data-ttu-id="75bba-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75bba-145">If successful, this method returns a `200 OK` response code and updated [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75bba-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75bba-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75bba-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75bba-147">Request</span></span>
<span data-ttu-id="75bba-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75bba-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="75bba-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="75bba-149">Response</span></span>
<span data-ttu-id="75bba-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75bba-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

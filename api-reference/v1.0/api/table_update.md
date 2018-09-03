# <a name="update-table"></a><span data-ttu-id="7e4e2-101">Tabelle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7e4e2-101">Update table</span></span>

<span data-ttu-id="7e4e2-102">Dient zum Aktualisieren der Eigenschaften des Tabellenobjekts.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-102">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e4e2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7e4e2-103">Permissions</span></span>
<span data-ttu-id="7e4e2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e4e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7e4e2-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e4e2-106">Permission type</span></span>      | <span data-ttu-id="7e4e2-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e4e2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e4e2-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e4e2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7e4e2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e4e2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e4e2-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e4e2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e4e2-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e4e2-111">Not supported.</span></span>    |
|<span data-ttu-id="7e4e2-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e4e2-112">Application</span></span> | <span data-ttu-id="7e4e2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e4e2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e4e2-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e4e2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7e4e2-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e4e2-115">Optional request headers</span></span>
| <span data-ttu-id="7e4e2-116">Name</span><span class="sxs-lookup"><span data-stu-id="7e4e2-116">Name</span></span>       | <span data-ttu-id="7e4e2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e4e2-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7e4e2-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7e4e2-118">Authorization</span></span>  | <span data-ttu-id="7e4e2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e4e2-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7e4e2-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="7e4e2-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e4e2-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e4e2-124">Request body</span></span>
<span data-ttu-id="7e4e2-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e4e2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e4e2-128">Property</span></span>     | <span data-ttu-id="7e4e2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7e4e2-129">Type</span></span>   |<span data-ttu-id="7e4e2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e4e2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e4e2-131">Name</span><span class="sxs-lookup"><span data-stu-id="7e4e2-131">name</span></span>|<span data-ttu-id="7e4e2-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e4e2-132">string</span></span>|<span data-ttu-id="7e4e2-133">Der Name der Tabelle.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-133">Name of the table.</span></span>|
|<span data-ttu-id="7e4e2-134">showHeaders</span><span class="sxs-lookup"><span data-stu-id="7e4e2-134">showHeaders</span></span>|<span data-ttu-id="7e4e2-135">boolesch</span><span class="sxs-lookup"><span data-stu-id="7e4e2-135">boolean</span></span>|<span data-ttu-id="7e4e2-p105">Gibt an, ob die Kopfzeile sichtbar oder nicht sichtbar ist. Dieser Wert kann festgelegt werden, um die Kopfzeile anzuzeigen, oder sie zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="7e4e2-138">showTotals</span><span class="sxs-lookup"><span data-stu-id="7e4e2-138">showTotals</span></span>|<span data-ttu-id="7e4e2-139">boolesch</span><span class="sxs-lookup"><span data-stu-id="7e4e2-139">boolean</span></span>|<span data-ttu-id="7e4e2-p106">Gibt an, ob die Ergebniszeile sichtbar ist oder nicht. Dieser Wert kann so festgelegt werden, dass die Ergebniszeile angezeigt oder ausgeblendet wird.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="7e4e2-142">Stil</span><span class="sxs-lookup"><span data-stu-id="7e4e2-142">style</span></span>|<span data-ttu-id="7e4e2-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e4e2-143">string</span></span>|<span data-ttu-id="7e4e2-144">Konstanter Wert, der das Tabellenformat darstellt.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-144">Constant value that represents the Table style.</span></span> <span data-ttu-id="7e4e2-145">Die möglichen Werte sind: TableStyleLight1 bis TableStyleLight21 TableStyleMedium1 bis TableStyleMedium28 TableStyleStyleDark1 bis TableStyleStyleDark11.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-145">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="7e4e2-146">Eine benutzerdefinierte Formatvorlage, die in der Arbeitsmappe vorhanden ist, kann auch angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-146">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="7e4e2-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e4e2-147">Response</span></span>

<span data-ttu-id="7e4e2-148">Wenn erfolgreich, gibt diese Methode einen Antwortcode `200 OK` und ein aktualisiertes [WorkbookTable](../resources/table.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-148">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e4e2-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e4e2-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e4e2-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e4e2-150">Request</span></span>
<span data-ttu-id="7e4e2-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-151">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="7e4e2-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e4e2-152">Response</span></span>
<span data-ttu-id="7e4e2-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e4e2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
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

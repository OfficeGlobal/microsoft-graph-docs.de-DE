# <a name="update-tablecolumn"></a><span data-ttu-id="7065c-101">tablecolumn aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7065c-101">Update tablecolumn</span></span>

<span data-ttu-id="7065c-102">Dient zum Aktualisieren der Eigenschaften des tablecolumn-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7065c-102">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7065c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7065c-103">Permissions</span></span>
<span data-ttu-id="7065c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7065c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7065c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7065c-106">Permission type</span></span>      | <span data-ttu-id="7065c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7065c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7065c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7065c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7065c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7065c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7065c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7065c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7065c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7065c-111">Not supported.</span></span>    |
|<span data-ttu-id="7065c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7065c-112">Application</span></span> | <span data-ttu-id="7065c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7065c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7065c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7065c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7065c-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7065c-115">Optional request headers</span></span>
| <span data-ttu-id="7065c-116">Name</span><span class="sxs-lookup"><span data-stu-id="7065c-116">Name</span></span>       | <span data-ttu-id="7065c-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7065c-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7065c-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7065c-118">Authorization</span></span>  | <span data-ttu-id="7065c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7065c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7065c-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7065c-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="7065c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7065c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7065c-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7065c-124">Request body</span></span>
<span data-ttu-id="7065c-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="7065c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7065c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7065c-128">Property</span></span>     | <span data-ttu-id="7065c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7065c-129">Type</span></span>   |<span data-ttu-id="7065c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7065c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7065c-131">Werte</span><span class="sxs-lookup"><span data-stu-id="7065c-131">values</span></span>|<span data-ttu-id="7065c-132">Json</span><span class="sxs-lookup"><span data-stu-id="7065c-132">Json</span></span>|<span data-ttu-id="7065c-p105">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="7065c-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="7065c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7065c-136">Response</span></span>

<span data-ttu-id="7065c-137">Wenn erfolgreich, gibt diese Methode einen `200 OK` Antwortcode und ein aktualisiertes [WorkbookTableColumn](../resources/tablecolumn.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7065c-137">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7065c-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7065c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7065c-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7065c-139">Request</span></span>
<span data-ttu-id="7065c-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7065c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="7065c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7065c-141">Response</span></span>
<span data-ttu-id="7065c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7065c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
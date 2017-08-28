# <a name="update-formatprotection"></a><span data-ttu-id="f1a90-101">formatprotection aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f1a90-101">Update formatprotection</span></span>

<span data-ttu-id="f1a90-102">Dient zum Aktualisieren der Eigenschaften des formatprotection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1a90-102">Update the properties of formatprotection object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1a90-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1a90-103">Prerequisites</span></span>
<span data-ttu-id="f1a90-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="f1a90-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="f1a90-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1a90-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="f1a90-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1a90-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="f1a90-107">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1a90-107">Optional request headers</span></span>
| <span data-ttu-id="f1a90-108">Name</span><span class="sxs-lookup"><span data-stu-id="f1a90-108">Name</span></span>       | <span data-ttu-id="f1a90-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1a90-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f1a90-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1a90-110">Authorization</span></span>  | <span data-ttu-id="f1a90-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f1a90-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1a90-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1a90-113">Request body</span></span>
<span data-ttu-id="f1a90-p102">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f1a90-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f1a90-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1a90-117">Property</span></span>     | <span data-ttu-id="f1a90-118">Typ</span><span class="sxs-lookup"><span data-stu-id="f1a90-118">Type</span></span>   |<span data-ttu-id="f1a90-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1a90-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1a90-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="f1a90-120">formulaHidden</span></span>|<span data-ttu-id="f1a90-121">boolean</span><span class="sxs-lookup"><span data-stu-id="f1a90-121">boolean</span></span>|<span data-ttu-id="f1a90-p103">Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.</span><span class="sxs-lookup"><span data-stu-id="f1a90-p103">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="f1a90-124">locked</span><span class="sxs-lookup"><span data-stu-id="f1a90-124">locked</span></span>|<span data-ttu-id="f1a90-125">boolean</span><span class="sxs-lookup"><span data-stu-id="f1a90-125">boolean</span></span>|<span data-ttu-id="f1a90-p104">Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.</span><span class="sxs-lookup"><span data-stu-id="f1a90-p104">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="f1a90-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1a90-128">Response</span></span>

<span data-ttu-id="f1a90-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [FormatProtection](../resources/formatprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1a90-129">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1a90-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1a90-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1a90-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1a90-131">Request</span></span>
<span data-ttu-id="f1a90-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1a90-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="f1a90-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1a90-133">Response</span></span>
<span data-ttu-id="f1a90-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1a90-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
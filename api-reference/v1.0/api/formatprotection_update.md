# <a name="update-formatprotection"></a><span data-ttu-id="11865-101">formatprotection aktualisieren</span><span class="sxs-lookup"><span data-stu-id="11865-101">Update formatprotection</span></span>

<span data-ttu-id="11865-102">Dient zum Aktualisieren der Eigenschaften des formatprotection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="11865-102">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="11865-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="11865-103">Permissions</span></span>
<span data-ttu-id="11865-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="11865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="11865-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11865-106">Permission type</span></span>      | <span data-ttu-id="11865-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11865-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="11865-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11865-108">Delegated (work or school account)</span></span> | <span data-ttu-id="11865-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11865-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="11865-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11865-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11865-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11865-111">Not supported.</span></span>    | 
|<span data-ttu-id="11865-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11865-112">Application</span></span> | <span data-ttu-id="11865-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11865-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="11865-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11865-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="11865-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11865-115">Optional request headers</span></span>
| <span data-ttu-id="11865-116">Name</span><span class="sxs-lookup"><span data-stu-id="11865-116">Name</span></span>       | <span data-ttu-id="11865-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11865-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="11865-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="11865-118">Authorization</span></span>  | <span data-ttu-id="11865-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11865-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="11865-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11865-121">Request body</span></span>
<span data-ttu-id="11865-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="11865-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="11865-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11865-125">Property</span></span>     | <span data-ttu-id="11865-126">Typ</span><span class="sxs-lookup"><span data-stu-id="11865-126">Type</span></span>   |<span data-ttu-id="11865-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11865-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11865-128">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="11865-128">formulaHidden</span></span>|<span data-ttu-id="11865-129">boolean</span><span class="sxs-lookup"><span data-stu-id="11865-129">boolean</span></span>|<span data-ttu-id="11865-p104">Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.</span><span class="sxs-lookup"><span data-stu-id="11865-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="11865-132">locked</span><span class="sxs-lookup"><span data-stu-id="11865-132">locked</span></span>|<span data-ttu-id="11865-133">boolean</span><span class="sxs-lookup"><span data-stu-id="11865-133">boolean</span></span>|<span data-ttu-id="11865-p105">Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.</span><span class="sxs-lookup"><span data-stu-id="11865-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="11865-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="11865-136">Response</span></span>

<span data-ttu-id="11865-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [FormatProtection](../resources/formatprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11865-137">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="11865-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11865-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11865-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11865-139">Request</span></span>
<span data-ttu-id="11865-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11865-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="11865-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="11865-141">Response</span></span>
<span data-ttu-id="11865-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11865-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
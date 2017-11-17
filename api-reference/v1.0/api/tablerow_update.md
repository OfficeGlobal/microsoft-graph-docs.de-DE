# <a name="update-tablerow"></a><span data-ttu-id="aa717-101">tablerow aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aa717-101">Update tablerow</span></span>

<span data-ttu-id="aa717-102">Dient zum Aktualisieren der Eigenschaften des tablerow-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa717-102">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa717-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa717-103">Permissions</span></span>
<span data-ttu-id="aa717-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa717-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa717-106">Permission type</span></span>      | <span data-ttu-id="aa717-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa717-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa717-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa717-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aa717-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa717-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa717-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa717-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa717-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa717-111">Not supported.</span></span>    |
|<span data-ttu-id="aa717-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa717-112">Application</span></span> | <span data-ttu-id="aa717-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa717-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa717-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa717-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="aa717-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa717-115">Optional request headers</span></span>
| <span data-ttu-id="aa717-116">Name</span><span class="sxs-lookup"><span data-stu-id="aa717-116">Name</span></span>       | <span data-ttu-id="aa717-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa717-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="aa717-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa717-118">Authorization</span></span>  | <span data-ttu-id="aa717-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa717-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa717-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa717-121">Request body</span></span>
<span data-ttu-id="aa717-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="aa717-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aa717-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa717-125">Property</span></span>     | <span data-ttu-id="aa717-126">Typ</span><span class="sxs-lookup"><span data-stu-id="aa717-126">Type</span></span>   |<span data-ttu-id="aa717-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa717-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa717-128">values</span><span class="sxs-lookup"><span data-stu-id="aa717-128">values</span></span>|<span data-ttu-id="aa717-129">json</span><span class="sxs-lookup"><span data-stu-id="aa717-129">json</span></span>|<span data-ttu-id="aa717-p104">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="aa717-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="aa717-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa717-133">Response</span></span>

<span data-ttu-id="aa717-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa717-134">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa717-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa717-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa717-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa717-136">Request</span></span>
<span data-ttu-id="aa717-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa717-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="aa717-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa717-138">Response</span></span>
<span data-ttu-id="aa717-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa717-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
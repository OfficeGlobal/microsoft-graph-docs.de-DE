# <a name="update-rangefill"></a><span data-ttu-id="44685-101">rangefill aktualisieren</span><span class="sxs-lookup"><span data-stu-id="44685-101">Update rangefill</span></span>

<span data-ttu-id="44685-102">Dient zum Aktualisieren der Eigenschaften des rangefill-Objekts.</span><span class="sxs-lookup"><span data-stu-id="44685-102">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="44685-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="44685-103">Permissions</span></span>
<span data-ttu-id="44685-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="44685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44685-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44685-106">Permission type</span></span>      | <span data-ttu-id="44685-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44685-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44685-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44685-108">Delegated (work or school account)</span></span> | <span data-ttu-id="44685-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44685-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44685-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44685-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44685-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44685-111">Not supported.</span></span>    |
|<span data-ttu-id="44685-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44685-112">Application</span></span> | <span data-ttu-id="44685-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44685-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44685-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44685-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="44685-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44685-115">Optional request headers</span></span>
| <span data-ttu-id="44685-116">Name</span><span class="sxs-lookup"><span data-stu-id="44685-116">Name</span></span>       | <span data-ttu-id="44685-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44685-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="44685-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="44685-118">Authorization</span></span>  | <span data-ttu-id="44685-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44685-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44685-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="44685-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="44685-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="44685-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44685-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44685-124">Request body</span></span>
<span data-ttu-id="44685-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="44685-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="44685-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44685-128">Property</span></span>     | <span data-ttu-id="44685-129">Typ</span><span class="sxs-lookup"><span data-stu-id="44685-129">Type</span></span>   |<span data-ttu-id="44685-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44685-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44685-131">color</span><span class="sxs-lookup"><span data-stu-id="44685-131">color</span></span>|<span data-ttu-id="44685-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="44685-132">string</span></span>|<span data-ttu-id="44685-133">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.</span><span class="sxs-lookup"><span data-stu-id="44685-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="44685-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="44685-134">Response</span></span>

<span data-ttu-id="44685-135">Wenn erfolgreich, gibt dieses Verfahren im Antworttext einen `200 OK` Antwortcode und ein aktualisiertes[WorkbookRangefill](../resources/rangefill.md)-Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="44685-135">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44685-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44685-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44685-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44685-137">Request</span></span>
<span data-ttu-id="44685-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44685-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="44685-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="44685-139">Response</span></span>
<span data-ttu-id="44685-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44685-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# <a name="update-chartfont"></a><span data-ttu-id="90c87-101">ChartFont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="90c87-101">Update chartfont</span></span>

<span data-ttu-id="90c87-102">Dient zum Aktualisieren der Eigenschaften des ChartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="90c87-102">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="90c87-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="90c87-103">Permissions</span></span>
<span data-ttu-id="90c87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="90c87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="90c87-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90c87-106">Permission type</span></span>      | <span data-ttu-id="90c87-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90c87-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90c87-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90c87-108">Delegated (work or school account)</span></span> | <span data-ttu-id="90c87-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90c87-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90c87-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90c87-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90c87-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90c87-111">Not supported.</span></span>    |
|<span data-ttu-id="90c87-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90c87-112">Application</span></span> | <span data-ttu-id="90c87-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90c87-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90c87-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90c87-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="90c87-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="90c87-115">Optional request headers</span></span>
| <span data-ttu-id="90c87-116">Name</span><span class="sxs-lookup"><span data-stu-id="90c87-116">Name</span></span>       | <span data-ttu-id="90c87-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90c87-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="90c87-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="90c87-118">Authorization</span></span>  | <span data-ttu-id="90c87-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="90c87-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90c87-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="90c87-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="90c87-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="90c87-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90c87-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90c87-124">Request body</span></span>
<span data-ttu-id="90c87-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="90c87-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="90c87-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90c87-128">Property</span></span>     | <span data-ttu-id="90c87-129">Typ</span><span class="sxs-lookup"><span data-stu-id="90c87-129">Type</span></span>   |<span data-ttu-id="90c87-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90c87-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90c87-131">bold</span><span class="sxs-lookup"><span data-stu-id="90c87-131">bold</span></span>|<span data-ttu-id="90c87-132">boolean</span><span class="sxs-lookup"><span data-stu-id="90c87-132">boolean</span></span>|<span data-ttu-id="90c87-133">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="90c87-133">Represents the bold status of font.</span></span>|
|<span data-ttu-id="90c87-134">color</span><span class="sxs-lookup"><span data-stu-id="90c87-134">color</span></span>|<span data-ttu-id="90c87-135">string</span><span class="sxs-lookup"><span data-stu-id="90c87-135">string</span></span>|<span data-ttu-id="90c87-p105">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="90c87-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="90c87-139">italic</span><span class="sxs-lookup"><span data-stu-id="90c87-139">italic</span></span>|<span data-ttu-id="90c87-140">boolean</span><span class="sxs-lookup"><span data-stu-id="90c87-140">boolean</span></span>|<span data-ttu-id="90c87-141">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="90c87-141">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="90c87-142">name</span><span class="sxs-lookup"><span data-stu-id="90c87-142">name</span></span>|<span data-ttu-id="90c87-143">string</span><span class="sxs-lookup"><span data-stu-id="90c87-143">string</span></span>|<span data-ttu-id="90c87-144">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="90c87-144">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="90c87-145">size</span><span class="sxs-lookup"><span data-stu-id="90c87-145">size</span></span>|<span data-ttu-id="90c87-146">double</span><span class="sxs-lookup"><span data-stu-id="90c87-146">double</span></span>|<span data-ttu-id="90c87-147">Der Schriftgrad (z. B. 11)</span><span class="sxs-lookup"><span data-stu-id="90c87-147">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="90c87-148">underline</span><span class="sxs-lookup"><span data-stu-id="90c87-148">underline</span></span>|<span data-ttu-id="90c87-149">string</span><span class="sxs-lookup"><span data-stu-id="90c87-149">string</span></span>|<span data-ttu-id="90c87-150">Art der Unterstreichung für die Schriftart.</span><span class="sxs-lookup"><span data-stu-id="90c87-150">Type of underline applied to the font. Possible values are: , .</span></span> <span data-ttu-id="90c87-151">Mögliche Werte sind: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="90c87-151">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="90c87-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="90c87-152">Response</span></span>

<span data-ttu-id="90c87-153">Wenn das Verfahren erfolgreich verläuft, werden im Antworttext der `200 OK` Antwortcode und ein aktualisiertes [WorkbookChartFont](../resources/chartfont.md)-Objekt zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90c87-153">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90c87-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90c87-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90c87-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90c87-155">Request</span></span>
<span data-ttu-id="90c87-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90c87-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="90c87-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="90c87-157">Response</span></span>
<span data-ttu-id="90c87-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90c87-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
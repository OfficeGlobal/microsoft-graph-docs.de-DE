# <a name="update-chartfont"></a><span data-ttu-id="37b8e-101">ChartFont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="37b8e-101">Update chartfont</span></span>

<span data-ttu-id="37b8e-102">Dient zum Aktualisieren der Eigenschaften des ChartFont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="37b8e-102">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="37b8e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="37b8e-103">Permissions</span></span>
<span data-ttu-id="37b8e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="37b8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="37b8e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37b8e-106">Permission type</span></span>      | <span data-ttu-id="37b8e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37b8e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37b8e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37b8e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="37b8e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37b8e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="37b8e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37b8e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37b8e-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37b8e-111">Not supported.</span></span>    |
|<span data-ttu-id="37b8e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37b8e-112">Application</span></span> | <span data-ttu-id="37b8e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37b8e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37b8e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37b8e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="37b8e-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37b8e-115">Optional request headers</span></span>
| <span data-ttu-id="37b8e-116">Name</span><span class="sxs-lookup"><span data-stu-id="37b8e-116">Name</span></span>       | <span data-ttu-id="37b8e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37b8e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="37b8e-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="37b8e-118">Authorization</span></span>  | <span data-ttu-id="37b8e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="37b8e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37b8e-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37b8e-121">Request body</span></span>
<span data-ttu-id="37b8e-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="37b8e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="37b8e-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37b8e-125">Property</span></span>     | <span data-ttu-id="37b8e-126">Typ</span><span class="sxs-lookup"><span data-stu-id="37b8e-126">Type</span></span>   |<span data-ttu-id="37b8e-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37b8e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37b8e-128">bold</span><span class="sxs-lookup"><span data-stu-id="37b8e-128">bold</span></span>|<span data-ttu-id="37b8e-129">boolean</span><span class="sxs-lookup"><span data-stu-id="37b8e-129">boolean</span></span>|<span data-ttu-id="37b8e-130">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="37b8e-130">Represents the bold status of font.</span></span>|
|<span data-ttu-id="37b8e-131">color</span><span class="sxs-lookup"><span data-stu-id="37b8e-131">color</span></span>|<span data-ttu-id="37b8e-132">string</span><span class="sxs-lookup"><span data-stu-id="37b8e-132">string</span></span>|<span data-ttu-id="37b8e-p104">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="37b8e-p104">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="37b8e-136">italic</span><span class="sxs-lookup"><span data-stu-id="37b8e-136">italic</span></span>|<span data-ttu-id="37b8e-137">boolean</span><span class="sxs-lookup"><span data-stu-id="37b8e-137">boolean</span></span>|<span data-ttu-id="37b8e-138">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="37b8e-138">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="37b8e-139">name</span><span class="sxs-lookup"><span data-stu-id="37b8e-139">name</span></span>|<span data-ttu-id="37b8e-140">string</span><span class="sxs-lookup"><span data-stu-id="37b8e-140">string</span></span>|<span data-ttu-id="37b8e-141">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="37b8e-141">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="37b8e-142">size</span><span class="sxs-lookup"><span data-stu-id="37b8e-142">size</span></span>|<span data-ttu-id="37b8e-143">double</span><span class="sxs-lookup"><span data-stu-id="37b8e-143">double</span></span>|<span data-ttu-id="37b8e-144">Der Schriftgrad (z. B. 11)</span><span class="sxs-lookup"><span data-stu-id="37b8e-144">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="37b8e-145">underline</span><span class="sxs-lookup"><span data-stu-id="37b8e-145">underline</span></span>|<span data-ttu-id="37b8e-146">string</span><span class="sxs-lookup"><span data-stu-id="37b8e-146">string</span></span>|<span data-ttu-id="37b8e-p105">Art der auf die Schriftart angewendeten Unterstreichung. Mögliche Werte: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="37b8e-p105">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="37b8e-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="37b8e-149">Response</span></span>

<span data-ttu-id="37b8e-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartFont](../resources/chartfont.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37b8e-150">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37b8e-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37b8e-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37b8e-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37b8e-152">Request</span></span>
<span data-ttu-id="37b8e-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37b8e-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
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
##### <a name="response"></a><span data-ttu-id="37b8e-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="37b8e-154">Response</span></span>
<span data-ttu-id="37b8e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37b8e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
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
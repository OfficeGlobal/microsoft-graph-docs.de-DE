# <a name="update-rangefont"></a><span data-ttu-id="f389d-101">rangefont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f389d-101">Update rangefont</span></span>

<span data-ttu-id="f389d-102">Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f389d-102">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f389d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f389d-103">Permissions</span></span>
<span data-ttu-id="f389d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f389d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f389d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f389d-106">Permission type</span></span>      | <span data-ttu-id="f389d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f389d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f389d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f389d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f389d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f389d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f389d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f389d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f389d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f389d-111">Not supported.</span></span>    |
|<span data-ttu-id="f389d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f389d-112">Application</span></span> | <span data-ttu-id="f389d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f389d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f389d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f389d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="f389d-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f389d-115">Optional request headers</span></span>
| <span data-ttu-id="f389d-116">Name</span><span class="sxs-lookup"><span data-stu-id="f389d-116">Name</span></span>       | <span data-ttu-id="f389d-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f389d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f389d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="f389d-118">Authorization</span></span>  | <span data-ttu-id="f389d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f389d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f389d-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f389d-121">Request body</span></span>
<span data-ttu-id="f389d-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f389d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f389d-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f389d-125">Property</span></span>     | <span data-ttu-id="f389d-126">Typ</span><span class="sxs-lookup"><span data-stu-id="f389d-126">Type</span></span>   |<span data-ttu-id="f389d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f389d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f389d-128">bold</span><span class="sxs-lookup"><span data-stu-id="f389d-128">bold</span></span>|<span data-ttu-id="f389d-129">boolean</span><span class="sxs-lookup"><span data-stu-id="f389d-129">boolean</span></span>|<span data-ttu-id="f389d-130">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="f389d-130">Represents the bold status of font.</span></span>|
|<span data-ttu-id="f389d-131">color</span><span class="sxs-lookup"><span data-stu-id="f389d-131">color</span></span>|<span data-ttu-id="f389d-132">string</span><span class="sxs-lookup"><span data-stu-id="f389d-132">string</span></span>|<span data-ttu-id="f389d-p104">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="f389d-p104">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="f389d-136">italic</span><span class="sxs-lookup"><span data-stu-id="f389d-136">italic</span></span>|<span data-ttu-id="f389d-137">boolean</span><span class="sxs-lookup"><span data-stu-id="f389d-137">boolean</span></span>|<span data-ttu-id="f389d-138">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="f389d-138">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="f389d-139">name</span><span class="sxs-lookup"><span data-stu-id="f389d-139">name</span></span>|<span data-ttu-id="f389d-140">string</span><span class="sxs-lookup"><span data-stu-id="f389d-140">string</span></span>|<span data-ttu-id="f389d-141">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="f389d-141">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="f389d-142">size</span><span class="sxs-lookup"><span data-stu-id="f389d-142">size</span></span>|<span data-ttu-id="f389d-143">double</span><span class="sxs-lookup"><span data-stu-id="f389d-143">double</span></span>|<span data-ttu-id="f389d-144">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="f389d-144">Font size.</span></span>|
|<span data-ttu-id="f389d-145">underline</span><span class="sxs-lookup"><span data-stu-id="f389d-145">underline</span></span>|<span data-ttu-id="f389d-146">string</span><span class="sxs-lookup"><span data-stu-id="f389d-146">string</span></span>|<span data-ttu-id="f389d-p105">Art der auf die Schriftart angewendete Unterstreichung. Die folgenden Werte sind möglich: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="f389d-p105">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="f389d-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="f389d-149">Response</span></span>

<span data-ttu-id="f389d-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeFont](../resources/rangefont.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f389d-150">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f389d-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f389d-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f389d-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f389d-152">Request</span></span>
<span data-ttu-id="f389d-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f389d-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/font
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
##### <a name="response"></a><span data-ttu-id="f389d-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="f389d-154">Response</span></span>
<span data-ttu-id="f389d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f389d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
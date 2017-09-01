# <a name="update-chartaxis"></a><span data-ttu-id="0fa11-101">ChartAxis aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0fa11-101">Update chartaxis</span></span>

<span data-ttu-id="0fa11-102">Dient zum Aktualisieren der Eigenschaften des ChartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0fa11-102">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0fa11-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0fa11-103">Permissions</span></span>
<span data-ttu-id="0fa11-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0fa11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0fa11-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0fa11-106">Permission type</span></span>      | <span data-ttu-id="0fa11-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0fa11-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fa11-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0fa11-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0fa11-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fa11-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0fa11-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0fa11-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa11-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fa11-111">Not supported.</span></span>    |
|<span data-ttu-id="0fa11-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0fa11-112">Application</span></span> | <span data-ttu-id="0fa11-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fa11-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fa11-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fa11-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="0fa11-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0fa11-115">Optional request headers</span></span>
| <span data-ttu-id="0fa11-116">Name</span><span class="sxs-lookup"><span data-stu-id="0fa11-116">Name</span></span>       | <span data-ttu-id="0fa11-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fa11-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0fa11-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fa11-118">Authorization</span></span>  | <span data-ttu-id="0fa11-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0fa11-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fa11-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0fa11-121">Request body</span></span>
<span data-ttu-id="0fa11-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0fa11-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0fa11-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0fa11-125">Property</span></span>     | <span data-ttu-id="0fa11-126">Typ</span><span class="sxs-lookup"><span data-stu-id="0fa11-126">Type</span></span>   |<span data-ttu-id="0fa11-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fa11-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fa11-128">majorUnit</span><span class="sxs-lookup"><span data-stu-id="0fa11-128">majorUnit</span></span>|<span data-ttu-id="0fa11-129">object</span><span class="sxs-lookup"><span data-stu-id="0fa11-129">object</span></span>|<span data-ttu-id="0fa11-p104">Stellt das Intervall zwischen zwei Hauptteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden.  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="0fa11-p104">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="0fa11-133">maximum</span><span class="sxs-lookup"><span data-stu-id="0fa11-133">maximum</span></span>|<span data-ttu-id="0fa11-134">object</span><span class="sxs-lookup"><span data-stu-id="0fa11-134">object</span></span>|<span data-ttu-id="0fa11-p105">Stellt den Maximalwert auf der Größenachse dar.  Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="0fa11-p105">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="0fa11-138">minimum</span><span class="sxs-lookup"><span data-stu-id="0fa11-138">minimum</span></span>|<span data-ttu-id="0fa11-139">object</span><span class="sxs-lookup"><span data-stu-id="0fa11-139">object</span></span>|<span data-ttu-id="0fa11-p106">Stellt den Mindestwert auf der Größenachse dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="0fa11-p106">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="0fa11-143">minorUnit</span><span class="sxs-lookup"><span data-stu-id="0fa11-143">minorUnit</span></span>|<span data-ttu-id="0fa11-144">object</span><span class="sxs-lookup"><span data-stu-id="0fa11-144">object</span></span>|<span data-ttu-id="0fa11-p107">Stellt das Intervall zwischen zwei Hilfsteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte). Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="0fa11-p107">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="0fa11-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fa11-148">Response</span></span>

<span data-ttu-id="0fa11-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartAxis](../resources/chartaxis.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fa11-149">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0fa11-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0fa11-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fa11-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fa11-151">Request</span></span>
<span data-ttu-id="0fa11-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0fa11-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="0fa11-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fa11-153">Response</span></span>
<span data-ttu-id="0fa11-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fa11-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
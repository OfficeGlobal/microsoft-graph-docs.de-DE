# <a name="chart-image"></a><span data-ttu-id="863c2-101">Diagramm: Bild</span><span class="sxs-lookup"><span data-stu-id="863c2-101">Chart: Image</span></span>

<span data-ttu-id="863c2-102">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="863c2-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="863c2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="863c2-103">Permissions</span></span>
<span data-ttu-id="863c2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="863c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="863c2-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="863c2-106">Permission type</span></span>      | <span data-ttu-id="863c2-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="863c2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="863c2-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="863c2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="863c2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="863c2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="863c2-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="863c2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="863c2-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="863c2-111">Not supported.</span></span>    |
|<span data-ttu-id="863c2-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="863c2-112">Application</span></span> | <span data-ttu-id="863c2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="863c2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="863c2-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="863c2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="863c2-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="863c2-115">Request headers</span></span>
| <span data-ttu-id="863c2-116">Name</span><span class="sxs-lookup"><span data-stu-id="863c2-116">Name</span></span>       | <span data-ttu-id="863c2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="863c2-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="863c2-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="863c2-118">Authorization</span></span>  | <span data-ttu-id="863c2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="863c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="863c2-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="863c2-121">Request body</span></span>
<span data-ttu-id="863c2-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="863c2-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="863c2-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="863c2-123">Parameter</span></span>    | <span data-ttu-id="863c2-124">Typ</span><span class="sxs-lookup"><span data-stu-id="863c2-124">Type</span></span>   |<span data-ttu-id="863c2-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="863c2-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="863c2-126">height</span><span class="sxs-lookup"><span data-stu-id="863c2-126">height</span></span>|<span data-ttu-id="863c2-127">number</span><span class="sxs-lookup"><span data-stu-id="863c2-127">number</span></span>|<span data-ttu-id="863c2-p103">Optional. Die gewünschte Höhe des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="863c2-p103">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="863c2-130">width</span><span class="sxs-lookup"><span data-stu-id="863c2-130">width</span></span>|<span data-ttu-id="863c2-131">number</span><span class="sxs-lookup"><span data-stu-id="863c2-131">number</span></span>|<span data-ttu-id="863c2-p104">Optional. Die gewünschte Breite des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="863c2-p104">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="863c2-134">fittingMode</span><span class="sxs-lookup"><span data-stu-id="863c2-134">fittingMode</span></span>|<span data-ttu-id="863c2-135">string</span><span class="sxs-lookup"><span data-stu-id="863c2-135">string</span></span>|<span data-ttu-id="863c2-p105">Optional. Die Methode, die verwendet wird, um das Diagramm auf die angegebenen Maße zu skalieren (wenn Höhe und Breite festgelegt sind).  Mögliche Werte: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="863c2-p105">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="863c2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="863c2-139">Response</span></span>

<span data-ttu-id="863c2-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine base64-Bildzeichenfolge im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="863c2-140">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="863c2-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="863c2-141">Example</span></span>
<span data-ttu-id="863c2-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="863c2-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="863c2-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="863c2-143">Request</span></span>
<span data-ttu-id="863c2-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="863c2-144">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
Content-type: application/json
Content-length: 77

{
  "height": {
  },
  "width": {
  },
  "fittingMode": "fittingMode-value"
}
```

##### <a name="response"></a><span data-ttu-id="863c2-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="863c2-145">Response</span></span>
<span data-ttu-id="863c2-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="863c2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

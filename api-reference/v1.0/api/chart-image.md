---
title: 'Diagramm: Bild'
description: Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.
author: lumine2008
ms.openlocfilehash: ccf2ba82dad05508b0857122f0316be8afcd03bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318193"
---
# <a name="chart-image"></a><span data-ttu-id="ac81a-103">Diagramm: Bild</span><span class="sxs-lookup"><span data-stu-id="ac81a-103">Chart: Image</span></span>

<span data-ttu-id="ac81a-104">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="ac81a-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="ac81a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ac81a-105">Permissions</span></span>
<span data-ttu-id="ac81a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac81a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac81a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac81a-108">Permission type</span></span>      | <span data-ttu-id="ac81a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac81a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac81a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac81a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac81a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac81a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ac81a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac81a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac81a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac81a-113">Not supported.</span></span>    |
|<span data-ttu-id="ac81a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac81a-114">Application</span></span> | <span data-ttu-id="ac81a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac81a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac81a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac81a-116">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="ac81a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac81a-117">Request headers</span></span>
| <span data-ttu-id="ac81a-118">Name</span><span class="sxs-lookup"><span data-stu-id="ac81a-118">Name</span></span>       | <span data-ttu-id="ac81a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac81a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ac81a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac81a-120">Authorization</span></span>  | <span data-ttu-id="ac81a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ac81a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac81a-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="ac81a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ac81a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="ac81a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="ac81a-126">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="ac81a-126">Path parameters</span></span>
<span data-ttu-id="ac81a-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ac81a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac81a-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="ac81a-128">Parameter</span></span>    | <span data-ttu-id="ac81a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ac81a-129">Type</span></span>   |<span data-ttu-id="ac81a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac81a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac81a-131">height</span><span class="sxs-lookup"><span data-stu-id="ac81a-131">height</span></span>|<span data-ttu-id="ac81a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ac81a-132">Int32</span></span>|<span data-ttu-id="ac81a-133">Die gewünschte Höhe des resultierenden Bildes.</span><span class="sxs-lookup"><span data-stu-id="ac81a-133">The desired height of the resulting image.</span></span> <span data-ttu-id="ac81a-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="ac81a-134">Optional.</span></span>|
|<span data-ttu-id="ac81a-135">width</span><span class="sxs-lookup"><span data-stu-id="ac81a-135">width</span></span>|<span data-ttu-id="ac81a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ac81a-136">Int32</span></span>|<span data-ttu-id="ac81a-137">Die gewünschte Breite des resultierenden Bildes.</span><span class="sxs-lookup"><span data-stu-id="ac81a-137">The desired width of the resulting image.</span></span> <span data-ttu-id="ac81a-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="ac81a-138">Optional.</span></span>|
|<span data-ttu-id="ac81a-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="ac81a-139">fittingMode</span></span>|<span data-ttu-id="ac81a-140">string</span><span class="sxs-lookup"><span data-stu-id="ac81a-140">string</span></span>|<span data-ttu-id="ac81a-141">Die Methode verwendet, um das Diagramm zu den angegebenen Dimensionen skalieren (wenn die Höhe und Breite festgelegt werden)."</span><span class="sxs-lookup"><span data-stu-id="ac81a-141">The method used to scale the chart to the specified dimensions (if both height and width are set)."</span></span>  <span data-ttu-id="ac81a-142">Die möglichen Werte sind: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="ac81a-142">The possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="ac81a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac81a-143">Response</span></span>

<span data-ttu-id="ac81a-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine base64-Bildzeichenfolge im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac81a-144">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac81a-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac81a-145">Example</span></span>
<span data-ttu-id="ac81a-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ac81a-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ac81a-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac81a-147">Request</span></span>
<span data-ttu-id="ac81a-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac81a-148">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="ac81a-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac81a-149">Response</span></span>
<span data-ttu-id="ac81a-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac81a-150">Here is an example of the response.</span></span> <span data-ttu-id="ac81a-151">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ac81a-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ac81a-152">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac81a-152">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="ac81a-153">Verwendung</span><span class="sxs-lookup"><span data-stu-id="ac81a-153">Usage</span></span>

<span data-ttu-id="ac81a-154">Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="ac81a-154">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="ac81a-155">Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="ac81a-155">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="ac81a-156">Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="ac81a-156">Here is an example of a chart image returned with the default parameters.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="ac81a-158">Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an.</span><span class="sxs-lookup"><span data-stu-id="ac81a-158">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="ac81a-159">So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="ac81a-159">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'Diagramm: Bild'
description: Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.
ms.openlocfilehash: 0930300413b68424d4d1613f0dbe76b531ae91f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058376"
---
# <a name="chart-image"></a><span data-ttu-id="48ccd-103">Diagramm: Bild</span><span class="sxs-lookup"><span data-stu-id="48ccd-103">Chart: Image</span></span>

> <span data-ttu-id="48ccd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="48ccd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48ccd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48ccd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48ccd-106">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="48ccd-106">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="48ccd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48ccd-107">Permissions</span></span>
<span data-ttu-id="48ccd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48ccd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48ccd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48ccd-110">Permission type</span></span>      | <span data-ttu-id="48ccd-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48ccd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48ccd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48ccd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48ccd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48ccd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="48ccd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48ccd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48ccd-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48ccd-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="48ccd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48ccd-116">Application</span></span> | <span data-ttu-id="48ccd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48ccd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48ccd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48ccd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="48ccd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48ccd-119">Request headers</span></span>
| <span data-ttu-id="48ccd-120">Name</span><span class="sxs-lookup"><span data-stu-id="48ccd-120">Name</span></span>       | <span data-ttu-id="48ccd-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48ccd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48ccd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48ccd-122">Authorization</span></span>  | <span data-ttu-id="48ccd-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48ccd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48ccd-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="48ccd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="48ccd-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="48ccd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48ccd-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48ccd-128">Request body</span></span>
<span data-ttu-id="48ccd-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="48ccd-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48ccd-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="48ccd-130">Parameter</span></span>    | <span data-ttu-id="48ccd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="48ccd-131">Type</span></span>   |<span data-ttu-id="48ccd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48ccd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48ccd-133">height</span><span class="sxs-lookup"><span data-stu-id="48ccd-133">height</span></span>|<span data-ttu-id="48ccd-134">number</span><span class="sxs-lookup"><span data-stu-id="48ccd-134">number</span></span>|<span data-ttu-id="48ccd-p105">Optional. Die gewünschte Höhe des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="48ccd-p105">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="48ccd-137">width</span><span class="sxs-lookup"><span data-stu-id="48ccd-137">width</span></span>|<span data-ttu-id="48ccd-138">number</span><span class="sxs-lookup"><span data-stu-id="48ccd-138">number</span></span>|<span data-ttu-id="48ccd-p106">Optional. Die gewünschte Breite des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="48ccd-p106">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="48ccd-141">fittingMode</span><span class="sxs-lookup"><span data-stu-id="48ccd-141">fittingMode</span></span>|<span data-ttu-id="48ccd-142">string</span><span class="sxs-lookup"><span data-stu-id="48ccd-142">string</span></span>|<span data-ttu-id="48ccd-p107">Optional. Die Methode, die verwendet wird, um das Diagramm auf die angegebenen Maße zu skalieren (wenn Höhe und Breite festgelegt sind).  Mögliche Werte: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="48ccd-p107">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="48ccd-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="48ccd-146">Response</span></span>

<span data-ttu-id="48ccd-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine base64-Bildzeichenfolge im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48ccd-147">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48ccd-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48ccd-148">Example</span></span>
<span data-ttu-id="48ccd-149">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="48ccd-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="48ccd-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48ccd-150">Request</span></span>
<span data-ttu-id="48ccd-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48ccd-151">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="48ccd-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="48ccd-152">Response</span></span>
<span data-ttu-id="48ccd-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="48ccd-153">Here is an example of the response.</span></span> <span data-ttu-id="48ccd-154">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="48ccd-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="48ccd-155">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48ccd-155">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="48ccd-156">Verwendung</span><span class="sxs-lookup"><span data-stu-id="48ccd-156">Usage</span></span>

<span data-ttu-id="48ccd-157">Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="48ccd-157">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="48ccd-158">Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="48ccd-158">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="48ccd-159">Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="48ccd-159">Here is an example of a chart image returned with the default parameters.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="48ccd-161">Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an.</span><span class="sxs-lookup"><span data-stu-id="48ccd-161">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="48ccd-162">So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="48ccd-162">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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

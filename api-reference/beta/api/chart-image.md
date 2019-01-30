---
title: 'Diagramm: Bild'
description: Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5892864d8adb94c4c6193dc4776f8febd938ff36
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642842"
---
# <a name="chart-image"></a><span data-ttu-id="b7c7c-103">Diagramm: Bild</span><span class="sxs-lookup"><span data-stu-id="b7c7c-103">Chart: Image</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7c7c-104">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7c7c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b7c7c-105">Permissions</span></span>
<span data-ttu-id="b7c7c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7c7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c7c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7c7c-108">Permission type</span></span>      | <span data-ttu-id="b7c7c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7c7c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7c7c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7c7c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7c7c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c7c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7c7c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7c7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7c7c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c7c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7c7c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7c7c-114">Application</span></span> | <span data-ttu-id="b7c7c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7c7c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7c7c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7c7c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="b7c7c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7c7c-117">Request headers</span></span>
| <span data-ttu-id="b7c7c-118">Name</span><span class="sxs-lookup"><span data-stu-id="b7c7c-118">Name</span></span>       | <span data-ttu-id="b7c7c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7c7c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7c7c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c7c-120">Authorization</span></span>  | <span data-ttu-id="b7c7c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7c7c-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b7c7c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b7c7c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7c7c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b7c7c-126">Request body</span></span>
<span data-ttu-id="b7c7c-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7c7c-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="b7c7c-128">Parameter</span></span>    | <span data-ttu-id="b7c7c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b7c7c-129">Type</span></span>   |<span data-ttu-id="b7c7c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7c7c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7c7c-131">height</span><span class="sxs-lookup"><span data-stu-id="b7c7c-131">height</span></span>|<span data-ttu-id="b7c7c-132">number</span><span class="sxs-lookup"><span data-stu-id="b7c7c-132">number</span></span>|<span data-ttu-id="b7c7c-p104">Optional. Die gewünschte Höhe des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="b7c7c-135">width</span><span class="sxs-lookup"><span data-stu-id="b7c7c-135">width</span></span>|<span data-ttu-id="b7c7c-136">number</span><span class="sxs-lookup"><span data-stu-id="b7c7c-136">number</span></span>|<span data-ttu-id="b7c7c-p105">Optional. Die gewünschte Breite des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="b7c7c-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="b7c7c-139">fittingMode</span></span>|<span data-ttu-id="b7c7c-140">string</span><span class="sxs-lookup"><span data-stu-id="b7c7c-140">string</span></span>|<span data-ttu-id="b7c7c-p106">Optional. Die Methode, die verwendet wird, um das Diagramm auf die angegebenen Maße zu skalieren (wenn Höhe und Breite festgelegt sind).  Mögliche Werte: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="b7c7c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7c7c-144">Response</span></span>

<span data-ttu-id="b7c7c-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine base64-Bildzeichenfolge im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-145">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c7c-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7c7c-146">Example</span></span>
<span data-ttu-id="b7c7c-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7c7c-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7c7c-148">Request</span></span>
<span data-ttu-id="b7c7c-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-149">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="b7c7c-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7c7c-150">Response</span></span>
<span data-ttu-id="b7c7c-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-151">Here is an example of the response.</span></span> <span data-ttu-id="b7c7c-152">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b7c7c-153">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-153">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="b7c7c-154">Verwendung</span><span class="sxs-lookup"><span data-stu-id="b7c7c-154">Usage</span></span>

<span data-ttu-id="b7c7c-155">Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-155">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="b7c7c-156">Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-156">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="b7c7c-157">Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-157">Here is an example of a chart image returned with the default parameters.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="b7c7c-159">Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-159">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="b7c7c-160">So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="b7c7c-160">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-image.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

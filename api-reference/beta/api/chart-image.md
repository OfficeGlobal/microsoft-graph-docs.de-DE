---
title: 'Diagramm: Bild'
description: Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5ee56b38ca75162a760be54e58dacb6ced6bbc16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976408"
---
# <a name="chart-image"></a><span data-ttu-id="49a20-103">Diagramm: Bild</span><span class="sxs-lookup"><span data-stu-id="49a20-103">Chart: Image</span></span>

> <span data-ttu-id="49a20-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="49a20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49a20-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49a20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49a20-106">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="49a20-106">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="49a20-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="49a20-107">Permissions</span></span>
<span data-ttu-id="49a20-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49a20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49a20-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49a20-110">Permission type</span></span>      | <span data-ttu-id="49a20-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49a20-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49a20-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49a20-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49a20-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49a20-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49a20-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49a20-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49a20-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49a20-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49a20-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49a20-116">Application</span></span> | <span data-ttu-id="49a20-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49a20-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49a20-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49a20-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="49a20-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49a20-119">Request headers</span></span>
| <span data-ttu-id="49a20-120">Name</span><span class="sxs-lookup"><span data-stu-id="49a20-120">Name</span></span>       | <span data-ttu-id="49a20-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49a20-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49a20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49a20-122">Authorization</span></span>  | <span data-ttu-id="49a20-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49a20-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49a20-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="49a20-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="49a20-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="49a20-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49a20-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49a20-128">Request body</span></span>
<span data-ttu-id="49a20-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="49a20-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49a20-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="49a20-130">Parameter</span></span>    | <span data-ttu-id="49a20-131">Typ</span><span class="sxs-lookup"><span data-stu-id="49a20-131">Type</span></span>   |<span data-ttu-id="49a20-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49a20-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49a20-133">height</span><span class="sxs-lookup"><span data-stu-id="49a20-133">height</span></span>|<span data-ttu-id="49a20-134">number</span><span class="sxs-lookup"><span data-stu-id="49a20-134">number</span></span>|<span data-ttu-id="49a20-p105">Optional. Die gewünschte Höhe des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="49a20-p105">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="49a20-137">width</span><span class="sxs-lookup"><span data-stu-id="49a20-137">width</span></span>|<span data-ttu-id="49a20-138">number</span><span class="sxs-lookup"><span data-stu-id="49a20-138">number</span></span>|<span data-ttu-id="49a20-p106">Optional. Die gewünschte Breite des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="49a20-p106">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="49a20-141">fittingMode</span><span class="sxs-lookup"><span data-stu-id="49a20-141">fittingMode</span></span>|<span data-ttu-id="49a20-142">string</span><span class="sxs-lookup"><span data-stu-id="49a20-142">string</span></span>|<span data-ttu-id="49a20-p107">Optional. Die Methode, die verwendet wird, um das Diagramm auf die angegebenen Maße zu skalieren (wenn Höhe und Breite festgelegt sind).  Mögliche Werte: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="49a20-p107">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="49a20-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="49a20-146">Response</span></span>

<span data-ttu-id="49a20-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine base64-Bildzeichenfolge im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49a20-147">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49a20-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49a20-148">Example</span></span>
<span data-ttu-id="49a20-149">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="49a20-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49a20-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49a20-150">Request</span></span>
<span data-ttu-id="49a20-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49a20-151">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="49a20-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="49a20-152">Response</span></span>
<span data-ttu-id="49a20-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="49a20-153">Here is an example of the response.</span></span> <span data-ttu-id="49a20-154">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="49a20-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="49a20-155">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49a20-155">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="49a20-156">Verwendung</span><span class="sxs-lookup"><span data-stu-id="49a20-156">Usage</span></span>

<span data-ttu-id="49a20-157">Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="49a20-157">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="49a20-158">Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="49a20-158">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="49a20-159">Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="49a20-159">Here is an example of a chart image returned with the default parameters.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="49a20-161">Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an.</span><span class="sxs-lookup"><span data-stu-id="49a20-161">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="49a20-162">So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="49a20-162">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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

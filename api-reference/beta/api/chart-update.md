---
title: Diagramm aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des Diagrammobjekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 98db5ec8a3425d75aa73eb9f705b64621982a373
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956794"
---
# <a name="update-chart"></a><span data-ttu-id="2a90f-103">Diagramm aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a90f-103">Update chart</span></span>

> <span data-ttu-id="2a90f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2a90f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a90f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a90f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a90f-106">Dient zum Aktualisieren der Eigenschaften des Diagrammobjekts.</span><span class="sxs-lookup"><span data-stu-id="2a90f-106">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a90f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a90f-107">Permissions</span></span>
<span data-ttu-id="2a90f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a90f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a90f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a90f-110">Permission type</span></span>      | <span data-ttu-id="2a90f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a90f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a90f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a90f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a90f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a90f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2a90f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a90f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a90f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a90f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2a90f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a90f-116">Application</span></span> | <span data-ttu-id="2a90f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a90f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a90f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a90f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="2a90f-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a90f-119">Optional request headers</span></span>
| <span data-ttu-id="2a90f-120">Name</span><span class="sxs-lookup"><span data-stu-id="2a90f-120">Name</span></span>       | <span data-ttu-id="2a90f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a90f-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2a90f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a90f-122">Authorization</span></span>  | <span data-ttu-id="2a90f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a90f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a90f-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2a90f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2a90f-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2a90f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a90f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a90f-128">Request body</span></span>
<span data-ttu-id="2a90f-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="2a90f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2a90f-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a90f-132">Property</span></span>     | <span data-ttu-id="2a90f-133">Typ</span><span class="sxs-lookup"><span data-stu-id="2a90f-133">Type</span></span>   |<span data-ttu-id="2a90f-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a90f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a90f-135">height</span><span class="sxs-lookup"><span data-stu-id="2a90f-135">height</span></span>|<span data-ttu-id="2a90f-136">double</span><span class="sxs-lookup"><span data-stu-id="2a90f-136">double</span></span>|<span data-ttu-id="2a90f-137">Die Höhe des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="2a90f-137">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="2a90f-138">left</span><span class="sxs-lookup"><span data-stu-id="2a90f-138">left</span></span>|<span data-ttu-id="2a90f-139">double</span><span class="sxs-lookup"><span data-stu-id="2a90f-139">double</span></span>|<span data-ttu-id="2a90f-140">Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="2a90f-140">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="2a90f-141">name</span><span class="sxs-lookup"><span data-stu-id="2a90f-141">name</span></span>|<span data-ttu-id="2a90f-142">string</span><span class="sxs-lookup"><span data-stu-id="2a90f-142">string</span></span>|<span data-ttu-id="2a90f-143">Gibt den Namen eines Diagrammobjekts an.</span><span class="sxs-lookup"><span data-stu-id="2a90f-143">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="2a90f-144">top</span><span class="sxs-lookup"><span data-stu-id="2a90f-144">top</span></span>|<span data-ttu-id="2a90f-145">double</span><span class="sxs-lookup"><span data-stu-id="2a90f-145">double</span></span>|<span data-ttu-id="2a90f-146">Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).</span><span class="sxs-lookup"><span data-stu-id="2a90f-146">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="2a90f-147">width</span><span class="sxs-lookup"><span data-stu-id="2a90f-147">width</span></span>|<span data-ttu-id="2a90f-148">double</span><span class="sxs-lookup"><span data-stu-id="2a90f-148">double</span></span>|<span data-ttu-id="2a90f-149">Die Breite des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="2a90f-149">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="2a90f-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a90f-150">Response</span></span>

<span data-ttu-id="2a90f-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a90f-151">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2a90f-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a90f-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a90f-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a90f-153">Request</span></span>
<span data-ttu-id="2a90f-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a90f-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="2a90f-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a90f-155">Response</span></span>
<span data-ttu-id="2a90f-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a90f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

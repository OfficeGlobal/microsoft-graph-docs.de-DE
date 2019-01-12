---
title: Diagramm aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des Diagrammobjekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 03a375e874a06914f5da9039dad58079df1199a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986320"
---
# <a name="update-chart"></a><span data-ttu-id="d6655-103">Diagramm aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d6655-103">Update chart</span></span>

<span data-ttu-id="d6655-104">Dient zum Aktualisieren der Eigenschaften des Diagrammobjekts.</span><span class="sxs-lookup"><span data-stu-id="d6655-104">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6655-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d6655-105">Permissions</span></span>
<span data-ttu-id="d6655-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6655-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6655-108">Permission type</span></span>      | <span data-ttu-id="d6655-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6655-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6655-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6655-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6655-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6655-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d6655-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6655-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6655-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6655-113">Not supported.</span></span>    |
|<span data-ttu-id="d6655-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6655-114">Application</span></span> | <span data-ttu-id="d6655-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6655-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6655-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6655-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d6655-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6655-117">Optional request headers</span></span>
| <span data-ttu-id="d6655-118">Name</span><span class="sxs-lookup"><span data-stu-id="d6655-118">Name</span></span>       | <span data-ttu-id="d6655-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6655-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d6655-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6655-120">Authorization</span></span>  | <span data-ttu-id="d6655-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d6655-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6655-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="d6655-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d6655-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="d6655-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6655-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6655-126">Request body</span></span>
<span data-ttu-id="d6655-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="d6655-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d6655-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6655-130">Property</span></span>     | <span data-ttu-id="d6655-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d6655-131">Type</span></span>   |<span data-ttu-id="d6655-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6655-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6655-133">height</span><span class="sxs-lookup"><span data-stu-id="d6655-133">height</span></span>|<span data-ttu-id="d6655-134">double</span><span class="sxs-lookup"><span data-stu-id="d6655-134">double</span></span>|<span data-ttu-id="d6655-135">Die Höhe des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="d6655-135">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="d6655-136">left</span><span class="sxs-lookup"><span data-stu-id="d6655-136">left</span></span>|<span data-ttu-id="d6655-137">double</span><span class="sxs-lookup"><span data-stu-id="d6655-137">double</span></span>|<span data-ttu-id="d6655-138">Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="d6655-138">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="d6655-139">name</span><span class="sxs-lookup"><span data-stu-id="d6655-139">name</span></span>|<span data-ttu-id="d6655-140">string</span><span class="sxs-lookup"><span data-stu-id="d6655-140">string</span></span>|<span data-ttu-id="d6655-141">Gibt den Namen eines Diagrammobjekts an.</span><span class="sxs-lookup"><span data-stu-id="d6655-141">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="d6655-142">top</span><span class="sxs-lookup"><span data-stu-id="d6655-142">top</span></span>|<span data-ttu-id="d6655-143">double</span><span class="sxs-lookup"><span data-stu-id="d6655-143">double</span></span>|<span data-ttu-id="d6655-144">Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).</span><span class="sxs-lookup"><span data-stu-id="d6655-144">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="d6655-145">width</span><span class="sxs-lookup"><span data-stu-id="d6655-145">width</span></span>|<span data-ttu-id="d6655-146">double</span><span class="sxs-lookup"><span data-stu-id="d6655-146">double</span></span>|<span data-ttu-id="d6655-147">Die Breite des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="d6655-147">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="d6655-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6655-148">Response</span></span>

<span data-ttu-id="d6655-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookChart](../resources/chart.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d6655-149">If successful, this method returns a `200 OK` response code and updated [WorkbookChart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6655-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6655-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6655-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6655-151">Request</span></span>
<span data-ttu-id="d6655-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6655-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="d6655-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6655-153">Response</span></span>
<span data-ttu-id="d6655-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6655-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
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

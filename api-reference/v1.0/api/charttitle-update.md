---
title: ChartTitle aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 08feb358af9ee67dda6f7da37b10c9788b83a224
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976877"
---
# <a name="update-charttitle"></a><span data-ttu-id="be5f0-103">ChartTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="be5f0-103">Update charttitle</span></span>

<span data-ttu-id="be5f0-104">Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="be5f0-104">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be5f0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be5f0-105">Permissions</span></span>
<span data-ttu-id="be5f0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be5f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be5f0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be5f0-108">Permission type</span></span>      | <span data-ttu-id="be5f0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be5f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be5f0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be5f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be5f0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be5f0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be5f0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be5f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be5f0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be5f0-113">Not supported.</span></span>    |
|<span data-ttu-id="be5f0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be5f0-114">Application</span></span> | <span data-ttu-id="be5f0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be5f0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be5f0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be5f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="be5f0-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be5f0-117">Optional request headers</span></span>
| <span data-ttu-id="be5f0-118">Name</span><span class="sxs-lookup"><span data-stu-id="be5f0-118">Name</span></span>       | <span data-ttu-id="be5f0-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be5f0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="be5f0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="be5f0-120">Authorization</span></span>  | <span data-ttu-id="be5f0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="be5f0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be5f0-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="be5f0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="be5f0-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="be5f0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be5f0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be5f0-126">Request body</span></span>
<span data-ttu-id="be5f0-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="be5f0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="be5f0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be5f0-130">Property</span></span>     | <span data-ttu-id="be5f0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="be5f0-131">Type</span></span>   |<span data-ttu-id="be5f0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be5f0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be5f0-133">Overlay</span><span class="sxs-lookup"><span data-stu-id="be5f0-133">overlay</span></span>|<span data-ttu-id="be5f0-134">boolean</span><span class="sxs-lookup"><span data-stu-id="be5f0-134">boolean</span></span>|<span data-ttu-id="be5f0-135">Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.</span><span class="sxs-lookup"><span data-stu-id="be5f0-135">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="be5f0-136">text</span><span class="sxs-lookup"><span data-stu-id="be5f0-136">text</span></span>|<span data-ttu-id="be5f0-137">string</span><span class="sxs-lookup"><span data-stu-id="be5f0-137">string</span></span>|<span data-ttu-id="be5f0-138">Stellt den Titeltext eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="be5f0-138">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="be5f0-139">visible</span><span class="sxs-lookup"><span data-stu-id="be5f0-139">visible</span></span>|<span data-ttu-id="be5f0-140">boolean</span><span class="sxs-lookup"><span data-stu-id="be5f0-140">boolean</span></span>|<span data-ttu-id="be5f0-141">Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="be5f0-141">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="be5f0-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="be5f0-142">Response</span></span>

<span data-ttu-id="be5f0-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookChartTitle](../resources/charttitle.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be5f0-143">If successful, this method returns a `200 OK` response code and updated [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be5f0-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be5f0-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be5f0-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be5f0-145">Request</span></span>
<span data-ttu-id="be5f0-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be5f0-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="be5f0-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="be5f0-147">Response</span></span>
<span data-ttu-id="be5f0-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be5f0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

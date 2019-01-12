---
title: ChartLineFormat aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartLineFormat-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fac999f0c238d7b0769ae95238d452786556a1de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922697"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="a8cbc-103">ChartLineFormat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a8cbc-103">Update chartlineformat</span></span>

<span data-ttu-id="a8cbc-104">Dient zum Aktualisieren der Eigenschaften des ChartLineFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-104">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8cbc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8cbc-105">Permissions</span></span>
<span data-ttu-id="a8cbc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8cbc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8cbc-108">Permission type</span></span>      | <span data-ttu-id="a8cbc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8cbc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8cbc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8cbc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8cbc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8cbc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8cbc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8cbc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8cbc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8cbc-113">Not supported.</span></span>    |
|<span data-ttu-id="a8cbc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8cbc-114">Application</span></span> | <span data-ttu-id="a8cbc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8cbc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8cbc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8cbc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="a8cbc-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8cbc-117">Optional request headers</span></span>
| <span data-ttu-id="a8cbc-118">Name</span><span class="sxs-lookup"><span data-stu-id="a8cbc-118">Name</span></span>       | <span data-ttu-id="a8cbc-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8cbc-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a8cbc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8cbc-120">Authorization</span></span>  | <span data-ttu-id="a8cbc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8cbc-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a8cbc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a8cbc-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8cbc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8cbc-126">Request body</span></span>
<span data-ttu-id="a8cbc-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a8cbc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8cbc-130">Property</span></span>     | <span data-ttu-id="a8cbc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a8cbc-131">Type</span></span>   |<span data-ttu-id="a8cbc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8cbc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8cbc-133">color</span><span class="sxs-lookup"><span data-stu-id="a8cbc-133">color</span></span>|<span data-ttu-id="a8cbc-134">string</span><span class="sxs-lookup"><span data-stu-id="a8cbc-134">string</span></span>|<span data-ttu-id="a8cbc-135">HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-135">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="a8cbc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8cbc-136">Response</span></span>

<span data-ttu-id="a8cbc-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookChartLineFormat](../resources/chartlineformat.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8cbc-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8cbc-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8cbc-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8cbc-139">Request</span></span>
<span data-ttu-id="a8cbc-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="a8cbc-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8cbc-141">Response</span></span>
<span data-ttu-id="a8cbc-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

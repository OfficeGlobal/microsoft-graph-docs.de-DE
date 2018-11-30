---
title: ChartAxis aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartAxis-Objekts.
ms.openlocfilehash: 665c20683c2a2f54d4f5e73a66993707bc5f6539
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017633"
---
# <a name="update-chartaxis"></a><span data-ttu-id="afe3c-103">ChartAxis aktualisieren</span><span class="sxs-lookup"><span data-stu-id="afe3c-103">Update chartaxis</span></span>

<span data-ttu-id="afe3c-104">Dient zum Aktualisieren der Eigenschaften des ChartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="afe3c-104">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="afe3c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="afe3c-105">Permissions</span></span>
<span data-ttu-id="afe3c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afe3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe3c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="afe3c-108">Permission type</span></span>      | <span data-ttu-id="afe3c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="afe3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afe3c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="afe3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afe3c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afe3c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="afe3c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="afe3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afe3c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afe3c-113">Not supported.</span></span>    |
|<span data-ttu-id="afe3c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="afe3c-114">Application</span></span> | <span data-ttu-id="afe3c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afe3c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afe3c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afe3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="afe3c-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afe3c-117">Optional request headers</span></span>
| <span data-ttu-id="afe3c-118">Name</span><span class="sxs-lookup"><span data-stu-id="afe3c-118">Name</span></span>       | <span data-ttu-id="afe3c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afe3c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="afe3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="afe3c-120">Authorization</span></span>  | <span data-ttu-id="afe3c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="afe3c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="afe3c-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="afe3c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="afe3c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="afe3c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afe3c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="afe3c-126">Request body</span></span>
<span data-ttu-id="afe3c-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="afe3c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="afe3c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="afe3c-130">Property</span></span>     | <span data-ttu-id="afe3c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="afe3c-131">Type</span></span>   |<span data-ttu-id="afe3c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afe3c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afe3c-133">majorUnit</span><span class="sxs-lookup"><span data-stu-id="afe3c-133">majorUnit</span></span>|<span data-ttu-id="afe3c-134">Json</span><span class="sxs-lookup"><span data-stu-id="afe3c-134">Json</span></span>|<span data-ttu-id="afe3c-p105">Stellt das Intervall zwischen zwei Hauptteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden.  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="afe3c-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="afe3c-138">maximum</span><span class="sxs-lookup"><span data-stu-id="afe3c-138">maximum</span></span>|<span data-ttu-id="afe3c-139">Json</span><span class="sxs-lookup"><span data-stu-id="afe3c-139">Json</span></span>|<span data-ttu-id="afe3c-p106">Stellt den Maximalwert auf der Größenachse dar.  Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="afe3c-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="afe3c-143">minimum</span><span class="sxs-lookup"><span data-stu-id="afe3c-143">minimum</span></span>|<span data-ttu-id="afe3c-144">Json</span><span class="sxs-lookup"><span data-stu-id="afe3c-144">Json</span></span>|<span data-ttu-id="afe3c-p107">Stellt den Mindestwert auf der Größenachse dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="afe3c-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="afe3c-148">minorUnit</span><span class="sxs-lookup"><span data-stu-id="afe3c-148">minorUnit</span></span>|<span data-ttu-id="afe3c-149">Json</span><span class="sxs-lookup"><span data-stu-id="afe3c-149">Json</span></span>|<span data-ttu-id="afe3c-p108">Stellt das Intervall zwischen zwei Hilfsteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte). Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="afe3c-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="afe3c-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="afe3c-153">Response</span></span>

<span data-ttu-id="afe3c-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookChartAxis](../resources/chartaxis.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="afe3c-154">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afe3c-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afe3c-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afe3c-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afe3c-156">Request</span></span>
<span data-ttu-id="afe3c-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="afe3c-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
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
##### <a name="response"></a><span data-ttu-id="afe3c-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="afe3c-158">Response</span></span>
<span data-ttu-id="afe3c-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afe3c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxis"
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
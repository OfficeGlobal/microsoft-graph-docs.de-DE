---
title: ChartTitle aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.
ms.openlocfilehash: 4b6e4093c5abda12d7d4cd29bace743c7ec63b31
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020049"
---
# <a name="update-charttitle"></a><span data-ttu-id="45582-103">ChartTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="45582-103">Update charttitle</span></span>

<span data-ttu-id="45582-104">Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="45582-104">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="45582-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="45582-105">Permissions</span></span>
<span data-ttu-id="45582-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45582-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45582-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45582-108">Permission type</span></span>      | <span data-ttu-id="45582-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45582-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45582-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45582-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45582-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45582-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="45582-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45582-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45582-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45582-113">Not supported.</span></span>    |
|<span data-ttu-id="45582-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45582-114">Application</span></span> | <span data-ttu-id="45582-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45582-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45582-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45582-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="45582-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45582-117">Optional request headers</span></span>
| <span data-ttu-id="45582-118">Name</span><span class="sxs-lookup"><span data-stu-id="45582-118">Name</span></span>       | <span data-ttu-id="45582-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45582-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="45582-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="45582-120">Authorization</span></span>  | <span data-ttu-id="45582-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45582-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45582-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="45582-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="45582-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="45582-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45582-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45582-126">Request body</span></span>
<span data-ttu-id="45582-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="45582-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="45582-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45582-130">Property</span></span>     | <span data-ttu-id="45582-131">Typ</span><span class="sxs-lookup"><span data-stu-id="45582-131">Type</span></span>   |<span data-ttu-id="45582-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45582-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45582-133">Overlay</span><span class="sxs-lookup"><span data-stu-id="45582-133">overlay</span></span>|<span data-ttu-id="45582-134">boolean</span><span class="sxs-lookup"><span data-stu-id="45582-134">boolean</span></span>|<span data-ttu-id="45582-135">Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.</span><span class="sxs-lookup"><span data-stu-id="45582-135">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="45582-136">text</span><span class="sxs-lookup"><span data-stu-id="45582-136">text</span></span>|<span data-ttu-id="45582-137">string</span><span class="sxs-lookup"><span data-stu-id="45582-137">string</span></span>|<span data-ttu-id="45582-138">Stellt den Titeltext eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="45582-138">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="45582-139">visible</span><span class="sxs-lookup"><span data-stu-id="45582-139">visible</span></span>|<span data-ttu-id="45582-140">boolean</span><span class="sxs-lookup"><span data-stu-id="45582-140">boolean</span></span>|<span data-ttu-id="45582-141">Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="45582-141">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="45582-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="45582-142">Response</span></span>

<span data-ttu-id="45582-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookChartTitle](../resources/charttitle.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="45582-143">If successful, this method returns a `200 OK` response code and updated [WorkbookChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45582-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45582-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45582-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45582-145">Request</span></span>
<span data-ttu-id="45582-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45582-146">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="45582-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="45582-147">Response</span></span>
<span data-ttu-id="45582-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45582-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
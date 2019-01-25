---
title: ChartLegend aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 83c46208edf769a2c3d3a97d242b874596d3308d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513501"
---
# <a name="update-chartlegend"></a><span data-ttu-id="77f64-103">ChartLegend aktualisieren</span><span class="sxs-lookup"><span data-stu-id="77f64-103">Update chartlegend</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77f64-104">Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="77f64-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="77f64-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="77f64-105">Permissions</span></span>
<span data-ttu-id="77f64-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77f64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77f64-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77f64-108">Permission type</span></span>      | <span data-ttu-id="77f64-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77f64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77f64-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77f64-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77f64-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77f64-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77f64-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77f64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77f64-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77f64-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77f64-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77f64-114">Application</span></span> | <span data-ttu-id="77f64-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77f64-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77f64-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77f64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="77f64-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77f64-117">Optional request headers</span></span>
| <span data-ttu-id="77f64-118">Name</span><span class="sxs-lookup"><span data-stu-id="77f64-118">Name</span></span>       | <span data-ttu-id="77f64-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77f64-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="77f64-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77f64-120">Authorization</span></span>  | <span data-ttu-id="77f64-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77f64-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77f64-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="77f64-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="77f64-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="77f64-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77f64-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77f64-126">Request body</span></span>
<span data-ttu-id="77f64-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="77f64-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="77f64-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77f64-130">Property</span></span>     | <span data-ttu-id="77f64-131">Typ</span><span class="sxs-lookup"><span data-stu-id="77f64-131">Type</span></span>   |<span data-ttu-id="77f64-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77f64-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f64-133">Overlay</span><span class="sxs-lookup"><span data-stu-id="77f64-133">overlay</span></span>|<span data-ttu-id="77f64-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77f64-134">boolean</span></span>|<span data-ttu-id="77f64-135">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="77f64-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="77f64-136">Position</span><span class="sxs-lookup"><span data-stu-id="77f64-136">position</span></span>|<span data-ttu-id="77f64-137">string</span><span class="sxs-lookup"><span data-stu-id="77f64-137">string</span></span>|<span data-ttu-id="77f64-p105">Gibt die Position der Legende im Diagramm an. Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="77f64-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="77f64-140">visible</span><span class="sxs-lookup"><span data-stu-id="77f64-140">visible</span></span>|<span data-ttu-id="77f64-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="77f64-141">boolean</span></span>|<span data-ttu-id="77f64-142">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="77f64-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="77f64-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="77f64-143">Response</span></span>

<span data-ttu-id="77f64-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartLegend](../resources/chartlegend.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77f64-144">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77f64-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77f64-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77f64-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77f64-146">Request</span></span>
<span data-ttu-id="77f64-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77f64-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="77f64-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="77f64-148">Response</span></span>
<span data-ttu-id="77f64-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77f64-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartlegend-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: ChartLegend aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 03bcd9ce5d5c15f624dd0eaa231f8965137c210e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946630"
---
# <a name="update-chartlegend"></a><span data-ttu-id="a102a-103">ChartLegend aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a102a-103">Update chartlegend</span></span>

> <span data-ttu-id="a102a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a102a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a102a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a102a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a102a-106">Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a102a-106">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a102a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a102a-107">Permissions</span></span>
<span data-ttu-id="a102a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a102a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a102a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a102a-110">Permission type</span></span>      | <span data-ttu-id="a102a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a102a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a102a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a102a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a102a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a102a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a102a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a102a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a102a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a102a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a102a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a102a-116">Application</span></span> | <span data-ttu-id="a102a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a102a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a102a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a102a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="a102a-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a102a-119">Optional request headers</span></span>
| <span data-ttu-id="a102a-120">Name</span><span class="sxs-lookup"><span data-stu-id="a102a-120">Name</span></span>       | <span data-ttu-id="a102a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a102a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a102a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a102a-122">Authorization</span></span>  | <span data-ttu-id="a102a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a102a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a102a-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a102a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a102a-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a102a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a102a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a102a-128">Request body</span></span>
<span data-ttu-id="a102a-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a102a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a102a-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a102a-132">Property</span></span>     | <span data-ttu-id="a102a-133">Typ</span><span class="sxs-lookup"><span data-stu-id="a102a-133">Type</span></span>   |<span data-ttu-id="a102a-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a102a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a102a-135">Overlay</span><span class="sxs-lookup"><span data-stu-id="a102a-135">overlay</span></span>|<span data-ttu-id="a102a-136">boolean</span><span class="sxs-lookup"><span data-stu-id="a102a-136">boolean</span></span>|<span data-ttu-id="a102a-137">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="a102a-137">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="a102a-138">Position</span><span class="sxs-lookup"><span data-stu-id="a102a-138">position</span></span>|<span data-ttu-id="a102a-139">string</span><span class="sxs-lookup"><span data-stu-id="a102a-139">string</span></span>|<span data-ttu-id="a102a-p106">Gibt die Position der Legende im Diagramm an. Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="a102a-p106">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="a102a-142">visible</span><span class="sxs-lookup"><span data-stu-id="a102a-142">visible</span></span>|<span data-ttu-id="a102a-143">boolean</span><span class="sxs-lookup"><span data-stu-id="a102a-143">boolean</span></span>|<span data-ttu-id="a102a-144">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="a102a-144">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="a102a-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="a102a-145">Response</span></span>

<span data-ttu-id="a102a-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartLegend](../resources/chartlegend.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a102a-146">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a102a-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a102a-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a102a-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a102a-148">Request</span></span>
<span data-ttu-id="a102a-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a102a-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a102a-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="a102a-150">Response</span></span>
<span data-ttu-id="a102a-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a102a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

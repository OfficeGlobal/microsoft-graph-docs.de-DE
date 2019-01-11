---
title: ChartLegend aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a5dae3bfc8244a0f622665d831c3081e1f0f432d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854635"
---
# <a name="update-chartlegend"></a><span data-ttu-id="f174e-103">ChartLegend aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f174e-103">Update chartlegend</span></span>

> <span data-ttu-id="f174e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f174e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f174e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f174e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f174e-106">Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f174e-106">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f174e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f174e-107">Permissions</span></span>
<span data-ttu-id="f174e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f174e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f174e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f174e-110">Permission type</span></span>      | <span data-ttu-id="f174e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f174e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f174e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f174e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f174e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f174e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f174e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f174e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f174e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f174e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f174e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f174e-116">Application</span></span> | <span data-ttu-id="f174e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f174e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f174e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f174e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="f174e-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f174e-119">Optional request headers</span></span>
| <span data-ttu-id="f174e-120">Name</span><span class="sxs-lookup"><span data-stu-id="f174e-120">Name</span></span>       | <span data-ttu-id="f174e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f174e-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f174e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f174e-122">Authorization</span></span>  | <span data-ttu-id="f174e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f174e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f174e-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="f174e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f174e-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="f174e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f174e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f174e-128">Request body</span></span>
<span data-ttu-id="f174e-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f174e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f174e-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f174e-132">Property</span></span>     | <span data-ttu-id="f174e-133">Typ</span><span class="sxs-lookup"><span data-stu-id="f174e-133">Type</span></span>   |<span data-ttu-id="f174e-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f174e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f174e-135">Overlay</span><span class="sxs-lookup"><span data-stu-id="f174e-135">overlay</span></span>|<span data-ttu-id="f174e-136">boolean</span><span class="sxs-lookup"><span data-stu-id="f174e-136">boolean</span></span>|<span data-ttu-id="f174e-137">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="f174e-137">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="f174e-138">Position</span><span class="sxs-lookup"><span data-stu-id="f174e-138">position</span></span>|<span data-ttu-id="f174e-139">string</span><span class="sxs-lookup"><span data-stu-id="f174e-139">string</span></span>|<span data-ttu-id="f174e-p106">Gibt die Position der Legende im Diagramm an. Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="f174e-p106">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="f174e-142">visible</span><span class="sxs-lookup"><span data-stu-id="f174e-142">visible</span></span>|<span data-ttu-id="f174e-143">boolean</span><span class="sxs-lookup"><span data-stu-id="f174e-143">boolean</span></span>|<span data-ttu-id="f174e-144">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="f174e-144">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="f174e-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="f174e-145">Response</span></span>

<span data-ttu-id="f174e-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartLegend](../resources/chartlegend.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f174e-146">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f174e-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f174e-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f174e-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f174e-148">Request</span></span>
<span data-ttu-id="f174e-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f174e-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f174e-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="f174e-150">Response</span></span>
<span data-ttu-id="f174e-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f174e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

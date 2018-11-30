---
title: ChartLegend aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.
ms.openlocfilehash: 7eb89f40e0f691e597d519070997f90729d8a2f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058325"
---
# <a name="update-chartlegend"></a><span data-ttu-id="26f1f-103">ChartLegend aktualisieren</span><span class="sxs-lookup"><span data-stu-id="26f1f-103">Update chartlegend</span></span>

> <span data-ttu-id="26f1f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="26f1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26f1f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26f1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26f1f-106">Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="26f1f-106">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="26f1f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="26f1f-107">Permissions</span></span>
<span data-ttu-id="26f1f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26f1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26f1f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26f1f-110">Permission type</span></span>      | <span data-ttu-id="26f1f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26f1f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26f1f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26f1f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26f1f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26f1f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26f1f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26f1f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26f1f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26f1f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26f1f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26f1f-116">Application</span></span> | <span data-ttu-id="26f1f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26f1f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26f1f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26f1f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="26f1f-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26f1f-119">Optional request headers</span></span>
| <span data-ttu-id="26f1f-120">Name</span><span class="sxs-lookup"><span data-stu-id="26f1f-120">Name</span></span>       | <span data-ttu-id="26f1f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26f1f-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="26f1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26f1f-122">Authorization</span></span>  | <span data-ttu-id="26f1f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="26f1f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26f1f-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="26f1f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="26f1f-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="26f1f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26f1f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26f1f-128">Request body</span></span>
<span data-ttu-id="26f1f-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="26f1f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26f1f-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26f1f-132">Property</span></span>     | <span data-ttu-id="26f1f-133">Typ</span><span class="sxs-lookup"><span data-stu-id="26f1f-133">Type</span></span>   |<span data-ttu-id="26f1f-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26f1f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26f1f-135">Overlay</span><span class="sxs-lookup"><span data-stu-id="26f1f-135">overlay</span></span>|<span data-ttu-id="26f1f-136">boolean</span><span class="sxs-lookup"><span data-stu-id="26f1f-136">boolean</span></span>|<span data-ttu-id="26f1f-137">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="26f1f-137">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="26f1f-138">Position</span><span class="sxs-lookup"><span data-stu-id="26f1f-138">position</span></span>|<span data-ttu-id="26f1f-139">string</span><span class="sxs-lookup"><span data-stu-id="26f1f-139">string</span></span>|<span data-ttu-id="26f1f-p106">Gibt die Position der Legende im Diagramm an. Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="26f1f-p106">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="26f1f-142">visible</span><span class="sxs-lookup"><span data-stu-id="26f1f-142">visible</span></span>|<span data-ttu-id="26f1f-143">boolean</span><span class="sxs-lookup"><span data-stu-id="26f1f-143">boolean</span></span>|<span data-ttu-id="26f1f-144">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="26f1f-144">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="26f1f-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="26f1f-145">Response</span></span>

<span data-ttu-id="26f1f-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartLegend](../resources/chartlegend.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26f1f-146">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26f1f-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26f1f-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26f1f-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26f1f-148">Request</span></span>
<span data-ttu-id="26f1f-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26f1f-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="26f1f-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="26f1f-150">Response</span></span>
<span data-ttu-id="26f1f-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26f1f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
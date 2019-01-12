---
title: 'ChartCollection: add'
description: Erstellt ein neues Diagramm.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 19ab5936b563fc491e08923d257d334d9932af98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936578"
---
# <a name="chartcollection-add"></a><span data-ttu-id="04b58-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="04b58-103">ChartCollection: add</span></span>

> <span data-ttu-id="04b58-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="04b58-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04b58-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04b58-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04b58-106">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="04b58-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="04b58-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="04b58-107">Permissions</span></span>
<span data-ttu-id="04b58-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b58-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04b58-110">Permission type</span></span>      | <span data-ttu-id="04b58-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04b58-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04b58-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04b58-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04b58-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04b58-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="04b58-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04b58-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04b58-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04b58-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="04b58-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04b58-116">Application</span></span> | <span data-ttu-id="04b58-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04b58-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04b58-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04b58-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="04b58-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04b58-119">Request headers</span></span>
| <span data-ttu-id="04b58-120">Name</span><span class="sxs-lookup"><span data-stu-id="04b58-120">Name</span></span>       | <span data-ttu-id="04b58-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04b58-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04b58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04b58-122">Authorization</span></span>  | <span data-ttu-id="04b58-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04b58-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04b58-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="04b58-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="04b58-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="04b58-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b58-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04b58-128">Request body</span></span>
<span data-ttu-id="04b58-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="04b58-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04b58-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="04b58-130">Parameter</span></span>    | <span data-ttu-id="04b58-131">Typ</span><span class="sxs-lookup"><span data-stu-id="04b58-131">Type</span></span>   |<span data-ttu-id="04b58-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04b58-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04b58-133">type</span><span class="sxs-lookup"><span data-stu-id="04b58-133">type</span></span>|<span data-ttu-id="04b58-134">string</span><span class="sxs-lookup"><span data-stu-id="04b58-134">string</span></span>|<span data-ttu-id="04b58-p105">Stellt die Art des Diagramms dar.  Mögliche Werte: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="04b58-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="04b58-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="04b58-137">sourceData</span></span>|<span data-ttu-id="04b58-138">string</span><span class="sxs-lookup"><span data-stu-id="04b58-138">string</span></span>|<span data-ttu-id="04b58-139">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="04b58-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="04b58-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="04b58-140">seriesBy</span></span>|<span data-ttu-id="04b58-141">string</span><span class="sxs-lookup"><span data-stu-id="04b58-141">string</span></span>|<span data-ttu-id="04b58-p106">Optional. Gibt an, wie Spalten oder Zeilen als Datenreihen im Diagramm verwendet werden.  Mögliche Werte: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="04b58-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="04b58-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="04b58-145">Response</span></span>

<span data-ttu-id="04b58-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04b58-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04b58-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04b58-147">Example</span></span>
<span data-ttu-id="04b58-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="04b58-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="04b58-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04b58-149">Request</span></span>
<span data-ttu-id="04b58-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04b58-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="04b58-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="04b58-151">Response</span></span>
<span data-ttu-id="04b58-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04b58-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

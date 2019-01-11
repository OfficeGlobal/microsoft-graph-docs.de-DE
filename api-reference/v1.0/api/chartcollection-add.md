---
title: 'ChartCollection: add'
description: Erstellt ein neues Diagramm.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4aa1a017da88fdd06b8e396130d5b09fbbeaebb5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867942"
---
# <a name="chartcollection-add"></a><span data-ttu-id="d810a-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="d810a-103">ChartCollection: add</span></span>

<span data-ttu-id="d810a-104">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="d810a-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="d810a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d810a-105">Permissions</span></span>
<span data-ttu-id="d810a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d810a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d810a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d810a-108">Permission type</span></span>      | <span data-ttu-id="d810a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d810a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d810a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d810a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d810a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d810a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d810a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d810a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d810a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d810a-113">Not supported.</span></span>    |
|<span data-ttu-id="d810a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d810a-114">Application</span></span> | <span data-ttu-id="d810a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d810a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d810a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d810a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="d810a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d810a-117">Request headers</span></span>
| <span data-ttu-id="d810a-118">Name</span><span class="sxs-lookup"><span data-stu-id="d810a-118">Name</span></span>       | <span data-ttu-id="d810a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d810a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d810a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d810a-120">Authorization</span></span>  | <span data-ttu-id="d810a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d810a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d810a-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="d810a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d810a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="d810a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d810a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d810a-126">Request body</span></span>
<span data-ttu-id="d810a-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d810a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d810a-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="d810a-128">Parameter</span></span>    | <span data-ttu-id="d810a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d810a-129">Type</span></span>   |<span data-ttu-id="d810a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d810a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d810a-131">type</span><span class="sxs-lookup"><span data-stu-id="d810a-131">type</span></span>|<span data-ttu-id="d810a-132">string</span><span class="sxs-lookup"><span data-stu-id="d810a-132">string</span></span>|<span data-ttu-id="d810a-133">Stellt den Typ eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="d810a-133">Represents the type of a chart.</span></span>  <span data-ttu-id="d810a-134">Die möglichen Werte sind: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="d810a-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="d810a-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="d810a-135">sourceData</span></span>|<span data-ttu-id="d810a-136">Json</span><span class="sxs-lookup"><span data-stu-id="d810a-136">Json</span></span>|<span data-ttu-id="d810a-137">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d810a-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="d810a-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="d810a-138">seriesBy</span></span>|<span data-ttu-id="d810a-139">string</span><span class="sxs-lookup"><span data-stu-id="d810a-139">string</span></span>|<span data-ttu-id="d810a-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="d810a-140">Optional.</span></span> <span data-ttu-id="d810a-141">Gibt an, dass die Möglichkeit Spalten und Zeilen als Datenreihen im Diagramm verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d810a-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="d810a-142">Die möglichen Werte sind: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="d810a-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="d810a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="d810a-143">Response</span></span>

<span data-ttu-id="d810a-144">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookChart](../resources/chart.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d810a-144">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d810a-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d810a-145">Example</span></span>
<span data-ttu-id="d810a-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="d810a-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d810a-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d810a-147">Request</span></span>
<span data-ttu-id="d810a-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d810a-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="d810a-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="d810a-149">Response</span></span>
<span data-ttu-id="d810a-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d810a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

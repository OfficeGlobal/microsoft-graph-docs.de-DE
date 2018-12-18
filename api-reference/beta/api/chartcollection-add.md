---
title: 'ChartCollection: add'
description: Erstellt ein neues Diagramm.
author: lumine2008
ms.openlocfilehash: 704afc9890e3921c69cdd7b746c0e362c4627511
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325550"
---
# <a name="chartcollection-add"></a><span data-ttu-id="c179c-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="c179c-103">ChartCollection: add</span></span>

> <span data-ttu-id="c179c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c179c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c179c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c179c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c179c-106">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="c179c-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="c179c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c179c-107">Permissions</span></span>
<span data-ttu-id="c179c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c179c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c179c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c179c-110">Permission type</span></span>      | <span data-ttu-id="c179c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c179c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c179c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c179c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c179c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c179c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c179c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c179c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c179c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c179c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c179c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c179c-116">Application</span></span> | <span data-ttu-id="c179c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c179c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c179c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c179c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="c179c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c179c-119">Request headers</span></span>
| <span data-ttu-id="c179c-120">Name</span><span class="sxs-lookup"><span data-stu-id="c179c-120">Name</span></span>       | <span data-ttu-id="c179c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c179c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c179c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c179c-122">Authorization</span></span>  | <span data-ttu-id="c179c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c179c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c179c-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c179c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c179c-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c179c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c179c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c179c-128">Request body</span></span>
<span data-ttu-id="c179c-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c179c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c179c-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="c179c-130">Parameter</span></span>    | <span data-ttu-id="c179c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c179c-131">Type</span></span>   |<span data-ttu-id="c179c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c179c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c179c-133">type</span><span class="sxs-lookup"><span data-stu-id="c179c-133">type</span></span>|<span data-ttu-id="c179c-134">string</span><span class="sxs-lookup"><span data-stu-id="c179c-134">string</span></span>|<span data-ttu-id="c179c-p105">Stellt die Art des Diagramms dar.  Mögliche Werte: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="c179c-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="c179c-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="c179c-137">sourceData</span></span>|<span data-ttu-id="c179c-138">string</span><span class="sxs-lookup"><span data-stu-id="c179c-138">string</span></span>|<span data-ttu-id="c179c-139">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="c179c-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="c179c-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="c179c-140">seriesBy</span></span>|<span data-ttu-id="c179c-141">string</span><span class="sxs-lookup"><span data-stu-id="c179c-141">string</span></span>|<span data-ttu-id="c179c-p106">Optional. Gibt an, wie Spalten oder Zeilen als Datenreihen im Diagramm verwendet werden.  Mögliche Werte: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="c179c-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="c179c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="c179c-145">Response</span></span>

<span data-ttu-id="c179c-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c179c-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c179c-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c179c-147">Example</span></span>
<span data-ttu-id="c179c-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c179c-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c179c-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c179c-149">Request</span></span>
<span data-ttu-id="c179c-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c179c-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c179c-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c179c-151">Response</span></span>
<span data-ttu-id="c179c-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c179c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

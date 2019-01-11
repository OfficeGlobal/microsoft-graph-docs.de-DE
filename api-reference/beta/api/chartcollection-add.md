---
title: 'ChartCollection: add'
description: Erstellt ein neues Diagramm.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 51ad28568abe7445a85f813698736130f04ac48e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892421"
---
# <a name="chartcollection-add"></a><span data-ttu-id="d7ff4-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="d7ff4-103">ChartCollection: add</span></span>

> <span data-ttu-id="d7ff4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7ff4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7ff4-106">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7ff4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7ff4-107">Permissions</span></span>
<span data-ttu-id="d7ff4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7ff4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7ff4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7ff4-110">Permission type</span></span>      | <span data-ttu-id="d7ff4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7ff4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7ff4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7ff4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7ff4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7ff4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7ff4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7ff4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7ff4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7ff4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7ff4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7ff4-116">Application</span></span> | <span data-ttu-id="d7ff4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7ff4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7ff4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7ff4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="d7ff4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7ff4-119">Request headers</span></span>
| <span data-ttu-id="d7ff4-120">Name</span><span class="sxs-lookup"><span data-stu-id="d7ff4-120">Name</span></span>       | <span data-ttu-id="d7ff4-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7ff4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7ff4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7ff4-122">Authorization</span></span>  | <span data-ttu-id="d7ff4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7ff4-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="d7ff4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7ff4-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7ff4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7ff4-128">Request body</span></span>
<span data-ttu-id="d7ff4-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d7ff4-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="d7ff4-130">Parameter</span></span>    | <span data-ttu-id="d7ff4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d7ff4-131">Type</span></span>   |<span data-ttu-id="d7ff4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7ff4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7ff4-133">type</span><span class="sxs-lookup"><span data-stu-id="d7ff4-133">type</span></span>|<span data-ttu-id="d7ff4-134">string</span><span class="sxs-lookup"><span data-stu-id="d7ff4-134">string</span></span>|<span data-ttu-id="d7ff4-p105">Stellt die Art des Diagramms dar.  Mögliche Werte: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="d7ff4-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="d7ff4-137">sourceData</span></span>|<span data-ttu-id="d7ff4-138">string</span><span class="sxs-lookup"><span data-stu-id="d7ff4-138">string</span></span>|<span data-ttu-id="d7ff4-139">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="d7ff4-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="d7ff4-140">seriesBy</span></span>|<span data-ttu-id="d7ff4-141">string</span><span class="sxs-lookup"><span data-stu-id="d7ff4-141">string</span></span>|<span data-ttu-id="d7ff4-p106">Optional. Gibt an, wie Spalten oder Zeilen als Datenreihen im Diagramm verwendet werden.  Mögliche Werte: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="d7ff4-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7ff4-145">Response</span></span>

<span data-ttu-id="d7ff4-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7ff4-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7ff4-147">Example</span></span>
<span data-ttu-id="d7ff4-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7ff4-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7ff4-149">Request</span></span>
<span data-ttu-id="d7ff4-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d7ff4-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7ff4-151">Response</span></span>
<span data-ttu-id="d7ff4-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7ff4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

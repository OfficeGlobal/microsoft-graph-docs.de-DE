---
title: 'ChartCollection: add'
description: Erstellt ein neues Diagramm.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cdb3ff01b0741f0f1a4a0bff22e3a8e3dc32335c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516336"
---
# <a name="chartcollection-add"></a><span data-ttu-id="8d8ca-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="8d8ca-103">ChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d8ca-104">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d8ca-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8d8ca-105">Permissions</span></span>
<span data-ttu-id="8d8ca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d8ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d8ca-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d8ca-108">Permission type</span></span>      | <span data-ttu-id="8d8ca-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d8ca-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d8ca-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d8ca-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d8ca-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d8ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d8ca-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d8ca-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d8ca-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d8ca-114">Application</span></span> | <span data-ttu-id="8d8ca-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d8ca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d8ca-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d8ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="8d8ca-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d8ca-117">Request headers</span></span>
| <span data-ttu-id="8d8ca-118">Name</span><span class="sxs-lookup"><span data-stu-id="8d8ca-118">Name</span></span>       | <span data-ttu-id="8d8ca-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d8ca-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d8ca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d8ca-120">Authorization</span></span>  | <span data-ttu-id="8d8ca-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d8ca-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8d8ca-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8d8ca-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d8ca-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d8ca-126">Request body</span></span>
<span data-ttu-id="8d8ca-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d8ca-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="8d8ca-128">Parameter</span></span>    | <span data-ttu-id="8d8ca-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8d8ca-129">Type</span></span>   |<span data-ttu-id="8d8ca-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d8ca-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d8ca-131">type</span><span class="sxs-lookup"><span data-stu-id="8d8ca-131">type</span></span>|<span data-ttu-id="8d8ca-132">string</span><span class="sxs-lookup"><span data-stu-id="8d8ca-132">string</span></span>|<span data-ttu-id="8d8ca-p104">Stellt die Art des Diagramms dar.  Mögliche Werte: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-p104">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="8d8ca-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="8d8ca-135">sourceData</span></span>|<span data-ttu-id="8d8ca-136">string</span><span class="sxs-lookup"><span data-stu-id="8d8ca-136">string</span></span>|<span data-ttu-id="8d8ca-137">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="8d8ca-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="8d8ca-138">seriesBy</span></span>|<span data-ttu-id="8d8ca-139">string</span><span class="sxs-lookup"><span data-stu-id="8d8ca-139">string</span></span>|<span data-ttu-id="8d8ca-p105">Optional. Gibt an, wie Spalten oder Zeilen als Datenreihen im Diagramm verwendet werden.  Mögliche Werte: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-p105">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="8d8ca-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d8ca-143">Response</span></span>

<span data-ttu-id="8d8ca-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-144">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d8ca-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d8ca-145">Example</span></span>
<span data-ttu-id="8d8ca-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d8ca-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d8ca-147">Request</span></span>
<span data-ttu-id="8d8ca-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8d8ca-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d8ca-149">Response</span></span>
<span data-ttu-id="8d8ca-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d8ca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

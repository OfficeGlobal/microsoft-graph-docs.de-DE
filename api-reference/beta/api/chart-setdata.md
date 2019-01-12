---
title: 'Chart: setData'
description: Setzt die Quelldaten für das Diagramm zurück.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a92fe8e0c43b5dff4a406efbe0c2238ff0cab0ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921661"
---
# <a name="chart-setdata"></a><span data-ttu-id="8d222-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="8d222-103">Chart: setData</span></span>

> <span data-ttu-id="8d222-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d222-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d222-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d222-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d222-106">Setzt die Quelldaten für das Diagramm zurück.</span><span class="sxs-lookup"><span data-stu-id="8d222-106">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d222-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8d222-107">Permissions</span></span>
<span data-ttu-id="8d222-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d222-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d222-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d222-110">Permission type</span></span>      | <span data-ttu-id="8d222-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d222-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d222-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d222-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d222-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d222-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d222-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d222-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d222-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d222-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d222-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d222-116">Application</span></span> | <span data-ttu-id="8d222-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d222-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d222-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d222-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="8d222-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d222-119">Request headers</span></span>
| <span data-ttu-id="8d222-120">Name</span><span class="sxs-lookup"><span data-stu-id="8d222-120">Name</span></span>       | <span data-ttu-id="8d222-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d222-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d222-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d222-122">Authorization</span></span>  | <span data-ttu-id="8d222-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8d222-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d222-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8d222-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8d222-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8d222-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d222-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d222-128">Request body</span></span>
<span data-ttu-id="8d222-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8d222-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d222-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="8d222-130">Parameter</span></span>    | <span data-ttu-id="8d222-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8d222-131">Type</span></span>   |<span data-ttu-id="8d222-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d222-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d222-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="8d222-133">sourceData</span></span>|<span data-ttu-id="8d222-134">string</span><span class="sxs-lookup"><span data-stu-id="8d222-134">string</span></span>|<span data-ttu-id="8d222-135">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="8d222-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="8d222-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="8d222-136">seriesBy</span></span>|<span data-ttu-id="8d222-137">string</span><span class="sxs-lookup"><span data-stu-id="8d222-137">string</span></span>|<span data-ttu-id="8d222-p105">Optional. Gibt an, wie Spalten oder Zeilen als Datenreihen im Diagramm verwendet werden. Folgende Ergebnisse sind möglich: Auto (Standard), Rows, Columns.  Mögliche Werte: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="8d222-p105">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="8d222-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d222-142">Response</span></span>

<span data-ttu-id="8d222-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d222-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d222-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d222-145">Example</span></span>
<span data-ttu-id="8d222-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8d222-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d222-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d222-147">Request</span></span>
<span data-ttu-id="8d222-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d222-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="8d222-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d222-149">Response</span></span>
<span data-ttu-id="8d222-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8d222-150">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'Chart: setData'
description: Setzt die Quelldaten für das Diagramm zurück.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b295b38df2cf7be1c568588d58bfb2cf529f4dc4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858149"
---
# <a name="chart-setdata"></a><span data-ttu-id="2b856-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="2b856-103">Chart: setData</span></span>

<span data-ttu-id="2b856-104">Setzt die Quelldaten für das Diagramm zurück.</span><span class="sxs-lookup"><span data-stu-id="2b856-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b856-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b856-105">Permissions</span></span>
<span data-ttu-id="2b856-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b856-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b856-108">Permission type</span></span>      | <span data-ttu-id="2b856-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b856-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b856-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b856-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b856-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b856-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2b856-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b856-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b856-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b856-113">Not supported.</span></span>    |
|<span data-ttu-id="2b856-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b856-114">Application</span></span> | <span data-ttu-id="2b856-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b856-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b856-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b856-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="2b856-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b856-117">Request headers</span></span>
| <span data-ttu-id="2b856-118">Name</span><span class="sxs-lookup"><span data-stu-id="2b856-118">Name</span></span>       | <span data-ttu-id="2b856-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b856-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2b856-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b856-120">Authorization</span></span>  | <span data-ttu-id="2b856-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b856-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b856-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2b856-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2b856-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2b856-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b856-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b856-126">Request body</span></span>
<span data-ttu-id="2b856-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2b856-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2b856-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="2b856-128">Parameter</span></span>    | <span data-ttu-id="2b856-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2b856-129">Type</span></span>   |<span data-ttu-id="2b856-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b856-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b856-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="2b856-131">sourceData</span></span>|<span data-ttu-id="2b856-132">Json</span><span class="sxs-lookup"><span data-stu-id="2b856-132">Json</span></span>|<span data-ttu-id="2b856-133">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2b856-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="2b856-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="2b856-134">seriesBy</span></span>|<span data-ttu-id="2b856-135">string</span><span class="sxs-lookup"><span data-stu-id="2b856-135">string</span></span>|<span data-ttu-id="2b856-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="2b856-136">Optional.</span></span> <span data-ttu-id="2b856-137">Gibt an, dass die Möglichkeit Spalten und Zeilen als Datenreihen im Diagramm verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2b856-137">Specifies the way columns or rows are used as data series on the chart.</span></span> <span data-ttu-id="2b856-138">Kann eine der folgenden sein: automatisch (Standardeinstellung), Zeilen, Spalten.</span><span class="sxs-lookup"><span data-stu-id="2b856-138">Can be one of the following: Auto (default), Rows, Columns.</span></span>  <span data-ttu-id="2b856-139">Die möglichen Werte sind: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="2b856-139">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="2b856-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b856-140">Response</span></span>

<span data-ttu-id="2b856-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b856-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b856-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b856-143">Example</span></span>
<span data-ttu-id="2b856-144">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2b856-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2b856-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b856-145">Request</span></span>
<span data-ttu-id="2b856-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b856-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="2b856-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b856-147">Response</span></span>
<span data-ttu-id="2b856-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2b856-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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

---
title: 'ChartSeriesCollection: ItemAt'
description: Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.
ms.openlocfilehash: 493cfb974961a16a2229b4e37f8b5b4ecc2d6cb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018321"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="99e64-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="99e64-103">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="99e64-104">Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="99e64-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="99e64-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99e64-105">Permissions</span></span>
<span data-ttu-id="99e64-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99e64-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99e64-108">Permission type</span></span>      | <span data-ttu-id="99e64-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99e64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99e64-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99e64-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99e64-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99e64-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99e64-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99e64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e64-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99e64-113">Not supported.</span></span>    |
|<span data-ttu-id="99e64-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99e64-114">Application</span></span> | <span data-ttu-id="99e64-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99e64-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99e64-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99e64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="99e64-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99e64-117">Request headers</span></span>
| <span data-ttu-id="99e64-118">Name</span><span class="sxs-lookup"><span data-stu-id="99e64-118">Name</span></span>       | <span data-ttu-id="99e64-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99e64-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99e64-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e64-120">Authorization</span></span>  | <span data-ttu-id="99e64-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99e64-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99e64-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="99e64-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="99e64-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="99e64-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99e64-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99e64-126">Request body</span></span>
<span data-ttu-id="99e64-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="99e64-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99e64-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="99e64-128">Parameter</span></span>    | <span data-ttu-id="99e64-129">Typ</span><span class="sxs-lookup"><span data-stu-id="99e64-129">Type</span></span>   |<span data-ttu-id="99e64-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99e64-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99e64-131">Index</span><span class="sxs-lookup"><span data-stu-id="99e64-131">index</span></span>|<span data-ttu-id="99e64-132">Int32</span><span class="sxs-lookup"><span data-stu-id="99e64-132">Int32</span></span>|<span data-ttu-id="99e64-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="99e64-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="99e64-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="99e64-135">Response</span></span>

<span data-ttu-id="99e64-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookChartSeries](../resources/chartseries.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="99e64-136">If successful, this method returns `200 OK` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99e64-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99e64-137">Example</span></span>
<span data-ttu-id="99e64-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="99e64-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99e64-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99e64-139">Request</span></span>
<span data-ttu-id="99e64-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99e64-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```

##### <a name="response"></a><span data-ttu-id="99e64-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="99e64-141">Response</span></span>
<span data-ttu-id="99e64-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99e64-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
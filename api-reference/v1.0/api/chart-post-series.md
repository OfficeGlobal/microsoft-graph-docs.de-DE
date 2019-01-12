---
title: ChartSeries erstellen
description: Verwenden Sie diese API, um eine neue ChartSeries zu erstellen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 053fd380728928241c146787c03b87a5207a0b7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927534"
---
# <a name="create-chartseries"></a><span data-ttu-id="f803f-103">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="f803f-103">Create ChartSeries</span></span>

<span data-ttu-id="f803f-104">Verwenden Sie diese API, um eine neue ChartSeries zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f803f-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="f803f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f803f-105">Permissions</span></span>
<span data-ttu-id="f803f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f803f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f803f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f803f-108">Permission type</span></span>      | <span data-ttu-id="f803f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f803f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f803f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f803f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f803f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f803f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f803f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f803f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f803f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f803f-113">Not supported.</span></span>    |
|<span data-ttu-id="f803f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f803f-114">Application</span></span> | <span data-ttu-id="f803f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f803f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f803f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f803f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="f803f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f803f-117">Request headers</span></span>
| <span data-ttu-id="f803f-118">Name</span><span class="sxs-lookup"><span data-stu-id="f803f-118">Name</span></span>       | <span data-ttu-id="f803f-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f803f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f803f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f803f-120">Authorization</span></span>  | <span data-ttu-id="f803f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f803f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f803f-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="f803f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f803f-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="f803f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f803f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f803f-126">Request body</span></span>
<span data-ttu-id="f803f-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [WorkbookChartSeries](../resources/chartseries.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f803f-127">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f803f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f803f-128">Response</span></span>

<span data-ttu-id="f803f-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und [WorkbookChartSeries](../resources/chartseries.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f803f-129">If successful, this method returns `201 Created` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f803f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f803f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f803f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f803f-131">Request</span></span>
<span data-ttu-id="f803f-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f803f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="f803f-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [WorkbookChartSeries](../resources/chartseries.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f803f-133">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f803f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f803f-134">Response</span></span>
<span data-ttu-id="f803f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f803f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

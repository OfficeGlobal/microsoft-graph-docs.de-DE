---
title: ChartSeries erstellen
description: Verwenden Sie diese API, um eine neue ChartSeries zu erstellen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 16e72376dde3d009a83d679ca88ec145e00c4496
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946700"
---
# <a name="create-chartseries"></a><span data-ttu-id="956b7-103">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="956b7-103">Create ChartSeries</span></span>

> <span data-ttu-id="956b7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="956b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="956b7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="956b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="956b7-106">Verwenden Sie diese API, um eine neue ChartSeries zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="956b7-106">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="956b7-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="956b7-107">Permissions</span></span>
<span data-ttu-id="956b7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="956b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="956b7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="956b7-110">Permission type</span></span>      | <span data-ttu-id="956b7-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="956b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="956b7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="956b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="956b7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="956b7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="956b7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="956b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="956b7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="956b7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="956b7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="956b7-116">Application</span></span> | <span data-ttu-id="956b7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="956b7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="956b7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="956b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="956b7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="956b7-119">Request headers</span></span>
| <span data-ttu-id="956b7-120">Name</span><span class="sxs-lookup"><span data-stu-id="956b7-120">Name</span></span>       | <span data-ttu-id="956b7-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="956b7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="956b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="956b7-122">Authorization</span></span>  | <span data-ttu-id="956b7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="956b7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="956b7-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="956b7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="956b7-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="956b7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="956b7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="956b7-128">Request body</span></span>
<span data-ttu-id="956b7-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartSeries](../resources/chartseries.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="956b7-129">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="956b7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="956b7-130">Response</span></span>

<span data-ttu-id="956b7-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [ChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="956b7-131">If successful, this method returns `201 Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="956b7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="956b7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="956b7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="956b7-133">Request</span></span>
<span data-ttu-id="956b7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="956b7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="956b7-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartSeries](../resources/chartseries.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="956b7-135">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="956b7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="956b7-136">Response</span></span>
<span data-ttu-id="956b7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="956b7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
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

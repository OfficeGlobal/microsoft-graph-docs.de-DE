---
title: 'ChartSeriesCollection: ItemAt'
description: Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 063a5a605908693e5b189c92865eaec2c0dba1ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518268"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="9d385-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="9d385-103">ChartSeriesCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d385-104">Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="9d385-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="9d385-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d385-105">Permissions</span></span>
<span data-ttu-id="9d385-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d385-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d385-108">Permission type</span></span>      | <span data-ttu-id="9d385-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d385-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d385-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d385-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d385-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d385-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9d385-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d385-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d385-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d385-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9d385-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d385-114">Application</span></span> | <span data-ttu-id="9d385-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d385-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d385-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d385-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="9d385-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d385-117">Request headers</span></span>
| <span data-ttu-id="9d385-118">Name</span><span class="sxs-lookup"><span data-stu-id="9d385-118">Name</span></span>       | <span data-ttu-id="9d385-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d385-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9d385-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d385-120">Authorization</span></span>  | <span data-ttu-id="9d385-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d385-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d385-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9d385-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9d385-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9d385-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d385-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d385-126">Request body</span></span>
<span data-ttu-id="9d385-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9d385-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9d385-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="9d385-128">Parameter</span></span>    | <span data-ttu-id="9d385-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9d385-129">Type</span></span>   |<span data-ttu-id="9d385-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d385-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d385-131">Index</span><span class="sxs-lookup"><span data-stu-id="9d385-131">index</span></span>|<span data-ttu-id="9d385-132">number</span><span class="sxs-lookup"><span data-stu-id="9d385-132">number</span></span>|<span data-ttu-id="9d385-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="9d385-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="9d385-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d385-135">Response</span></span>

<span data-ttu-id="9d385-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d385-136">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d385-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d385-137">Example</span></span>
<span data-ttu-id="9d385-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9d385-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9d385-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d385-139">Request</span></span>
<span data-ttu-id="9d385-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d385-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="9d385-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d385-141">Response</span></span>
<span data-ttu-id="9d385-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d385-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartseriescollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

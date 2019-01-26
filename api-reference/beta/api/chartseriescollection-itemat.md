---
title: 'ChartSeriesCollection: ItemAt'
description: Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cadfcec8b2d114697d6a5c015aa6715ec90eee31
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576192"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="9386a-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="9386a-103">ChartSeriesCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9386a-104">Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="9386a-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="9386a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9386a-105">Permissions</span></span>
<span data-ttu-id="9386a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9386a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9386a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9386a-108">Permission type</span></span>      | <span data-ttu-id="9386a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9386a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9386a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9386a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9386a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9386a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9386a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9386a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9386a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9386a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9386a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9386a-114">Application</span></span> | <span data-ttu-id="9386a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9386a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9386a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9386a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="9386a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9386a-117">Request headers</span></span>
| <span data-ttu-id="9386a-118">Name</span><span class="sxs-lookup"><span data-stu-id="9386a-118">Name</span></span>       | <span data-ttu-id="9386a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9386a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9386a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9386a-120">Authorization</span></span>  | <span data-ttu-id="9386a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9386a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9386a-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9386a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9386a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9386a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9386a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9386a-126">Request body</span></span>
<span data-ttu-id="9386a-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9386a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9386a-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="9386a-128">Parameter</span></span>    | <span data-ttu-id="9386a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9386a-129">Type</span></span>   |<span data-ttu-id="9386a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9386a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9386a-131">Index</span><span class="sxs-lookup"><span data-stu-id="9386a-131">index</span></span>|<span data-ttu-id="9386a-132">number</span><span class="sxs-lookup"><span data-stu-id="9386a-132">number</span></span>|<span data-ttu-id="9386a-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="9386a-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="9386a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9386a-135">Response</span></span>

<span data-ttu-id="9386a-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9386a-136">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9386a-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9386a-137">Example</span></span>
<span data-ttu-id="9386a-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9386a-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9386a-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9386a-139">Request</span></span>
<span data-ttu-id="9386a-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9386a-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9386a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9386a-141">Response</span></span>
<span data-ttu-id="9386a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9386a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

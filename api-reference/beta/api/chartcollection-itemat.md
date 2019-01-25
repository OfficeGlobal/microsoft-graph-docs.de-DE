---
title: 'ChartCollection: ItemAt'
description: Ruft ein Diagramm anhand seiner Position in der Sammlung ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 82e5d79ee4498a5b5b4e2fc2adc0461aec13cae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521712"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="e12f4-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e12f4-103">ChartCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e12f4-104">Ruft ein Diagramm anhand seiner Position in der Sammlung ab.</span><span class="sxs-lookup"><span data-stu-id="e12f4-104">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="e12f4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e12f4-105">Permissions</span></span>
<span data-ttu-id="e12f4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e12f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e12f4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e12f4-108">Permission type</span></span>      | <span data-ttu-id="e12f4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e12f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e12f4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e12f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e12f4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e12f4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e12f4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e12f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e12f4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e12f4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e12f4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e12f4-114">Application</span></span> | <span data-ttu-id="e12f4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e12f4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e12f4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e12f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="e12f4-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e12f4-117">Request headers</span></span>
| <span data-ttu-id="e12f4-118">Name</span><span class="sxs-lookup"><span data-stu-id="e12f4-118">Name</span></span>       | <span data-ttu-id="e12f4-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e12f4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e12f4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e12f4-120">Authorization</span></span>  | <span data-ttu-id="e12f4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e12f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e12f4-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e12f4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e12f4-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e12f4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e12f4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e12f4-126">Request body</span></span>
<span data-ttu-id="e12f4-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e12f4-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e12f4-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="e12f4-128">Parameter</span></span>    | <span data-ttu-id="e12f4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e12f4-129">Type</span></span>   |<span data-ttu-id="e12f4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e12f4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e12f4-131">Index</span><span class="sxs-lookup"><span data-stu-id="e12f4-131">index</span></span>|<span data-ttu-id="e12f4-132">number</span><span class="sxs-lookup"><span data-stu-id="e12f4-132">number</span></span>|<span data-ttu-id="e12f4-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="e12f4-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e12f4-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e12f4-135">Response</span></span>

<span data-ttu-id="e12f4-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e12f4-136">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e12f4-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e12f4-137">Example</span></span>
<span data-ttu-id="e12f4-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e12f4-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e12f4-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e12f4-139">Request</span></span>
<span data-ttu-id="e12f4-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e12f4-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="e12f4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e12f4-141">Response</span></span>
<span data-ttu-id="e12f4-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e12f4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartcollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

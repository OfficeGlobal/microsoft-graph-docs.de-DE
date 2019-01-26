---
title: 'ChartPointsCollection: ItemAt'
description: Dient zum Abrufen eines Punkts anhand seiner Position in der Datenreihe.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a7a4274790f39bc8443273df0fb617e65a564372
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577207"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="1a226-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="1a226-103">ChartPointsCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a226-104">Dient zum Abrufen eines Punkts anhand seiner Position in der Datenreihe.</span><span class="sxs-lookup"><span data-stu-id="1a226-104">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a226-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1a226-105">Permissions</span></span>
<span data-ttu-id="1a226-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a226-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a226-108">Permission type</span></span>      | <span data-ttu-id="1a226-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a226-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a226-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a226-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a226-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a226-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a226-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a226-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a226-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a226-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a226-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a226-114">Application</span></span> | <span data-ttu-id="1a226-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a226-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a226-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a226-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="1a226-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a226-117">Request headers</span></span>
| <span data-ttu-id="1a226-118">Name</span><span class="sxs-lookup"><span data-stu-id="1a226-118">Name</span></span>       | <span data-ttu-id="1a226-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a226-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a226-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a226-120">Authorization</span></span>  | <span data-ttu-id="1a226-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a226-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a226-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1a226-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1a226-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1a226-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a226-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a226-126">Request body</span></span>
<span data-ttu-id="1a226-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1a226-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a226-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="1a226-128">Parameter</span></span>    | <span data-ttu-id="1a226-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1a226-129">Type</span></span>   |<span data-ttu-id="1a226-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a226-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a226-131">Index</span><span class="sxs-lookup"><span data-stu-id="1a226-131">index</span></span>|<span data-ttu-id="1a226-132">number</span><span class="sxs-lookup"><span data-stu-id="1a226-132">number</span></span>|<span data-ttu-id="1a226-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="1a226-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="1a226-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a226-135">Response</span></span>

<span data-ttu-id="1a226-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [ChartPoint](../resources/chartpoint.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a226-136">If successful, this method returns `200 OK` response code and [ChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a226-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a226-137">Example</span></span>
<span data-ttu-id="1a226-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1a226-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1a226-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a226-139">Request</span></span>
<span data-ttu-id="1a226-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a226-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="1a226-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a226-141">Response</span></span>
<span data-ttu-id="1a226-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a226-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartpointscollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: Diagramme auflisten
description: Dient zum Abrufen einer Liste von Diagrammobjekten.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9f3b293f0f52086e7d34bd9dff3c909fe4c5b85b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641603"
---
# <a name="list-charts"></a><span data-ttu-id="1a0e8-103">Diagramme auflisten</span><span class="sxs-lookup"><span data-stu-id="1a0e8-103">List charts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a0e8-104">Dient zum Abrufen einer Liste von Diagrammobjekten.</span><span class="sxs-lookup"><span data-stu-id="1a0e8-104">Retrieve a list of chart objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a0e8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1a0e8-105">Permissions</span></span>
<span data-ttu-id="1a0e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a0e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a0e8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a0e8-108">Permission type</span></span>      | <span data-ttu-id="1a0e8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a0e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a0e8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a0e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a0e8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a0e8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a0e8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a0e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a0e8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a0e8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a0e8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a0e8-114">Application</span></span> | <span data-ttu-id="1a0e8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a0e8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a0e8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a0e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a0e8-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1a0e8-117">Optional query parameters</span></span>
<span data-ttu-id="1a0e8-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1a0e8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a0e8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a0e8-119">Request headers</span></span>
| <span data-ttu-id="1a0e8-120">Name</span><span class="sxs-lookup"><span data-stu-id="1a0e8-120">Name</span></span>      |<span data-ttu-id="1a0e8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a0e8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a0e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a0e8-122">Authorization</span></span>  | <span data-ttu-id="1a0e8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a0e8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a0e8-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1a0e8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1a0e8-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1a0e8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a0e8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a0e8-128">Request body</span></span>
<span data-ttu-id="1a0e8-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1a0e8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a0e8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a0e8-130">Response</span></span>

<span data-ttu-id="1a0e8-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Chart](../resources/chart.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a0e8-131">If successful, this method returns a `200 OK` response code and collection of [Chart](../resources/chart.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a0e8-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a0e8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a0e8-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a0e8-133">Request</span></span>
<span data-ttu-id="1a0e8-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a0e8-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_charts"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
```
##### <a name="response"></a><span data-ttu-id="1a0e8-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a0e8-135">Response</span></span>
<span data-ttu-id="1a0e8-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a0e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 93

{
  "value": [
    {
      "id": "id-value",
      "height": 99,
      "left": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List charts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-list-charts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

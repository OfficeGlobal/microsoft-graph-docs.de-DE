---
title: ChartAxisTitle abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des ChartAxisTitle-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6ce8b7d9518df01ec04b1191a9784ea015e83c7d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576143"
---
# <a name="get-chartaxistitle"></a><span data-ttu-id="269aa-103">ChartAxisTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="269aa-103">Get ChartAxisTitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="269aa-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des ChartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="269aa-104">Retrieve the properties and relationships of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="269aa-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="269aa-105">Permissions</span></span>
<span data-ttu-id="269aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="269aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="269aa-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="269aa-108">Permission type</span></span>      | <span data-ttu-id="269aa-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="269aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="269aa-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="269aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="269aa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="269aa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="269aa-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="269aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="269aa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="269aa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="269aa-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="269aa-114">Application</span></span> | <span data-ttu-id="269aa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="269aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="269aa-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="269aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="269aa-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="269aa-117">Optional query parameters</span></span>
<span data-ttu-id="269aa-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="269aa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="269aa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="269aa-119">Request headers</span></span>
| <span data-ttu-id="269aa-120">Name</span><span class="sxs-lookup"><span data-stu-id="269aa-120">Name</span></span>      |<span data-ttu-id="269aa-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="269aa-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="269aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="269aa-122">Authorization</span></span>  | <span data-ttu-id="269aa-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="269aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="269aa-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="269aa-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="269aa-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="269aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="269aa-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="269aa-128">Request body</span></span>
<span data-ttu-id="269aa-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="269aa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="269aa-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="269aa-130">Response</span></span>

<span data-ttu-id="269aa-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und [WorkbookChartAxisTitle](../resources/chartaxistitle.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="269aa-131">If successful, this method returns a `200 OK` response code and [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="269aa-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="269aa-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="269aa-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="269aa-133">Request</span></span>
<span data-ttu-id="269aa-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="269aa-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartaxistitle"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
```
##### <a name="response"></a><span data-ttu-id="269aa-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="269aa-135">Response</span></span>
<span data-ttu-id="269aa-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="269aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartAxisTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartaxistitle-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

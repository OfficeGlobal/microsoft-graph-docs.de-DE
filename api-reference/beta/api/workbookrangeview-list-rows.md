---
title: rangeView-Zeilen auflisten
description: Abrufen einer Liste von rangeView-Objekten.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9d0d3cb5f29f9588481b5e87c7a20cc96e3850e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523001"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="10f6c-103">rangeView-Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="10f6c-103">List rangeView rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10f6c-104">Abrufen einer Liste von rangeView-Objekten.</span><span class="sxs-lookup"><span data-stu-id="10f6c-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="10f6c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="10f6c-105">Permissions</span></span>
<span data-ttu-id="10f6c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10f6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f6c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10f6c-108">Permission type</span></span>      | <span data-ttu-id="10f6c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10f6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10f6c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10f6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10f6c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10f6c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="10f6c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10f6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10f6c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10f6c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="10f6c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10f6c-114">Application</span></span> | <span data-ttu-id="10f6c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10f6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10f6c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10f6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="10f6c-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="10f6c-117">Optional query parameters</span></span>
<span data-ttu-id="10f6c-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="10f6c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10f6c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10f6c-119">Request headers</span></span>
| <span data-ttu-id="10f6c-120">Name</span><span class="sxs-lookup"><span data-stu-id="10f6c-120">Name</span></span>      |<span data-ttu-id="10f6c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10f6c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10f6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10f6c-122">Authorization</span></span>  | <span data-ttu-id="10f6c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10f6c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10f6c-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="10f6c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="10f6c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="10f6c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10f6c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10f6c-128">Request body</span></span>
<span data-ttu-id="10f6c-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="10f6c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10f6c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="10f6c-130">Response</span></span>

<span data-ttu-id="10f6c-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [workbookRangeView](../resources/workbookrangeview.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10f6c-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10f6c-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10f6c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10f6c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10f6c-133">Request</span></span>
<span data-ttu-id="10f6c-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10f6c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="10f6c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="10f6c-135">Response</span></span>
<span data-ttu-id="10f6c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10f6c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-list-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

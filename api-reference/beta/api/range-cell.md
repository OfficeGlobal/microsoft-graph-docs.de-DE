---
title: 'Range: Cell'
description: Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 59e25d3155caf13cac5441e6553116c9a54ceac6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526683"
---
# <a name="range-cell"></a><span data-ttu-id="1e1fe-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="1e1fe-105">Range: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e1fe-p102">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e1fe-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1e1fe-109">Permissions</span></span>
<span data-ttu-id="1e1fe-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e1fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e1fe-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e1fe-112">Permission type</span></span>      | <span data-ttu-id="1e1fe-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e1fe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e1fe-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e1fe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1e1fe-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e1fe-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e1fe-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e1fe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e1fe-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e1fe-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e1fe-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e1fe-118">Application</span></span> | <span data-ttu-id="1e1fe-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e1fe-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e1fe-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e1fe-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="1e1fe-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e1fe-121">Request headers</span></span>
| <span data-ttu-id="1e1fe-122">Name</span><span class="sxs-lookup"><span data-stu-id="1e1fe-122">Name</span></span>       | <span data-ttu-id="1e1fe-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e1fe-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e1fe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e1fe-124">Authorization</span></span>  | <span data-ttu-id="1e1fe-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e1fe-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1e1fe-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="1e1fe-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e1fe-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e1fe-130">Request body</span></span>
<span data-ttu-id="1e1fe-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1e1fe-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="1e1fe-132">Parameter</span></span>    | <span data-ttu-id="1e1fe-133">Typ</span><span class="sxs-lookup"><span data-stu-id="1e1fe-133">Type</span></span>   |<span data-ttu-id="1e1fe-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e1fe-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e1fe-135">row</span><span class="sxs-lookup"><span data-stu-id="1e1fe-135">row</span></span>|<span data-ttu-id="1e1fe-136">number</span><span class="sxs-lookup"><span data-stu-id="1e1fe-136">number</span></span>|<span data-ttu-id="1e1fe-p106">Zeilenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="1e1fe-139">Spalte</span><span class="sxs-lookup"><span data-stu-id="1e1fe-139">column</span></span>|<span data-ttu-id="1e1fe-140">number</span><span class="sxs-lookup"><span data-stu-id="1e1fe-140">number</span></span>|<span data-ttu-id="1e1fe-p107">Spaltenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="1e1fe-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e1fe-143">Response</span></span>

<span data-ttu-id="1e1fe-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e1fe-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e1fe-145">Example</span></span>
<span data-ttu-id="1e1fe-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e1fe-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e1fe-147">Request</span></span>
<span data-ttu-id="1e1fe-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="1e1fe-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e1fe-149">Response</span></span>
<span data-ttu-id="1e1fe-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e1fe-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-cell.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

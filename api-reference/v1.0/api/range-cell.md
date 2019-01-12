---
title: 'Range: Cell'
description: Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a46f0e43a9eb1099c2df615b88f15576afa30e9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951481"
---
# <a name="range-cell"></a><span data-ttu-id="79463-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="79463-105">Range: Cell</span></span>

<span data-ttu-id="79463-p102">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="79463-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="79463-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79463-109">Permissions</span></span>
<span data-ttu-id="79463-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79463-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79463-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79463-112">Permission type</span></span>      | <span data-ttu-id="79463-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79463-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79463-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79463-114">Delegated (work or school account)</span></span> | <span data-ttu-id="79463-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79463-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79463-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79463-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79463-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79463-117">Not supported.</span></span>    |
|<span data-ttu-id="79463-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79463-118">Application</span></span> | <span data-ttu-id="79463-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79463-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79463-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79463-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="79463-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79463-121">Request headers</span></span>
| <span data-ttu-id="79463-122">Name</span><span class="sxs-lookup"><span data-stu-id="79463-122">Name</span></span>       | <span data-ttu-id="79463-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79463-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79463-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="79463-124">Authorization</span></span>  | <span data-ttu-id="79463-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79463-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79463-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="79463-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="79463-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="79463-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="79463-130">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="79463-130">Path parameters</span></span>
<span data-ttu-id="79463-131">Enthalten Sie in den Pfad die folgenden Parameter.</span><span class="sxs-lookup"><span data-stu-id="79463-131">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="79463-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="79463-132">Parameter</span></span>    | <span data-ttu-id="79463-133">Typ</span><span class="sxs-lookup"><span data-stu-id="79463-133">Type</span></span>   |<span data-ttu-id="79463-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79463-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79463-135">row</span><span class="sxs-lookup"><span data-stu-id="79463-135">row</span></span>|<span data-ttu-id="79463-136">Int32</span><span class="sxs-lookup"><span data-stu-id="79463-136">Int32</span></span>|<span data-ttu-id="79463-p106">Zeilenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="79463-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="79463-139">Spalte</span><span class="sxs-lookup"><span data-stu-id="79463-139">column</span></span>|<span data-ttu-id="79463-140">Int32</span><span class="sxs-lookup"><span data-stu-id="79463-140">Int32</span></span>|<span data-ttu-id="79463-p107">Spaltenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="79463-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="79463-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="79463-143">Response</span></span>

<span data-ttu-id="79463-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79463-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79463-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79463-145">Example</span></span>
<span data-ttu-id="79463-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="79463-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79463-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79463-147">Request</span></span>
<span data-ttu-id="79463-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79463-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```

##### <a name="response"></a><span data-ttu-id="79463-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="79463-149">Response</span></span>
<span data-ttu-id="79463-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79463-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

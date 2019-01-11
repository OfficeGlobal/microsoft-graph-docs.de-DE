---
title: 'Range: Cell'
description: Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.
localization_priority: Normal
ms.openlocfilehash: 2806fdcdc6072067a4fb4012fb9dc908aa3c15f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877014"
---
# <a name="range-cell"></a><span data-ttu-id="07896-105">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="07896-105">Range: Cell</span></span>

> <span data-ttu-id="07896-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07896-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07896-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07896-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07896-p103">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="07896-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="07896-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07896-111">Permissions</span></span>
<span data-ttu-id="07896-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07896-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07896-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07896-114">Permission type</span></span>      | <span data-ttu-id="07896-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07896-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07896-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07896-116">Delegated (work or school account)</span></span> | <span data-ttu-id="07896-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07896-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07896-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07896-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07896-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07896-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07896-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07896-120">Application</span></span> | <span data-ttu-id="07896-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07896-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07896-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07896-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="07896-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07896-123">Request headers</span></span>
| <span data-ttu-id="07896-124">Name</span><span class="sxs-lookup"><span data-stu-id="07896-124">Name</span></span>       | <span data-ttu-id="07896-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07896-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07896-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="07896-126">Authorization</span></span>  | <span data-ttu-id="07896-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07896-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07896-129">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="07896-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="07896-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="07896-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07896-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07896-132">Request body</span></span>
<span data-ttu-id="07896-133">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="07896-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="07896-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="07896-134">Parameter</span></span>    | <span data-ttu-id="07896-135">Typ</span><span class="sxs-lookup"><span data-stu-id="07896-135">Type</span></span>   |<span data-ttu-id="07896-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07896-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07896-137">row</span><span class="sxs-lookup"><span data-stu-id="07896-137">row</span></span>|<span data-ttu-id="07896-138">number</span><span class="sxs-lookup"><span data-stu-id="07896-138">number</span></span>|<span data-ttu-id="07896-p107">Zeilenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="07896-p107">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="07896-141">Spalte</span><span class="sxs-lookup"><span data-stu-id="07896-141">column</span></span>|<span data-ttu-id="07896-142">number</span><span class="sxs-lookup"><span data-stu-id="07896-142">number</span></span>|<span data-ttu-id="07896-p108">Spaltenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="07896-p108">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="07896-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="07896-145">Response</span></span>

<span data-ttu-id="07896-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07896-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07896-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07896-147">Example</span></span>
<span data-ttu-id="07896-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="07896-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="07896-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07896-149">Request</span></span>
<span data-ttu-id="07896-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07896-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="07896-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="07896-151">Response</span></span>
<span data-ttu-id="07896-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07896-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

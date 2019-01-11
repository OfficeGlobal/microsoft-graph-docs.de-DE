---
title: 'Range: OffsetRange'
description: Ruft ein Objekt ab, das einen Bereich darstellt, der aus dem angegebenen Bereich versetzt ist. Die Dimension des zurückgegebenen Bereichs entspricht diesem Bereich. Wenn der resultierende Bereich außerhalb des Arbeitsblatt-Rasters erzwungen wird, wird eine Ausnahme ausgelöst.
localization_priority: Normal
ms.openlocfilehash: 7364420e660612995300e4fba964dc29de656be2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815918"
---
# <a name="range-offsetrange"></a><span data-ttu-id="aab67-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="aab67-105">Range: OffsetRange</span></span>

<span data-ttu-id="aab67-p102">Ruft ein Objekt ab, das einen Bereich darstellt, der aus dem angegebenen Bereich versetzt ist. Die Dimension des zurückgegebenen Bereichs entspricht diesem Bereich. Wenn der resultierende Bereich außerhalb des Arbeitsblatt-Rasters erzwungen wird, wird eine Ausnahme ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="aab67-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="aab67-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aab67-109">Permissions</span></span>
<span data-ttu-id="aab67-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aab67-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aab67-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aab67-112">Permission type</span></span>      | <span data-ttu-id="aab67-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aab67-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aab67-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aab67-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aab67-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aab67-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aab67-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aab67-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aab67-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aab67-117">Not supported.</span></span>    |
|<span data-ttu-id="aab67-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aab67-118">Application</span></span> | <span data-ttu-id="aab67-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aab67-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aab67-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aab67-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/offsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/offsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/offsetRange

```
## <a name="request-headers"></a><span data-ttu-id="aab67-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aab67-121">Request headers</span></span>
| <span data-ttu-id="aab67-122">Name</span><span class="sxs-lookup"><span data-stu-id="aab67-122">Name</span></span>       | <span data-ttu-id="aab67-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aab67-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aab67-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aab67-124">Authorization</span></span>  | <span data-ttu-id="aab67-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aab67-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aab67-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="aab67-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="aab67-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="aab67-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aab67-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aab67-130">Request body</span></span>
<span data-ttu-id="aab67-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="aab67-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aab67-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="aab67-132">Parameter</span></span>    | <span data-ttu-id="aab67-133">Typ</span><span class="sxs-lookup"><span data-stu-id="aab67-133">Type</span></span>   |<span data-ttu-id="aab67-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aab67-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aab67-135">rowOffset</span><span class="sxs-lookup"><span data-stu-id="aab67-135">rowOffset</span></span>|<span data-ttu-id="aab67-136">Int32</span><span class="sxs-lookup"><span data-stu-id="aab67-136">Int32</span></span>|<span data-ttu-id="aab67-p106">Die Anzahl an Zeilen (positiv, negativ oder 0), um die der Bereich versetzt werden muss. Bei positiven Werten wird der Bereich nach unten versetzt. Bei negativen Werten wird der Bereich nach oben versetzt.</span><span class="sxs-lookup"><span data-stu-id="aab67-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="aab67-139">columnOffset</span><span class="sxs-lookup"><span data-stu-id="aab67-139">columnOffset</span></span>|<span data-ttu-id="aab67-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aab67-140">Int32</span></span>|<span data-ttu-id="aab67-p107">Die Anzahl an Spalten (positiv, negativ oder 0), um die der Bereich versetzt werden muss. Bei positiven Werten wird der Bereich nach unten versetzt. Bei negativen Werten wird der Bereich nach oben versetzt.</span><span class="sxs-lookup"><span data-stu-id="aab67-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="aab67-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="aab67-143">Response</span></span>

<span data-ttu-id="aab67-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aab67-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aab67-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aab67-145">Example</span></span>
<span data-ttu-id="aab67-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="aab67-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aab67-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aab67-147">Request</span></span>
<span data-ttu-id="aab67-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aab67-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/offsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": 3,
  "columnOffset": 5
}
```

##### <a name="response"></a><span data-ttu-id="aab67-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="aab67-149">Response</span></span>
<span data-ttu-id="aab67-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aab67-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

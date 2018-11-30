---
title: 'Range: OffsetRange'
description: Ruft ein Objekt ab, das einen Bereich darstellt, der aus dem angegebenen Bereich versetzt ist. Die Dimension des zurückgegebenen Bereichs entspricht diesem Bereich. Wenn der resultierende Bereich außerhalb des Arbeitsblatt-Rasters erzwungen wird, wird eine Ausnahme ausgelöst.
ms.openlocfilehash: 301862e46a571754bcb4032c7c7bf87e3564268f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062875"
---
# <a name="range-offsetrange"></a><span data-ttu-id="46c38-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="46c38-105">Range: OffsetRange</span></span>

> <span data-ttu-id="46c38-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="46c38-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46c38-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46c38-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46c38-p103">Ruft ein Objekt ab, das einen Bereich darstellt, der aus dem angegebenen Bereich versetzt ist. Die Dimension des zurückgegebenen Bereichs entspricht diesem Bereich. Wenn der resultierende Bereich außerhalb des Arbeitsblatt-Rasters erzwungen wird, wird eine Ausnahme ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="46c38-p103">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="46c38-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="46c38-111">Permissions</span></span>
<span data-ttu-id="46c38-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46c38-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46c38-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46c38-114">Permission type</span></span>      | <span data-ttu-id="46c38-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46c38-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46c38-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46c38-116">Delegated (work or school account)</span></span> | <span data-ttu-id="46c38-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46c38-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46c38-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46c38-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46c38-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46c38-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46c38-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46c38-120">Application</span></span> | <span data-ttu-id="46c38-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46c38-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46c38-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46c38-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="46c38-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46c38-123">Request headers</span></span>
| <span data-ttu-id="46c38-124">Name</span><span class="sxs-lookup"><span data-stu-id="46c38-124">Name</span></span>       | <span data-ttu-id="46c38-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46c38-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46c38-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="46c38-126">Authorization</span></span>  | <span data-ttu-id="46c38-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="46c38-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46c38-129">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="46c38-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="46c38-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="46c38-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46c38-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46c38-132">Request body</span></span>
<span data-ttu-id="46c38-133">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="46c38-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46c38-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="46c38-134">Parameter</span></span>    | <span data-ttu-id="46c38-135">Typ</span><span class="sxs-lookup"><span data-stu-id="46c38-135">Type</span></span>   |<span data-ttu-id="46c38-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46c38-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46c38-137">rowOffset</span><span class="sxs-lookup"><span data-stu-id="46c38-137">rowOffset</span></span>|<span data-ttu-id="46c38-138">number</span><span class="sxs-lookup"><span data-stu-id="46c38-138">number</span></span>|<span data-ttu-id="46c38-p107">Die Anzahl an Zeilen (positiv, negativ oder 0), um die der Bereich versetzt werden muss. Bei positiven Werten wird der Bereich nach unten versetzt. Bei negativen Werten wird der Bereich nach oben versetzt.</span><span class="sxs-lookup"><span data-stu-id="46c38-p107">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="46c38-141">columnOffset</span><span class="sxs-lookup"><span data-stu-id="46c38-141">columnOffset</span></span>|<span data-ttu-id="46c38-142">number</span><span class="sxs-lookup"><span data-stu-id="46c38-142">number</span></span>|<span data-ttu-id="46c38-p108">Die Anzahl an Spalten (positiv, negativ oder 0), um die der Bereich versetzt werden muss. Bei positiven Werten wird der Bereich nach unten versetzt. Bei negativen Werten wird der Bereich nach oben versetzt.</span><span class="sxs-lookup"><span data-stu-id="46c38-p108">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="46c38-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="46c38-145">Response</span></span>

<span data-ttu-id="46c38-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46c38-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46c38-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46c38-147">Example</span></span>
<span data-ttu-id="46c38-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="46c38-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46c38-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46c38-149">Request</span></span>
<span data-ttu-id="46c38-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46c38-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="46c38-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="46c38-151">Response</span></span>
<span data-ttu-id="46c38-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46c38-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
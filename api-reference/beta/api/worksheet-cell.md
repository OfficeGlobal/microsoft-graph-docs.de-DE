---
title: 'Arbeitsblatt: Zelle'
description: Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5b4771283922c4c41aeb3210040b3e95823cad81
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976065"
---
# <a name="worksheet-cell"></a><span data-ttu-id="75745-104">Arbeitsblatt: Zelle</span><span class="sxs-lookup"><span data-stu-id="75745-104">Worksheet: Cell</span></span>

> <span data-ttu-id="75745-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="75745-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75745-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75745-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75745-p103">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.</span><span class="sxs-lookup"><span data-stu-id="75745-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="75745-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="75745-109">Permissions</span></span>
<span data-ttu-id="75745-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75745-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75745-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75745-112">Permission type</span></span>      | <span data-ttu-id="75745-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75745-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75745-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75745-114">Delegated (work or school account)</span></span> | <span data-ttu-id="75745-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75745-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75745-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75745-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75745-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75745-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75745-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75745-118">Application</span></span> | <span data-ttu-id="75745-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75745-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75745-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75745-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="75745-121">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="75745-121">Function parameters</span></span>
<span data-ttu-id="75745-122">Geben Sie in der Anforderungspfad die folgenden Parameter an.</span><span class="sxs-lookup"><span data-stu-id="75745-122">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="75745-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="75745-123">Parameter</span></span>    | <span data-ttu-id="75745-124">Typ</span><span class="sxs-lookup"><span data-stu-id="75745-124">Type</span></span>   |<span data-ttu-id="75745-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75745-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75745-126">row</span><span class="sxs-lookup"><span data-stu-id="75745-126">row</span></span>|<span data-ttu-id="75745-127">Int32</span><span class="sxs-lookup"><span data-stu-id="75745-127">Int32</span></span>|<span data-ttu-id="75745-p105">Zeilenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="75745-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="75745-130">Spalte</span><span class="sxs-lookup"><span data-stu-id="75745-130">column</span></span>|<span data-ttu-id="75745-131">Int32</span><span class="sxs-lookup"><span data-stu-id="75745-131">Int32</span></span>|<span data-ttu-id="75745-p106">Spaltenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="75745-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="75745-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75745-134">Request headers</span></span>
| <span data-ttu-id="75745-135">Name</span><span class="sxs-lookup"><span data-stu-id="75745-135">Name</span></span>       | <span data-ttu-id="75745-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75745-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75745-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="75745-137">Authorization</span></span>  | <span data-ttu-id="75745-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="75745-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75745-140">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="75745-140">Workbook-Session-Id</span></span>  | <span data-ttu-id="75745-p108">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="75745-p108">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75745-143">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75745-143">Request body</span></span>
<span data-ttu-id="75745-144">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="75745-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75745-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="75745-145">Response</span></span>

<span data-ttu-id="75745-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75745-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75745-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75745-147">Example</span></span>
<span data-ttu-id="75745-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="75745-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75745-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75745-149">Request</span></span>
<span data-ttu-id="75745-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75745-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="75745-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="75745-151">Response</span></span>
<span data-ttu-id="75745-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75745-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

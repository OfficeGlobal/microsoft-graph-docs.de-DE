---
title: 'Arbeitsblatt: Zelle'
description: Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4649a361ec46b9fb904cf959608fdee502f05c22
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520557"
---
# <a name="worksheet-cell"></a><span data-ttu-id="2520d-104">Arbeitsblatt: Zelle</span><span class="sxs-lookup"><span data-stu-id="2520d-104">Worksheet: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2520d-p102">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.</span><span class="sxs-lookup"><span data-stu-id="2520d-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="2520d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2520d-107">Permissions</span></span>
<span data-ttu-id="2520d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2520d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2520d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2520d-110">Permission type</span></span>      | <span data-ttu-id="2520d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2520d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2520d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2520d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2520d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2520d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2520d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2520d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2520d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2520d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2520d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2520d-116">Application</span></span> | <span data-ttu-id="2520d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2520d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2520d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2520d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="2520d-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="2520d-119">Function parameters</span></span>
<span data-ttu-id="2520d-120">Geben Sie in der Anforderungspfad die folgenden Parameter an.</span><span class="sxs-lookup"><span data-stu-id="2520d-120">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="2520d-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="2520d-121">Parameter</span></span>    | <span data-ttu-id="2520d-122">Typ</span><span class="sxs-lookup"><span data-stu-id="2520d-122">Type</span></span>   |<span data-ttu-id="2520d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2520d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2520d-124">row</span><span class="sxs-lookup"><span data-stu-id="2520d-124">row</span></span>|<span data-ttu-id="2520d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2520d-125">Int32</span></span>|<span data-ttu-id="2520d-p104">Zeilenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="2520d-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="2520d-128">Spalte</span><span class="sxs-lookup"><span data-stu-id="2520d-128">column</span></span>|<span data-ttu-id="2520d-129">Int32</span><span class="sxs-lookup"><span data-stu-id="2520d-129">Int32</span></span>|<span data-ttu-id="2520d-p105">Spaltenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="2520d-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2520d-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2520d-132">Request headers</span></span>
| <span data-ttu-id="2520d-133">Name</span><span class="sxs-lookup"><span data-stu-id="2520d-133">Name</span></span>       | <span data-ttu-id="2520d-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2520d-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2520d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="2520d-135">Authorization</span></span>  | <span data-ttu-id="2520d-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2520d-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2520d-138">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2520d-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="2520d-p107">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2520d-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2520d-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2520d-141">Request body</span></span>
<span data-ttu-id="2520d-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2520d-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2520d-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2520d-143">Response</span></span>

<span data-ttu-id="2520d-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2520d-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2520d-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2520d-145">Example</span></span>
<span data-ttu-id="2520d-146">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2520d-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2520d-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2520d-147">Request</span></span>
<span data-ttu-id="2520d-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2520d-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="2520d-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="2520d-149">Response</span></span>
<span data-ttu-id="2520d-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2520d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-cell.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: 'Range: Column'
description: Ruft eine Spalte ab, die im Bereich enthalten ist.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 04724e43b5e26d89dcefc71c07a23051a6ed9719
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526018"
---
# <a name="range-column"></a><span data-ttu-id="e0fb1-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="e0fb1-103">Range: Column</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0fb1-104">Ruft eine Spalte ab, die im Bereich enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0fb1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0fb1-105">Permissions</span></span>
<span data-ttu-id="e0fb1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0fb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0fb1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0fb1-108">Permission type</span></span>      | <span data-ttu-id="e0fb1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0fb1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0fb1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0fb1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0fb1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0fb1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0fb1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0fb1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0fb1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0fb1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0fb1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0fb1-114">Application</span></span> | <span data-ttu-id="e0fb1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0fb1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0fb1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0fb1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Column
GET /workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="e0fb1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0fb1-117">Request headers</span></span>
| <span data-ttu-id="e0fb1-118">Name</span><span class="sxs-lookup"><span data-stu-id="e0fb1-118">Name</span></span>       | <span data-ttu-id="e0fb1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0fb1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0fb1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0fb1-120">Authorization</span></span>  | <span data-ttu-id="e0fb1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0fb1-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e0fb1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0fb1-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0fb1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0fb1-126">Request body</span></span>
<span data-ttu-id="e0fb1-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0fb1-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="e0fb1-128">Parameter</span></span>    | <span data-ttu-id="e0fb1-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e0fb1-129">Type</span></span>   |<span data-ttu-id="e0fb1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0fb1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0fb1-131">Spalte</span><span class="sxs-lookup"><span data-stu-id="e0fb1-131">column</span></span>|<span data-ttu-id="e0fb1-132">number</span><span class="sxs-lookup"><span data-stu-id="e0fb1-132">number</span></span>|<span data-ttu-id="e0fb1-p104">Spaltenanzahl des abzurufenden Bereichs. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e0fb1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0fb1-135">Response</span></span>

<span data-ttu-id="e0fb1-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0fb1-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0fb1-137">Example</span></span>
<span data-ttu-id="e0fb1-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0fb1-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0fb1-139">Request</span></span>
<span data-ttu-id="e0fb1-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="e0fb1-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0fb1-141">Response</span></span>
<span data-ttu-id="e0fb1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0fb1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-column.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

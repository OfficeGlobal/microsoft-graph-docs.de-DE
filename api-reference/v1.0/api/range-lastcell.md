---
title: 'Range: LastCell'
description: .
author: lumine2008
ms.openlocfilehash: 4ae70424c252dab716ec0fe2a83ea434411238c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347033"
---
# <a name="range-lastcell"></a><span data-ttu-id="cd58a-103">Range: LastCell</span><span class="sxs-lookup"><span data-stu-id="cd58a-103">Range: LastCell</span></span>

<span data-ttu-id="cd58a-p101">Ruft die letzte Zelle im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs „B2: D5“ „D5“.</span><span class="sxs-lookup"><span data-stu-id="cd58a-p101">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="cd58a-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd58a-106">Permissions</span></span>
<span data-ttu-id="cd58a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd58a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd58a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd58a-109">Permission type</span></span>      | <span data-ttu-id="cd58a-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd58a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd58a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd58a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd58a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd58a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd58a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd58a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd58a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd58a-114">Not supported.</span></span>    |
|<span data-ttu-id="cd58a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd58a-115">Application</span></span> | <span data-ttu-id="cd58a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd58a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd58a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd58a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastCell
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastCell
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastCell

```
## <a name="request-headers"></a><span data-ttu-id="cd58a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd58a-118">Request headers</span></span>
| <span data-ttu-id="cd58a-119">Name</span><span class="sxs-lookup"><span data-stu-id="cd58a-119">Name</span></span>       | <span data-ttu-id="cd58a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd58a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd58a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd58a-121">Authorization</span></span>  | <span data-ttu-id="cd58a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd58a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd58a-124">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="cd58a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="cd58a-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="cd58a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd58a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd58a-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="cd58a-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd58a-128">Response</span></span>

<span data-ttu-id="cd58a-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd58a-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd58a-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd58a-130">Example</span></span>
<span data-ttu-id="cd58a-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="cd58a-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cd58a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd58a-132">Request</span></span>
<span data-ttu-id="cd58a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd58a-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastCell
```

##### <a name="response"></a><span data-ttu-id="cd58a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd58a-134">Response</span></span>
<span data-ttu-id="cd58a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd58a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastCell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
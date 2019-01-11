---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 3e1aaaee039da7777fc2c32f978ca049900582ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816779"
---
# <a name="range-lastrow"></a><span data-ttu-id="70a23-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="70a23-103">Range: LastRow</span></span>

<span data-ttu-id="70a23-p101">Ruft die letzte Zeile im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs "B2: D5" "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="70a23-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="70a23-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="70a23-106">Permissions</span></span>
<span data-ttu-id="70a23-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70a23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70a23-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70a23-109">Permission type</span></span>      | <span data-ttu-id="70a23-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70a23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70a23-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70a23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70a23-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70a23-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70a23-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70a23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70a23-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70a23-114">Not supported.</span></span>    |
|<span data-ttu-id="70a23-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70a23-115">Application</span></span> | <span data-ttu-id="70a23-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70a23-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70a23-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70a23-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastRow

```
## <a name="request-headers"></a><span data-ttu-id="70a23-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70a23-118">Request headers</span></span>
| <span data-ttu-id="70a23-119">Name</span><span class="sxs-lookup"><span data-stu-id="70a23-119">Name</span></span>       | <span data-ttu-id="70a23-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70a23-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="70a23-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70a23-121">Authorization</span></span>  | <span data-ttu-id="70a23-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="70a23-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70a23-124">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="70a23-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="70a23-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="70a23-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70a23-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70a23-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="70a23-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="70a23-128">Response</span></span>

<span data-ttu-id="70a23-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70a23-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70a23-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70a23-130">Example</span></span>
<span data-ttu-id="70a23-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="70a23-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="70a23-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70a23-132">Request</span></span>
<span data-ttu-id="70a23-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70a23-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastRow
```

##### <a name="response"></a><span data-ttu-id="70a23-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="70a23-134">Response</span></span>
<span data-ttu-id="70a23-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70a23-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

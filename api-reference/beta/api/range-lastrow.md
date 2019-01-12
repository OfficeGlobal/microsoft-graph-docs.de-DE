---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1a3f90c4962c2df11f959c23fccebb2fab289f90
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931427"
---
# <a name="range-lastrow"></a><span data-ttu-id="7a89f-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="7a89f-103">Range: LastRow</span></span>

> <span data-ttu-id="7a89f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a89f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a89f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a89f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a89f-p102">Ruft die letzte Zeile im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs "B2: D5" "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="7a89f-p102">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="7a89f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7a89f-108">Permissions</span></span>
<span data-ttu-id="7a89f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a89f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a89f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a89f-111">Permission type</span></span>      | <span data-ttu-id="7a89f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a89f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a89f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a89f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7a89f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a89f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7a89f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a89f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a89f-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a89f-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7a89f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a89f-117">Application</span></span> | <span data-ttu-id="7a89f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a89f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a89f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a89f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="7a89f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a89f-120">Request headers</span></span>
| <span data-ttu-id="7a89f-121">Name</span><span class="sxs-lookup"><span data-stu-id="7a89f-121">Name</span></span>       | <span data-ttu-id="7a89f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a89f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7a89f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a89f-123">Authorization</span></span>  | <span data-ttu-id="7a89f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a89f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a89f-126">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7a89f-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="7a89f-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7a89f-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a89f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a89f-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7a89f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a89f-130">Response</span></span>

<span data-ttu-id="7a89f-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a89f-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a89f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a89f-132">Example</span></span>
<span data-ttu-id="7a89f-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7a89f-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7a89f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a89f-134">Request</span></span>
<span data-ttu-id="7a89f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a89f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="7a89f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a89f-136">Response</span></span>
<span data-ttu-id="7a89f-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a89f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

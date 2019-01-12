---
title: 'Range: Row'
description: Ruft eine Zelle ab, die im Bereich enthalten ist.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c553923ffcc487f00df045b51511ba2035f2f7ea
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931082"
---
# <a name="range-row"></a><span data-ttu-id="7ce54-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="7ce54-103">Range: Row</span></span>

> <span data-ttu-id="7ce54-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ce54-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ce54-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ce54-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ce54-106">Ruft eine Zelle ab, die im Bereich enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="7ce54-106">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ce54-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7ce54-107">Permissions</span></span>
<span data-ttu-id="7ce54-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ce54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ce54-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ce54-110">Permission type</span></span>      | <span data-ttu-id="7ce54-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ce54-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ce54-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ce54-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ce54-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce54-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ce54-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ce54-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ce54-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce54-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ce54-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ce54-116">Application</span></span> | <span data-ttu-id="7ce54-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ce54-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ce54-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ce54-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/Row
POST /workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="7ce54-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ce54-119">Request headers</span></span>
| <span data-ttu-id="7ce54-120">Name</span><span class="sxs-lookup"><span data-stu-id="7ce54-120">Name</span></span>       | <span data-ttu-id="7ce54-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ce54-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7ce54-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ce54-122">Authorization</span></span>  | <span data-ttu-id="7ce54-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ce54-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ce54-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7ce54-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7ce54-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7ce54-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ce54-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ce54-128">Request body</span></span>
<span data-ttu-id="7ce54-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7ce54-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7ce54-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="7ce54-130">Parameter</span></span>    | <span data-ttu-id="7ce54-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7ce54-131">Type</span></span>   |<span data-ttu-id="7ce54-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ce54-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ce54-133">row</span><span class="sxs-lookup"><span data-stu-id="7ce54-133">row</span></span>|<span data-ttu-id="7ce54-134">number</span><span class="sxs-lookup"><span data-stu-id="7ce54-134">number</span></span>|<span data-ttu-id="7ce54-p105">Zeilenanzahl des abzurufenden Bereichs. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="7ce54-p105">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="7ce54-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ce54-137">Response</span></span>

<span data-ttu-id="7ce54-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ce54-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ce54-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ce54-139">Example</span></span>
<span data-ttu-id="7ce54-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7ce54-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7ce54-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ce54-141">Request</span></span>
<span data-ttu-id="7ce54-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ce54-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_row"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Row
Content-type: application/json
Content-length: 18

{
  "row": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="7ce54-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ce54-143">Response</span></span>
<span data-ttu-id="7ce54-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ce54-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

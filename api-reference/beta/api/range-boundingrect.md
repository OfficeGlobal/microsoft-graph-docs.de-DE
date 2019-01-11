---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 54a8fea095909d199f2cd2b74e2512f6c2f05a6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876615"
---
# <a name="range-boundingrect"></a><span data-ttu-id="c8cfc-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="c8cfc-103">Range: BoundingRect</span></span>

> <span data-ttu-id="c8cfc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8cfc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8cfc-p102">Ruft das kleinste Bereichsobjekt ab, das die angegebenen Bereiche umfasst. Beispielsweise das GetBoundingRect von "B2:C5" und "D10:E15" lautet "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="c8cfc-p102">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="c8cfc-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8cfc-108">Permissions</span></span>
<span data-ttu-id="c8cfc-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8cfc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8cfc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8cfc-111">Permission type</span></span>      | <span data-ttu-id="c8cfc-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8cfc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8cfc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8cfc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c8cfc-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8cfc-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8cfc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8cfc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8cfc-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8cfc-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8cfc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8cfc-117">Application</span></span> | <span data-ttu-id="c8cfc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8cfc-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8cfc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8cfc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="c8cfc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8cfc-120">Request headers</span></span>
| <span data-ttu-id="c8cfc-121">Name</span><span class="sxs-lookup"><span data-stu-id="c8cfc-121">Name</span></span>       | <span data-ttu-id="c8cfc-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8cfc-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8cfc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8cfc-123">Authorization</span></span>  | <span data-ttu-id="c8cfc-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8cfc-126">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c8cfc-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8cfc-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8cfc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8cfc-129">Request body</span></span>
<span data-ttu-id="c8cfc-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8cfc-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="c8cfc-131">Parameter</span></span>    | <span data-ttu-id="c8cfc-132">Typ</span><span class="sxs-lookup"><span data-stu-id="c8cfc-132">Type</span></span>   |<span data-ttu-id="c8cfc-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8cfc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8cfc-134">anotherRange</span><span class="sxs-lookup"><span data-stu-id="c8cfc-134">anotherRange</span></span>|<span data-ttu-id="c8cfc-135">string</span><span class="sxs-lookup"><span data-stu-id="c8cfc-135">string</span></span>|<span data-ttu-id="c8cfc-136">Das Bereichsobjekt oder die Adresse oder der Bereichsname.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-136">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="c8cfc-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8cfc-137">Response</span></span>

<span data-ttu-id="c8cfc-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8cfc-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8cfc-139">Example</span></span>
<span data-ttu-id="c8cfc-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8cfc-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8cfc-141">Request</span></span>
<span data-ttu-id="c8cfc-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="c8cfc-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8cfc-143">Response</span></span>
<span data-ttu-id="c8cfc-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8cfc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

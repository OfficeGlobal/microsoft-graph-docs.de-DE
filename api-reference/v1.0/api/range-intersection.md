---
title: 'Range: Intersection'
description: Ruft das Bereichsobjekt ab, das die rechteckige Schnittmenge der angegebenen Bereiche darstellt.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 95e7af555c1ac857272994dc634ed0dc9f1b0fad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951635"
---
# <a name="range-intersection"></a><span data-ttu-id="19f91-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="19f91-103">Range: Intersection</span></span>

<span data-ttu-id="19f91-104">Ruft das Bereichsobjekt ab, das die rechteckige Schnittmenge der angegebenen Bereiche darstellt.</span><span class="sxs-lookup"><span data-stu-id="19f91-104">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="19f91-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="19f91-105">Permissions</span></span>
<span data-ttu-id="19f91-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19f91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19f91-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19f91-108">Permission type</span></span>      | <span data-ttu-id="19f91-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19f91-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19f91-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19f91-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19f91-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19f91-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19f91-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19f91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19f91-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19f91-113">Not supported.</span></span>    |
|<span data-ttu-id="19f91-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19f91-114">Application</span></span> | <span data-ttu-id="19f91-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19f91-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19f91-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19f91-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="19f91-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19f91-117">Request headers</span></span>
| <span data-ttu-id="19f91-118">Name</span><span class="sxs-lookup"><span data-stu-id="19f91-118">Name</span></span>       | <span data-ttu-id="19f91-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19f91-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19f91-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="19f91-120">Authorization</span></span>  | <span data-ttu-id="19f91-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19f91-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19f91-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="19f91-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="19f91-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="19f91-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19f91-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19f91-126">Request body</span></span>
<span data-ttu-id="19f91-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="19f91-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19f91-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="19f91-128">Parameter</span></span>    | <span data-ttu-id="19f91-129">Typ</span><span class="sxs-lookup"><span data-stu-id="19f91-129">Type</span></span>   |<span data-ttu-id="19f91-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19f91-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19f91-131">anotherRange</span><span class="sxs-lookup"><span data-stu-id="19f91-131">anotherRange</span></span>|<span data-ttu-id="19f91-132">string</span><span class="sxs-lookup"><span data-stu-id="19f91-132">string</span></span>|<span data-ttu-id="19f91-133">Das Bereichsobjekt oder die Bereichsadresse, die verwendet wird, um die Schnittmenge der Bereiche zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="19f91-133">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="19f91-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="19f91-134">Response</span></span>

<span data-ttu-id="19f91-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19f91-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19f91-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19f91-136">Example</span></span>
<span data-ttu-id="19f91-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="19f91-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19f91-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19f91-138">Request</span></span>
<span data-ttu-id="19f91-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19f91-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="19f91-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="19f91-140">Response</span></span>
<span data-ttu-id="19f91-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19f91-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

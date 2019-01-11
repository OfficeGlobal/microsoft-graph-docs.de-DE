---
title: 'Range: UsedRange'
description: Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 980d0cc8ac59c28e148a50c25b90b52baad51110
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889929"
---
# <a name="range-usedrange"></a><span data-ttu-id="1baee-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="1baee-103">Range: UsedRange</span></span>

<span data-ttu-id="1baee-104">Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.</span><span class="sxs-lookup"><span data-stu-id="1baee-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1baee-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1baee-105">Permissions</span></span>
<span data-ttu-id="1baee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1baee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1baee-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1baee-108">Permission type</span></span>      | <span data-ttu-id="1baee-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1baee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1baee-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1baee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1baee-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1baee-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1baee-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1baee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1baee-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1baee-113">Not supported.</span></span>    |
|<span data-ttu-id="1baee-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1baee-114">Application</span></span> | <span data-ttu-id="1baee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1baee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1baee-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1baee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="1baee-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1baee-117">Request headers</span></span>
| <span data-ttu-id="1baee-118">Name</span><span class="sxs-lookup"><span data-stu-id="1baee-118">Name</span></span>       | <span data-ttu-id="1baee-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1baee-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1baee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1baee-120">Authorization</span></span>  | <span data-ttu-id="1baee-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1baee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1baee-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1baee-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1baee-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1baee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="1baee-126">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="1baee-126">Path parameters</span></span>
| <span data-ttu-id="1baee-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="1baee-127">Parameter</span></span>    | <span data-ttu-id="1baee-128">Typ</span><span class="sxs-lookup"><span data-stu-id="1baee-128">Type</span></span>   |<span data-ttu-id="1baee-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1baee-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1baee-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="1baee-130">valuesOnly</span></span>|<span data-ttu-id="1baee-131">boolean</span><span class="sxs-lookup"><span data-stu-id="1baee-131">boolean</span></span>|<span data-ttu-id="1baee-p104">Optional. Betrachtet nur Zellen mit Werten als verwendet.</span><span class="sxs-lookup"><span data-stu-id="1baee-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="1baee-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1baee-134">Response</span></span>

<span data-ttu-id="1baee-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1baee-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1baee-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1baee-136">Example</span></span>
<span data-ttu-id="1baee-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1baee-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1baee-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1baee-138">Request</span></span>
<span data-ttu-id="1baee-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1baee-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="1baee-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1baee-140">Response</span></span>
<span data-ttu-id="1baee-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1baee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="1baee-144">Es folgt ein Beispiel, Angeben der optionalen `valuesOnly` Parameter.</span><span class="sxs-lookup"><span data-stu-id="1baee-144">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="1baee-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1baee-145">Request</span></span>
<span data-ttu-id="1baee-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1baee-146">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="1baee-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="1baee-147">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

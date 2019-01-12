---
title: 'Range: UsedRange'
description: Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0ae8f8bec1eea6f2e13b4c4248d55afbb28cf19d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928066"
---
# <a name="range-usedrange"></a><span data-ttu-id="cbdd3-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="cbdd3-103">Range: UsedRange</span></span>

> <span data-ttu-id="cbdd3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbdd3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbdd3-106">Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-106">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbdd3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cbdd3-107">Permissions</span></span>
<span data-ttu-id="cbdd3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbdd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbdd3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cbdd3-110">Permission type</span></span>      | <span data-ttu-id="cbdd3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cbdd3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbdd3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cbdd3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cbdd3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbdd3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbdd3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cbdd3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbdd3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbdd3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbdd3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cbdd3-116">Application</span></span> | <span data-ttu-id="cbdd3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbdd3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbdd3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbdd3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="cbdd3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cbdd3-119">Request headers</span></span>
| <span data-ttu-id="cbdd3-120">Name</span><span class="sxs-lookup"><span data-stu-id="cbdd3-120">Name</span></span>       | <span data-ttu-id="cbdd3-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbdd3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cbdd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbdd3-122">Authorization</span></span>  | <span data-ttu-id="cbdd3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbdd3-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="cbdd3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cbdd3-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbdd3-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cbdd3-128">Request body</span></span>
<span data-ttu-id="cbdd3-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cbdd3-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="cbdd3-130">Parameter</span></span>    | <span data-ttu-id="cbdd3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cbdd3-131">Type</span></span>   |<span data-ttu-id="cbdd3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbdd3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbdd3-133">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="cbdd3-133">valuesOnly</span></span>|<span data-ttu-id="cbdd3-134">boolean</span><span class="sxs-lookup"><span data-stu-id="cbdd3-134">boolean</span></span>|<span data-ttu-id="cbdd3-p105">Optional. Betrachtet nur Zellen mit Werten als verwendet.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-p105">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="cbdd3-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbdd3-137">Response</span></span>

<span data-ttu-id="cbdd3-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbdd3-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cbdd3-139">Example</span></span>
<span data-ttu-id="cbdd3-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cbdd3-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbdd3-141">Request</span></span>
<span data-ttu-id="cbdd3-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="cbdd3-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbdd3-143">Response</span></span>
<span data-ttu-id="cbdd3-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbdd3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'Arbeitsblatt: Range'
description: Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e7dade7e0c83808aa10700e87dd54a1e8fe9bb7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971970"
---
# <a name="worksheet-range"></a><span data-ttu-id="3a2c2-103">Arbeitsblatt: Range</span><span class="sxs-lookup"><span data-stu-id="3a2c2-103">Worksheet: Range</span></span>

<span data-ttu-id="3a2c2-104">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a2c2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a2c2-105">Permissions</span></span>
<span data-ttu-id="3a2c2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a2c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a2c2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a2c2-108">Permission type</span></span>      | <span data-ttu-id="3a2c2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a2c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a2c2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a2c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a2c2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a2c2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a2c2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a2c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a2c2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a2c2-113">Not supported.</span></span>    |
|<span data-ttu-id="3a2c2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a2c2-114">Application</span></span> | <span data-ttu-id="3a2c2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a2c2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a2c2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a2c2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="3a2c2-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a2c2-117">Request headers</span></span>
| <span data-ttu-id="3a2c2-118">Name</span><span class="sxs-lookup"><span data-stu-id="3a2c2-118">Name</span></span>       | <span data-ttu-id="3a2c2-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a2c2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a2c2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a2c2-120">Authorization</span></span>  | <span data-ttu-id="3a2c2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a2c2-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3a2c2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3a2c2-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="3a2c2-126">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="3a2c2-126">Function parameters</span></span>

| <span data-ttu-id="3a2c2-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="3a2c2-127">Parameter</span></span>    | <span data-ttu-id="3a2c2-128">Typ</span><span class="sxs-lookup"><span data-stu-id="3a2c2-128">Type</span></span>   |<span data-ttu-id="3a2c2-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a2c2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a2c2-130">address</span><span class="sxs-lookup"><span data-stu-id="3a2c2-130">address</span></span>|<span data-ttu-id="3a2c2-131">string</span><span class="sxs-lookup"><span data-stu-id="3a2c2-131">string</span></span>|<span data-ttu-id="3a2c2-p104">Optional. Die Adresse oder der Name des Bereichs. Wenn nichts angegeben ist, wird der gesamte Arbeitsblattbereich zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="3a2c2-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a2c2-135">Response</span></span>

<span data-ttu-id="3a2c2-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a2c2-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a2c2-137">Example</span></span>
<span data-ttu-id="3a2c2-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a2c2-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a2c2-139">Request</span></span>
<span data-ttu-id="3a2c2-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="3a2c2-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a2c2-141">Response</span></span>
<span data-ttu-id="3a2c2-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="3a2c2-145">Wenn die optionalen `address` Parameter nicht angegeben ist, diese Funktion gibt den gesamte Arbeitsblattbereich zurück.</span><span class="sxs-lookup"><span data-stu-id="3a2c2-145">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="3a2c2-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a2c2-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="3a2c2-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a2c2-147">Response</span></span>

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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

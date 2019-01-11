---
title: 'Range: insert'
description: Fügt eine Zelle oder einen Zellbereich in das Arbeitsblatt anstelle dieses Bereichs ein, und verschiebt die anderen Zellen, um Platz zu schaffen. Gibt ein neues Bereichsobjekt in dem nun leeren Bereich zurück.
localization_priority: Normal
ms.openlocfilehash: 78cd2d4018a96428b7e5336d00ca20bada4abd36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804872"
---
# <a name="range-insert"></a><span data-ttu-id="f8a82-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="f8a82-104">Range: insert</span></span>

<span data-ttu-id="f8a82-p102">Fügt eine Zelle oder einen Zellbereich in das Arbeitsblatt anstelle dieses Bereichs ein, und verschiebt die anderen Zellen, um Platz zu schaffen. Gibt ein neues Bereichsobjekt in dem nun leeren Bereich zurück.</span><span class="sxs-lookup"><span data-stu-id="f8a82-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8a82-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f8a82-107">Permissions</span></span>
<span data-ttu-id="f8a82-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8a82-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8a82-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8a82-110">Permission type</span></span>      | <span data-ttu-id="f8a82-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8a82-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8a82-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8a82-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f8a82-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8a82-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f8a82-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8a82-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8a82-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8a82-115">Not supported.</span></span>    |
|<span data-ttu-id="f8a82-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8a82-116">Application</span></span> | <span data-ttu-id="f8a82-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8a82-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8a82-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8a82-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="f8a82-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8a82-119">Request headers</span></span>
| <span data-ttu-id="f8a82-120">Name</span><span class="sxs-lookup"><span data-stu-id="f8a82-120">Name</span></span>       | <span data-ttu-id="f8a82-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8a82-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8a82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8a82-122">Authorization</span></span>  | <span data-ttu-id="f8a82-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f8a82-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8a82-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="f8a82-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f8a82-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="f8a82-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8a82-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8a82-128">Request body</span></span>
<span data-ttu-id="f8a82-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f8a82-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8a82-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="f8a82-130">Parameter</span></span>    | <span data-ttu-id="f8a82-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f8a82-131">Type</span></span>   |<span data-ttu-id="f8a82-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8a82-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8a82-133">Shift</span><span class="sxs-lookup"><span data-stu-id="f8a82-133">shift</span></span>|<span data-ttu-id="f8a82-134">string</span><span class="sxs-lookup"><span data-stu-id="f8a82-134">string</span></span>|<span data-ttu-id="f8a82-135">Gibt an, wie die Zellen verschoben.</span><span class="sxs-lookup"><span data-stu-id="f8a82-135">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="f8a82-136">Die möglichen Werte sind: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="f8a82-136">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="f8a82-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8a82-137">Response</span></span>

<span data-ttu-id="f8a82-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8a82-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8a82-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8a82-139">Example</span></span>
<span data-ttu-id="f8a82-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f8a82-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f8a82-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8a82-141">Request</span></span>
<span data-ttu-id="f8a82-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8a82-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="f8a82-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8a82-143">Response</span></span>
<span data-ttu-id="f8a82-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8a82-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

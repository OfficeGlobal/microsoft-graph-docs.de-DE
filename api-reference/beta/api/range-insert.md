---
title: 'Range: insert'
description: Fügt eine Zelle oder einen Zellbereich in das Arbeitsblatt anstelle dieses Bereichs ein, und verschiebt die anderen Zellen, um Platz zu schaffen. Gibt ein neues Bereichsobjekt in dem nun leeren Bereich zurück.
ms.openlocfilehash: 57068d081cccf05f06adf966b476df60c482574e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063679"
---
# <a name="range-insert"></a><span data-ttu-id="60a2c-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="60a2c-104">Range: insert</span></span>

> <span data-ttu-id="60a2c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="60a2c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60a2c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60a2c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60a2c-p103">Fügt eine Zelle oder einen Zellbereich in das Arbeitsblatt anstelle dieses Bereichs ein, und verschiebt die anderen Zellen, um Platz zu schaffen. Gibt ein neues Bereichsobjekt in dem nun leeren Bereich zurück.</span><span class="sxs-lookup"><span data-stu-id="60a2c-p103">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="60a2c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="60a2c-109">Permissions</span></span>
<span data-ttu-id="60a2c-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60a2c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a2c-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60a2c-112">Permission type</span></span>      | <span data-ttu-id="60a2c-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60a2c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60a2c-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60a2c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="60a2c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60a2c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60a2c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60a2c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a2c-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60a2c-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="60a2c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60a2c-118">Application</span></span> | <span data-ttu-id="60a2c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60a2c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60a2c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60a2c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="60a2c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60a2c-121">Request headers</span></span>
| <span data-ttu-id="60a2c-122">Name</span><span class="sxs-lookup"><span data-stu-id="60a2c-122">Name</span></span>       | <span data-ttu-id="60a2c-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60a2c-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60a2c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a2c-124">Authorization</span></span>  | <span data-ttu-id="60a2c-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60a2c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60a2c-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="60a2c-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="60a2c-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="60a2c-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60a2c-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60a2c-130">Request body</span></span>
<span data-ttu-id="60a2c-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="60a2c-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60a2c-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="60a2c-132">Parameter</span></span>    | <span data-ttu-id="60a2c-133">Typ</span><span class="sxs-lookup"><span data-stu-id="60a2c-133">Type</span></span>   |<span data-ttu-id="60a2c-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60a2c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60a2c-135">Shift</span><span class="sxs-lookup"><span data-stu-id="60a2c-135">shift</span></span>|<span data-ttu-id="60a2c-136">string</span><span class="sxs-lookup"><span data-stu-id="60a2c-136">string</span></span>|<span data-ttu-id="60a2c-p107">Gibt an, wohin die Zellen verschoben werden.  Mögliche Werte: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="60a2c-p107">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="60a2c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="60a2c-139">Response</span></span>

<span data-ttu-id="60a2c-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60a2c-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60a2c-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60a2c-141">Example</span></span>
<span data-ttu-id="60a2c-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="60a2c-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="60a2c-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60a2c-143">Request</span></span>
<span data-ttu-id="60a2c-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60a2c-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="60a2c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="60a2c-145">Response</span></span>
<span data-ttu-id="60a2c-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60a2c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
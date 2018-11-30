---
title: 'TableColumnCollection: ItemAt'
description: Ruft eine Spalte anhand ihrer Position in der Auflistung ab.
ms.openlocfilehash: adac794a9e3648c86b09283824456cb2c555d92c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016654"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="76ad3-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="76ad3-103">TableColumnCollection: ItemAt</span></span>

<span data-ttu-id="76ad3-104">Ruft eine Spalte anhand ihrer Position in der Auflistung ab.</span><span class="sxs-lookup"><span data-stu-id="76ad3-104">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="76ad3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="76ad3-105">Permissions</span></span>
<span data-ttu-id="76ad3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76ad3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76ad3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76ad3-108">Permission type</span></span>      | <span data-ttu-id="76ad3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76ad3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76ad3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76ad3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76ad3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76ad3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="76ad3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76ad3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76ad3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76ad3-113">Not supported.</span></span>    |
|<span data-ttu-id="76ad3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76ad3-114">Application</span></span> | <span data-ttu-id="76ad3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76ad3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76ad3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76ad3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="76ad3-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76ad3-117">Request headers</span></span>
| <span data-ttu-id="76ad3-118">Name</span><span class="sxs-lookup"><span data-stu-id="76ad3-118">Name</span></span>       | <span data-ttu-id="76ad3-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76ad3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="76ad3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="76ad3-120">Authorization</span></span>  | <span data-ttu-id="76ad3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="76ad3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76ad3-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="76ad3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="76ad3-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="76ad3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76ad3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76ad3-126">Request body</span></span>
<span data-ttu-id="76ad3-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="76ad3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76ad3-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="76ad3-128">Parameter</span></span>    | <span data-ttu-id="76ad3-129">Typ</span><span class="sxs-lookup"><span data-stu-id="76ad3-129">Type</span></span>   |<span data-ttu-id="76ad3-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76ad3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76ad3-131">Index</span><span class="sxs-lookup"><span data-stu-id="76ad3-131">index</span></span>|<span data-ttu-id="76ad3-132">Int32</span><span class="sxs-lookup"><span data-stu-id="76ad3-132">Int32</span></span>|<span data-ttu-id="76ad3-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="76ad3-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="76ad3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="76ad3-135">Response</span></span>

<span data-ttu-id="76ad3-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookTableColumn](../resources/tablecolumn.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="76ad3-136">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76ad3-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76ad3-137">Example</span></span>
<span data-ttu-id="76ad3-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="76ad3-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76ad3-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76ad3-139">Request</span></span>
<span data-ttu-id="76ad3-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76ad3-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumncollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 3
}
```

##### <a name="response"></a><span data-ttu-id="76ad3-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="76ad3-141">Response</span></span>
<span data-ttu-id="76ad3-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76ad3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: 'TableRowCollection: ItemAt'
description: Ruft eine Zeile anhand ihrer Position in der Auflistung ab.
ms.openlocfilehash: 786e4cfb4ea9cbe86d2dff222a31737ab487b68f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019519"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="b18bd-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="b18bd-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="b18bd-104">Ruft eine Zeile anhand ihrer Position in der Auflistung ab.</span><span class="sxs-lookup"><span data-stu-id="b18bd-104">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="b18bd-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b18bd-105">Permissions</span></span>
<span data-ttu-id="b18bd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b18bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b18bd-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b18bd-108">Permission type</span></span>      | <span data-ttu-id="b18bd-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b18bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b18bd-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b18bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b18bd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b18bd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b18bd-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b18bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b18bd-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b18bd-113">Not supported.</span></span>    |
|<span data-ttu-id="b18bd-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b18bd-114">Application</span></span> | <span data-ttu-id="b18bd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b18bd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b18bd-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b18bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="b18bd-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b18bd-117">Request headers</span></span>
| <span data-ttu-id="b18bd-118">Name</span><span class="sxs-lookup"><span data-stu-id="b18bd-118">Name</span></span>       | <span data-ttu-id="b18bd-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b18bd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b18bd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b18bd-120">Authorization</span></span>  | <span data-ttu-id="b18bd-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b18bd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b18bd-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b18bd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b18bd-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b18bd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b18bd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b18bd-126">Request body</span></span>
<span data-ttu-id="b18bd-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b18bd-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b18bd-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="b18bd-128">Parameter</span></span>    | <span data-ttu-id="b18bd-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b18bd-129">Type</span></span>   |<span data-ttu-id="b18bd-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b18bd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b18bd-131">Index</span><span class="sxs-lookup"><span data-stu-id="b18bd-131">index</span></span>|<span data-ttu-id="b18bd-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b18bd-132">Int32</span></span>|<span data-ttu-id="b18bd-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="b18bd-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="b18bd-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b18bd-135">Response</span></span>

<span data-ttu-id="b18bd-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookTableRow](../resources/tablerow.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b18bd-136">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b18bd-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b18bd-137">Example</span></span>
<span data-ttu-id="b18bd-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b18bd-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b18bd-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b18bd-139">Request</span></span>
<span data-ttu-id="b18bd-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b18bd-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerowcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 4
}
```

##### <a name="response"></a><span data-ttu-id="b18bd-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b18bd-141">Response</span></span>
<span data-ttu-id="b18bd-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b18bd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
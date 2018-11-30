---
title: 'RangeBorderCollection: ItemAt'
description: Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.
ms.openlocfilehash: d62202f5d2678152af69e8c4b6b058d6f2ddcdaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017543"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="cf702-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="cf702-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="cf702-104">Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.</span><span class="sxs-lookup"><span data-stu-id="cf702-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="cf702-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cf702-105">Permissions</span></span>
<span data-ttu-id="cf702-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf702-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf702-108">Permission type</span></span>      | <span data-ttu-id="cf702-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf702-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf702-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf702-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf702-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf702-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cf702-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf702-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf702-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf702-113">Not supported.</span></span>    |
|<span data-ttu-id="cf702-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf702-114">Application</span></span> | <span data-ttu-id="cf702-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf702-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf702-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf702-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="cf702-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf702-117">Request headers</span></span>
| <span data-ttu-id="cf702-118">Name</span><span class="sxs-lookup"><span data-stu-id="cf702-118">Name</span></span>       | <span data-ttu-id="cf702-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf702-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cf702-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf702-120">Authorization</span></span>  | <span data-ttu-id="cf702-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf702-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf702-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="cf702-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cf702-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="cf702-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf702-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf702-126">Request body</span></span>
<span data-ttu-id="cf702-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="cf702-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cf702-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="cf702-128">Parameter</span></span>    | <span data-ttu-id="cf702-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cf702-129">Type</span></span>   |<span data-ttu-id="cf702-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf702-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf702-131">Index</span><span class="sxs-lookup"><span data-stu-id="cf702-131">index</span></span>|<span data-ttu-id="cf702-132">Int32</span><span class="sxs-lookup"><span data-stu-id="cf702-132">Int32</span></span>|<span data-ttu-id="cf702-p104">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="cf702-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="cf702-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf702-135">Response</span></span>

<span data-ttu-id="cf702-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookRangeBorder](../resources/rangeborder.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cf702-136">If successful, this method returns `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf702-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf702-137">Example</span></span>
<span data-ttu-id="cf702-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="cf702-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cf702-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf702-139">Request</span></span>
<span data-ttu-id="cf702-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf702-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "rangebordercollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 1
}
```

##### <a name="response"></a><span data-ttu-id="cf702-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf702-141">Response</span></span>
<span data-ttu-id="cf702-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf702-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
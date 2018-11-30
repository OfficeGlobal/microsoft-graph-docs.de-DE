---
title: 'Range: UsedRange'
description: Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.
ms.openlocfilehash: 106c3e04f564bdfa529c0a5e6ad17cda3200d436
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058133"
---
# <a name="range-usedrange"></a><span data-ttu-id="7ddfe-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="7ddfe-103">Range: UsedRange</span></span>

> <span data-ttu-id="7ddfe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ddfe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ddfe-106">Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-106">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ddfe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7ddfe-107">Permissions</span></span>
<span data-ttu-id="7ddfe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ddfe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ddfe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ddfe-110">Permission type</span></span>      | <span data-ttu-id="7ddfe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ddfe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ddfe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ddfe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ddfe-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ddfe-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ddfe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ddfe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ddfe-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ddfe-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ddfe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ddfe-116">Application</span></span> | <span data-ttu-id="7ddfe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ddfe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ddfe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ddfe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="7ddfe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ddfe-119">Request headers</span></span>
| <span data-ttu-id="7ddfe-120">Name</span><span class="sxs-lookup"><span data-stu-id="7ddfe-120">Name</span></span>       | <span data-ttu-id="7ddfe-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ddfe-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7ddfe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ddfe-122">Authorization</span></span>  | <span data-ttu-id="7ddfe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ddfe-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7ddfe-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7ddfe-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ddfe-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ddfe-128">Request body</span></span>
<span data-ttu-id="7ddfe-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7ddfe-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="7ddfe-130">Parameter</span></span>    | <span data-ttu-id="7ddfe-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7ddfe-131">Type</span></span>   |<span data-ttu-id="7ddfe-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ddfe-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ddfe-133">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="7ddfe-133">valuesOnly</span></span>|<span data-ttu-id="7ddfe-134">boolean</span><span class="sxs-lookup"><span data-stu-id="7ddfe-134">boolean</span></span>|<span data-ttu-id="7ddfe-p105">Optional. Betrachtet nur Zellen mit Werten als verwendet.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-p105">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="7ddfe-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ddfe-137">Response</span></span>

<span data-ttu-id="7ddfe-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ddfe-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ddfe-139">Example</span></span>
<span data-ttu-id="7ddfe-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7ddfe-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ddfe-141">Request</span></span>
<span data-ttu-id="7ddfe-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7ddfe-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ddfe-143">Response</span></span>
<span data-ttu-id="7ddfe-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ddfe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
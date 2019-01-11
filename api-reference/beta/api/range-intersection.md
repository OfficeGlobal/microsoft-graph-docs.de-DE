---
title: 'Range: Intersection'
description: Ruft das Bereichsobjekt ab, das die rechteckige Schnittmenge der angegebenen Bereiche darstellt.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 093a86daa5b80337bb5f760185f55e8a06f4b37a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877819"
---
# <a name="range-intersection"></a><span data-ttu-id="5582e-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="5582e-103">Range: Intersection</span></span>

> <span data-ttu-id="5582e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5582e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5582e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5582e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5582e-106">Ruft das Bereichsobjekt ab, das die rechteckige Schnittmenge der angegebenen Bereiche darstellt.</span><span class="sxs-lookup"><span data-stu-id="5582e-106">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="5582e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5582e-107">Permissions</span></span>
<span data-ttu-id="5582e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5582e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5582e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5582e-110">Permission type</span></span>      | <span data-ttu-id="5582e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5582e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5582e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5582e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5582e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5582e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5582e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5582e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5582e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5582e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5582e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5582e-116">Application</span></span> | <span data-ttu-id="5582e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5582e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5582e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5582e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="5582e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5582e-119">Request headers</span></span>
| <span data-ttu-id="5582e-120">Name</span><span class="sxs-lookup"><span data-stu-id="5582e-120">Name</span></span>       | <span data-ttu-id="5582e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5582e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5582e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5582e-122">Authorization</span></span>  | <span data-ttu-id="5582e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5582e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5582e-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5582e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5582e-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5582e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5582e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5582e-128">Request body</span></span>
<span data-ttu-id="5582e-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="5582e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5582e-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="5582e-130">Parameter</span></span>    | <span data-ttu-id="5582e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5582e-131">Type</span></span>   |<span data-ttu-id="5582e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5582e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5582e-133">anotherRange</span><span class="sxs-lookup"><span data-stu-id="5582e-133">anotherRange</span></span>|<span data-ttu-id="5582e-134">string</span><span class="sxs-lookup"><span data-stu-id="5582e-134">string</span></span>|<span data-ttu-id="5582e-135">Das Bereichsobjekt oder die Bereichsadresse, die verwendet wird, um die Schnittmenge der Bereiche zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="5582e-135">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="5582e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5582e-136">Response</span></span>

<span data-ttu-id="5582e-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5582e-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5582e-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5582e-138">Example</span></span>
<span data-ttu-id="5582e-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5582e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5582e-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5582e-140">Request</span></span>
<span data-ttu-id="5582e-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5582e-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="5582e-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="5582e-142">Response</span></span>
<span data-ttu-id="5582e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5582e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

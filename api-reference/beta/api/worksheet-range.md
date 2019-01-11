---
title: 'Arbeitsblatt: Range'
description: Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 78865ab8f7e4aa7d59bb6f3c782731bae058ae80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860669"
---
# <a name="worksheet-range"></a><span data-ttu-id="bc594-103">Arbeitsblatt: Range</span><span class="sxs-lookup"><span data-stu-id="bc594-103">Worksheet: Range</span></span>

> <span data-ttu-id="bc594-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bc594-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc594-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc594-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc594-106">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="bc594-106">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc594-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc594-107">Permissions</span></span>
<span data-ttu-id="bc594-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc594-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc594-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc594-110">Permission type</span></span>      | <span data-ttu-id="bc594-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc594-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc594-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc594-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc594-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc594-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc594-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc594-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc594-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc594-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc594-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc594-116">Application</span></span> | <span data-ttu-id="bc594-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc594-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc594-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc594-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="bc594-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc594-119">Request headers</span></span>
| <span data-ttu-id="bc594-120">Name</span><span class="sxs-lookup"><span data-stu-id="bc594-120">Name</span></span>       | <span data-ttu-id="bc594-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc594-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc594-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc594-122">Authorization</span></span>  | <span data-ttu-id="bc594-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc594-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc594-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="bc594-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc594-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="bc594-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc594-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc594-128">Request body</span></span>
<span data-ttu-id="bc594-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="bc594-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bc594-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="bc594-130">Parameter</span></span>    | <span data-ttu-id="bc594-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bc594-131">Type</span></span>   |<span data-ttu-id="bc594-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc594-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc594-133">address</span><span class="sxs-lookup"><span data-stu-id="bc594-133">address</span></span>|<span data-ttu-id="bc594-134">string</span><span class="sxs-lookup"><span data-stu-id="bc594-134">string</span></span>|<span data-ttu-id="bc594-p105">Optional. Die Adresse oder der Name des Bereichs. Wenn nichts angegeben ist, wird der gesamte Arbeitsblattbereich zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc594-p105">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="bc594-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc594-138">Response</span></span>

<span data-ttu-id="bc594-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc594-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc594-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc594-140">Example</span></span>
<span data-ttu-id="bc594-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="bc594-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bc594-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc594-142">Request</span></span>
<span data-ttu-id="bc594-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc594-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="bc594-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc594-144">Response</span></span>
<span data-ttu-id="bc594-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc594-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

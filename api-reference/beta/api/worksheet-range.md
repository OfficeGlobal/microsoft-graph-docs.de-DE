---
title: 'Arbeitsblatt: Range'
description: Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3d4241e6aeccd0d400388e03a4ce1254df7d0dc0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970997"
---
# <a name="worksheet-range"></a><span data-ttu-id="b9999-103">Arbeitsblatt: Range</span><span class="sxs-lookup"><span data-stu-id="b9999-103">Worksheet: Range</span></span>

> <span data-ttu-id="b9999-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9999-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9999-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9999-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9999-106">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="b9999-106">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9999-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9999-107">Permissions</span></span>
<span data-ttu-id="b9999-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9999-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9999-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9999-110">Permission type</span></span>      | <span data-ttu-id="b9999-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9999-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9999-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9999-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9999-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9999-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9999-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9999-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9999-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9999-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9999-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9999-116">Application</span></span> | <span data-ttu-id="b9999-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9999-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9999-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9999-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="b9999-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9999-119">Request headers</span></span>
| <span data-ttu-id="b9999-120">Name</span><span class="sxs-lookup"><span data-stu-id="b9999-120">Name</span></span>       | <span data-ttu-id="b9999-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9999-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9999-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9999-122">Authorization</span></span>  | <span data-ttu-id="b9999-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b9999-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9999-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b9999-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9999-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b9999-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9999-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9999-128">Request body</span></span>
<span data-ttu-id="b9999-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b9999-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9999-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="b9999-130">Parameter</span></span>    | <span data-ttu-id="b9999-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b9999-131">Type</span></span>   |<span data-ttu-id="b9999-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9999-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9999-133">address</span><span class="sxs-lookup"><span data-stu-id="b9999-133">address</span></span>|<span data-ttu-id="b9999-134">string</span><span class="sxs-lookup"><span data-stu-id="b9999-134">string</span></span>|<span data-ttu-id="b9999-p105">Optional. Die Adresse oder der Name des Bereichs. Wenn nichts angegeben ist, wird der gesamte Arbeitsblattbereich zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9999-p105">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="b9999-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9999-138">Response</span></span>

<span data-ttu-id="b9999-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9999-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9999-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9999-140">Example</span></span>
<span data-ttu-id="b9999-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b9999-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9999-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9999-142">Request</span></span>
<span data-ttu-id="b9999-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9999-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b9999-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9999-144">Response</span></span>
<span data-ttu-id="b9999-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9999-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

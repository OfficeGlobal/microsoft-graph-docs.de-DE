---
title: 'Arbeitsblatt: Range'
description: Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.
ms.openlocfilehash: defe05f953d5fe7cd5fafda6ae16f04bb9f91e86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062742"
---
# <a name="worksheet-range"></a><span data-ttu-id="5071e-103">Arbeitsblatt: Range</span><span class="sxs-lookup"><span data-stu-id="5071e-103">Worksheet: Range</span></span>

> <span data-ttu-id="5071e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5071e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5071e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5071e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5071e-106">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="5071e-106">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="5071e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5071e-107">Permissions</span></span>
<span data-ttu-id="5071e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5071e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5071e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5071e-110">Permission type</span></span>      | <span data-ttu-id="5071e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5071e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5071e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5071e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5071e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5071e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5071e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5071e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5071e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5071e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5071e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5071e-116">Application</span></span> | <span data-ttu-id="5071e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5071e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5071e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5071e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="5071e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5071e-119">Request headers</span></span>
| <span data-ttu-id="5071e-120">Name</span><span class="sxs-lookup"><span data-stu-id="5071e-120">Name</span></span>       | <span data-ttu-id="5071e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5071e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5071e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5071e-122">Authorization</span></span>  | <span data-ttu-id="5071e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5071e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5071e-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5071e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5071e-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5071e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5071e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5071e-128">Request body</span></span>
<span data-ttu-id="5071e-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="5071e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5071e-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="5071e-130">Parameter</span></span>    | <span data-ttu-id="5071e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5071e-131">Type</span></span>   |<span data-ttu-id="5071e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5071e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5071e-133">address</span><span class="sxs-lookup"><span data-stu-id="5071e-133">address</span></span>|<span data-ttu-id="5071e-134">string</span><span class="sxs-lookup"><span data-stu-id="5071e-134">string</span></span>|<span data-ttu-id="5071e-p105">Optional. Die Adresse oder der Name des Bereichs. Wenn nichts angegeben ist, wird der gesamte Arbeitsblattbereich zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5071e-p105">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="5071e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5071e-138">Response</span></span>

<span data-ttu-id="5071e-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5071e-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5071e-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5071e-140">Example</span></span>
<span data-ttu-id="5071e-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5071e-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5071e-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5071e-142">Request</span></span>
<span data-ttu-id="5071e-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5071e-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5071e-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="5071e-144">Response</span></span>
<span data-ttu-id="5071e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5071e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
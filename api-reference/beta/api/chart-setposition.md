---
title: 'Chart: setPosition'
description: Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dae44414db5a095c4cf12506582a9533972a0373
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941219"
---
# <a name="chart-setposition"></a><span data-ttu-id="1d4c2-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="1d4c2-103">Chart: setPosition</span></span>

> <span data-ttu-id="1d4c2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d4c2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d4c2-106">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-106">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d4c2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1d4c2-107">Permissions</span></span>
<span data-ttu-id="1d4c2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d4c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d4c2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d4c2-110">Permission type</span></span>      | <span data-ttu-id="1d4c2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d4c2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d4c2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d4c2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d4c2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d4c2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d4c2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d4c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d4c2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d4c2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d4c2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d4c2-116">Application</span></span> | <span data-ttu-id="1d4c2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d4c2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d4c2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d4c2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="1d4c2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d4c2-119">Request headers</span></span>
| <span data-ttu-id="1d4c2-120">Name</span><span class="sxs-lookup"><span data-stu-id="1d4c2-120">Name</span></span>       | <span data-ttu-id="1d4c2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d4c2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1d4c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d4c2-122">Authorization</span></span>  | <span data-ttu-id="1d4c2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d4c2-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1d4c2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1d4c2-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d4c2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d4c2-128">Request body</span></span>
<span data-ttu-id="1d4c2-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1d4c2-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="1d4c2-130">Parameter</span></span>    | <span data-ttu-id="1d4c2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1d4c2-131">Type</span></span>   |<span data-ttu-id="1d4c2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d4c2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d4c2-133">startCell</span><span class="sxs-lookup"><span data-stu-id="1d4c2-133">startCell</span></span>|<span data-ttu-id="1d4c2-134">string</span><span class="sxs-lookup"><span data-stu-id="1d4c2-134">string</span></span>|<span data-ttu-id="1d4c2-p105">Die Startzelle. An diese Position wird das Diagramm verschoben. Die Startzelle ist die obere linke oder die obere rechte Zelle, abhängig davon, ob die eingestellte Textrichtung des Benutzers von links nach rechts oder von rechts nach links ist.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-p105">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="1d4c2-138">endCell</span><span class="sxs-lookup"><span data-stu-id="1d4c2-138">endCell</span></span>|<span data-ttu-id="1d4c2-139">string</span><span class="sxs-lookup"><span data-stu-id="1d4c2-139">string</span></span>|<span data-ttu-id="1d4c2-p106">Optional. Die Endzelle. Wenn angegeben, werden Breite und Höhe des Diagramms so eingestellt, dass diese Zelle/dieser Bereich vollständig bedeckt ist.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-p106">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="1d4c2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d4c2-143">Response</span></span>

<span data-ttu-id="1d4c2-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d4c2-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d4c2-146">Example</span></span>
<span data-ttu-id="1d4c2-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1d4c2-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d4c2-148">Request</span></span>
<span data-ttu-id="1d4c2-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="1d4c2-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d4c2-150">Response</span></span>
<span data-ttu-id="1d4c2-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d4c2-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

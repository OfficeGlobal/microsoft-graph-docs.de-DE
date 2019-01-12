---
title: 'Chart: setPosition'
description: Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d8e4c65954790fcebc885a84183b7941e2701e28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981812"
---
# <a name="chart-setposition"></a><span data-ttu-id="7aa40-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="7aa40-103">Chart: setPosition</span></span>

<span data-ttu-id="7aa40-104">Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="7aa40-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="7aa40-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7aa40-105">Permissions</span></span>
<span data-ttu-id="7aa40-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa40-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7aa40-108">Permission type</span></span>      | <span data-ttu-id="7aa40-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7aa40-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aa40-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7aa40-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7aa40-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aa40-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7aa40-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7aa40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aa40-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7aa40-113">Not supported.</span></span>    |
|<span data-ttu-id="7aa40-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7aa40-114">Application</span></span> | <span data-ttu-id="7aa40-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7aa40-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aa40-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7aa40-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="7aa40-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7aa40-117">Request headers</span></span>
| <span data-ttu-id="7aa40-118">Name</span><span class="sxs-lookup"><span data-stu-id="7aa40-118">Name</span></span>       | <span data-ttu-id="7aa40-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7aa40-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7aa40-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa40-120">Authorization</span></span>  | <span data-ttu-id="7aa40-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7aa40-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7aa40-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7aa40-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7aa40-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7aa40-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aa40-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7aa40-126">Request body</span></span>
<span data-ttu-id="7aa40-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7aa40-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7aa40-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="7aa40-128">Parameter</span></span>    | <span data-ttu-id="7aa40-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7aa40-129">Type</span></span>   |<span data-ttu-id="7aa40-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7aa40-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7aa40-131">startCell</span><span class="sxs-lookup"><span data-stu-id="7aa40-131">startCell</span></span>|<span data-ttu-id="7aa40-132">Json</span><span class="sxs-lookup"><span data-stu-id="7aa40-132">Json</span></span>|<span data-ttu-id="7aa40-p104">Die Startzelle. An diese Position wird das Diagramm verschoben. Die Startzelle ist die obere linke oder die obere rechte Zelle, abhängig davon, ob die eingestellte Textrichtung des Benutzers von links nach rechts oder von rechts nach links ist.</span><span class="sxs-lookup"><span data-stu-id="7aa40-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="7aa40-136">endCell</span><span class="sxs-lookup"><span data-stu-id="7aa40-136">endCell</span></span>|<span data-ttu-id="7aa40-137">Json</span><span class="sxs-lookup"><span data-stu-id="7aa40-137">Json</span></span>|<span data-ttu-id="7aa40-p105">Optional. Die Endzelle. Wenn angegeben, werden Breite und Höhe des Diagramms so eingestellt, dass diese Zelle/dieser Bereich vollständig bedeckt ist.</span><span class="sxs-lookup"><span data-stu-id="7aa40-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="7aa40-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7aa40-141">Response</span></span>

<span data-ttu-id="7aa40-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7aa40-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aa40-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7aa40-144">Example</span></span>
<span data-ttu-id="7aa40-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7aa40-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7aa40-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7aa40-146">Request</span></span>
<span data-ttu-id="7aa40-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7aa40-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="7aa40-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="7aa40-148">Response</span></span>
<span data-ttu-id="7aa40-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7aa40-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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

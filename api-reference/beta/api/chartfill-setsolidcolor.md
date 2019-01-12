---
title: 'ChartFill: setSolidColor'
description: Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e5c0a120becc53b6b7d06fdc1e5c43130b5a414b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975918"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="dca43-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="dca43-103">ChartFill: setSolidColor</span></span>

> <span data-ttu-id="dca43-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dca43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dca43-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dca43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dca43-106">Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.</span><span class="sxs-lookup"><span data-stu-id="dca43-106">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="dca43-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dca43-107">Permissions</span></span>
<span data-ttu-id="dca43-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dca43-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dca43-110">Permission type</span></span>      | <span data-ttu-id="dca43-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dca43-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dca43-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dca43-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dca43-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca43-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dca43-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dca43-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dca43-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca43-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dca43-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dca43-116">Application</span></span> | <span data-ttu-id="dca43-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dca43-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dca43-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dca43-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="dca43-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dca43-119">Request headers</span></span>
| <span data-ttu-id="dca43-120">Name</span><span class="sxs-lookup"><span data-stu-id="dca43-120">Name</span></span>       | <span data-ttu-id="dca43-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dca43-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dca43-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dca43-122">Authorization</span></span>  | <span data-ttu-id="dca43-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dca43-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dca43-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="dca43-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dca43-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="dca43-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dca43-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dca43-128">Request body</span></span>
<span data-ttu-id="dca43-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="dca43-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dca43-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="dca43-130">Parameter</span></span>    | <span data-ttu-id="dca43-131">Typ</span><span class="sxs-lookup"><span data-stu-id="dca43-131">Type</span></span>   |<span data-ttu-id="dca43-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dca43-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dca43-133">color</span><span class="sxs-lookup"><span data-stu-id="dca43-133">color</span></span>|<span data-ttu-id="dca43-134">string</span><span class="sxs-lookup"><span data-stu-id="dca43-134">string</span></span>|<span data-ttu-id="dca43-135">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="dca43-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="dca43-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="dca43-136">Response</span></span>

<span data-ttu-id="dca43-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dca43-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dca43-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dca43-139">Example</span></span>
<span data-ttu-id="dca43-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="dca43-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dca43-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dca43-141">Request</span></span>
<span data-ttu-id="dca43-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dca43-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="dca43-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="dca43-143">Response</span></span>
<span data-ttu-id="dca43-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dca43-144">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'ChartFill: setSolidColor'
description: Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: af768275d5954e1a6df561e3147265a3382b794a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950851"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="ecb0e-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="ecb0e-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="ecb0e-104">Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="ecb0e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ecb0e-105">Permissions</span></span>
<span data-ttu-id="ecb0e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb0e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ecb0e-108">Permission type</span></span>      | <span data-ttu-id="ecb0e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ecb0e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecb0e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ecb0e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ecb0e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecb0e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ecb0e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ecb0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecb0e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ecb0e-113">Not supported.</span></span>    |
|<span data-ttu-id="ecb0e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ecb0e-114">Application</span></span> | <span data-ttu-id="ecb0e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ecb0e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecb0e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecb0e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="ecb0e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ecb0e-117">Request headers</span></span>
| <span data-ttu-id="ecb0e-118">Name</span><span class="sxs-lookup"><span data-stu-id="ecb0e-118">Name</span></span>       | <span data-ttu-id="ecb0e-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecb0e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ecb0e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecb0e-120">Authorization</span></span>  | <span data-ttu-id="ecb0e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ecb0e-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="ecb0e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ecb0e-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecb0e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ecb0e-126">Request body</span></span>
<span data-ttu-id="ecb0e-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ecb0e-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="ecb0e-128">Parameter</span></span>    | <span data-ttu-id="ecb0e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ecb0e-129">Type</span></span>   |<span data-ttu-id="ecb0e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecb0e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb0e-131">color</span><span class="sxs-lookup"><span data-stu-id="ecb0e-131">color</span></span>|<span data-ttu-id="ecb0e-132">string</span><span class="sxs-lookup"><span data-stu-id="ecb0e-132">string</span></span>|<span data-ttu-id="ecb0e-133">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="ecb0e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecb0e-134">Response</span></span>

<span data-ttu-id="ecb0e-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecb0e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ecb0e-137">Example</span></span>
<span data-ttu-id="ecb0e-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ecb0e-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ecb0e-139">Request</span></span>
<span data-ttu-id="ecb0e-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="ecb0e-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="ecb0e-141">Response</span></span>
<span data-ttu-id="ecb0e-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ecb0e-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
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

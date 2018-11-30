---
title: 'ChartFill: setSolidColor'
description: Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.
ms.openlocfilehash: bcb8397217ee6cc574fe08f585d51a6243d83ca9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016599"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="11c9d-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="11c9d-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="11c9d-104">Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.</span><span class="sxs-lookup"><span data-stu-id="11c9d-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="11c9d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="11c9d-105">Permissions</span></span>
<span data-ttu-id="11c9d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11c9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11c9d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11c9d-108">Permission type</span></span>      | <span data-ttu-id="11c9d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11c9d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11c9d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11c9d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11c9d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11c9d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11c9d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11c9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c9d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11c9d-113">Not supported.</span></span>    |
|<span data-ttu-id="11c9d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11c9d-114">Application</span></span> | <span data-ttu-id="11c9d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11c9d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11c9d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11c9d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="11c9d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11c9d-117">Request headers</span></span>
| <span data-ttu-id="11c9d-118">Name</span><span class="sxs-lookup"><span data-stu-id="11c9d-118">Name</span></span>       | <span data-ttu-id="11c9d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11c9d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11c9d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="11c9d-120">Authorization</span></span>  | <span data-ttu-id="11c9d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11c9d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11c9d-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="11c9d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="11c9d-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="11c9d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11c9d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11c9d-126">Request body</span></span>
<span data-ttu-id="11c9d-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="11c9d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11c9d-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="11c9d-128">Parameter</span></span>    | <span data-ttu-id="11c9d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="11c9d-129">Type</span></span>   |<span data-ttu-id="11c9d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11c9d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11c9d-131">color</span><span class="sxs-lookup"><span data-stu-id="11c9d-131">color</span></span>|<span data-ttu-id="11c9d-132">string</span><span class="sxs-lookup"><span data-stu-id="11c9d-132">string</span></span>|<span data-ttu-id="11c9d-133">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="11c9d-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="11c9d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="11c9d-134">Response</span></span>

<span data-ttu-id="11c9d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11c9d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11c9d-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11c9d-137">Example</span></span>
<span data-ttu-id="11c9d-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="11c9d-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="11c9d-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11c9d-139">Request</span></span>
<span data-ttu-id="11c9d-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11c9d-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="11c9d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="11c9d-141">Response</span></span>
<span data-ttu-id="11c9d-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11c9d-142">Here is an example of the response.</span></span> 
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
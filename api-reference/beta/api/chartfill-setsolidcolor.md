---
title: 'ChartFill: setSolidColor'
description: Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: ffd5d4f954fea72963c7d443a5df6de12f1dc516
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854642"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="70b72-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="70b72-103">ChartFill: setSolidColor</span></span>

> <span data-ttu-id="70b72-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="70b72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70b72-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70b72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70b72-106">Legt die Füllung eines Diagrammelements auf einfarbige Füllung fest.</span><span class="sxs-lookup"><span data-stu-id="70b72-106">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="70b72-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="70b72-107">Permissions</span></span>
<span data-ttu-id="70b72-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70b72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70b72-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70b72-110">Permission type</span></span>      | <span data-ttu-id="70b72-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70b72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70b72-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70b72-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70b72-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70b72-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70b72-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70b72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70b72-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70b72-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70b72-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70b72-116">Application</span></span> | <span data-ttu-id="70b72-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70b72-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70b72-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70b72-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="70b72-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70b72-119">Request headers</span></span>
| <span data-ttu-id="70b72-120">Name</span><span class="sxs-lookup"><span data-stu-id="70b72-120">Name</span></span>       | <span data-ttu-id="70b72-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70b72-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="70b72-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70b72-122">Authorization</span></span>  | <span data-ttu-id="70b72-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="70b72-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70b72-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="70b72-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="70b72-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="70b72-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70b72-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70b72-128">Request body</span></span>
<span data-ttu-id="70b72-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="70b72-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="70b72-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="70b72-130">Parameter</span></span>    | <span data-ttu-id="70b72-131">Typ</span><span class="sxs-lookup"><span data-stu-id="70b72-131">Type</span></span>   |<span data-ttu-id="70b72-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70b72-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70b72-133">color</span><span class="sxs-lookup"><span data-stu-id="70b72-133">color</span></span>|<span data-ttu-id="70b72-134">string</span><span class="sxs-lookup"><span data-stu-id="70b72-134">string</span></span>|<span data-ttu-id="70b72-135">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="70b72-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="70b72-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="70b72-136">Response</span></span>

<span data-ttu-id="70b72-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70b72-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70b72-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70b72-139">Example</span></span>
<span data-ttu-id="70b72-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="70b72-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="70b72-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70b72-141">Request</span></span>
<span data-ttu-id="70b72-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70b72-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="70b72-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="70b72-143">Response</span></span>
<span data-ttu-id="70b72-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70b72-144">Here is an example of the response.</span></span> 
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

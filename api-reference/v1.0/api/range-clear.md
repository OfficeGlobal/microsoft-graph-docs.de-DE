---
title: 'Range: clear'
description: Löschen von Bereichswerten, Format, Füllung, Rahmen usw.
ms.openlocfilehash: c4a320827031eed62727ef464551cd410d71b610
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019073"
---
# <a name="range-clear"></a><span data-ttu-id="c8b0c-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="c8b0c-103">Range: clear</span></span>

<span data-ttu-id="c8b0c-104">Löschen von Bereichswerten, Format, Füllung, Rahmen usw.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8b0c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8b0c-105">Permissions</span></span>
<span data-ttu-id="c8b0c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8b0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8b0c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8b0c-108">Permission type</span></span>      | <span data-ttu-id="c8b0c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8b0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8b0c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8b0c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8b0c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8b0c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8b0c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8b0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8b0c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8b0c-113">Not supported.</span></span>    |
|<span data-ttu-id="c8b0c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8b0c-114">Application</span></span> | <span data-ttu-id="c8b0c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8b0c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8b0c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8b0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="c8b0c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8b0c-117">Request headers</span></span>
| <span data-ttu-id="c8b0c-118">Name</span><span class="sxs-lookup"><span data-stu-id="c8b0c-118">Name</span></span>       | <span data-ttu-id="c8b0c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8b0c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8b0c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8b0c-120">Authorization</span></span>  | <span data-ttu-id="c8b0c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8b0c-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c8b0c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8b0c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8b0c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8b0c-126">Request body</span></span>
<span data-ttu-id="c8b0c-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8b0c-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="c8b0c-128">Parameter</span></span>    | <span data-ttu-id="c8b0c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c8b0c-129">Type</span></span>   |<span data-ttu-id="c8b0c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8b0c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8b0c-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="c8b0c-131">applyTo</span></span>|<span data-ttu-id="c8b0c-132">string</span><span class="sxs-lookup"><span data-stu-id="c8b0c-132">string</span></span>|<span data-ttu-id="c8b0c-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-133">Optional.</span></span> <span data-ttu-id="c8b0c-134">Bestimmt den Typ der Aktion löschen.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-134">Determines the type of clear action.</span></span>  <span data-ttu-id="c8b0c-135">Die möglichen Werte sind: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-135">The possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="c8b0c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8b0c-136">Response</span></span>

<span data-ttu-id="c8b0c-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8b0c-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8b0c-139">Example</span></span>
<span data-ttu-id="c8b0c-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8b0c-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8b0c-141">Request</span></span>
<span data-ttu-id="c8b0c-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="c8b0c-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8b0c-143">Response</span></span>
<span data-ttu-id="c8b0c-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8b0c-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
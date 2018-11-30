---
title: 'Range: clear'
description: Löschen von Bereichswerten, Format, Füllung, Rahmen usw.
ms.openlocfilehash: 2a75530d0a8c366718e7e67f64811e4da9fa27e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059425"
---
# <a name="range-clear"></a><span data-ttu-id="90936-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="90936-103">Range: clear</span></span>

> <span data-ttu-id="90936-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="90936-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90936-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90936-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90936-106">Löschen von Bereichswerten, Format, Füllung, Rahmen usw.</span><span class="sxs-lookup"><span data-stu-id="90936-106">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="90936-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="90936-107">Permissions</span></span>
<span data-ttu-id="90936-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90936-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90936-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90936-110">Permission type</span></span>      | <span data-ttu-id="90936-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90936-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90936-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90936-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90936-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90936-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90936-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90936-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90936-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90936-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="90936-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90936-116">Application</span></span> | <span data-ttu-id="90936-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90936-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90936-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90936-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="90936-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="90936-119">Request headers</span></span>
| <span data-ttu-id="90936-120">Name</span><span class="sxs-lookup"><span data-stu-id="90936-120">Name</span></span>       | <span data-ttu-id="90936-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90936-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90936-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90936-122">Authorization</span></span>  | <span data-ttu-id="90936-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="90936-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90936-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="90936-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="90936-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="90936-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90936-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90936-128">Request body</span></span>
<span data-ttu-id="90936-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="90936-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90936-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="90936-130">Parameter</span></span>    | <span data-ttu-id="90936-131">Typ</span><span class="sxs-lookup"><span data-stu-id="90936-131">Type</span></span>   |<span data-ttu-id="90936-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90936-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90936-133">applyTo</span><span class="sxs-lookup"><span data-stu-id="90936-133">applyTo</span></span>|<span data-ttu-id="90936-134">string</span><span class="sxs-lookup"><span data-stu-id="90936-134">string</span></span>|<span data-ttu-id="90936-p105">Optional. Bestimmt den Typ der Löschaktion.  Mögliche Werte: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="90936-p105">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="90936-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="90936-138">Response</span></span>

<span data-ttu-id="90936-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90936-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90936-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90936-141">Example</span></span>
<span data-ttu-id="90936-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="90936-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="90936-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90936-143">Request</span></span>
<span data-ttu-id="90936-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90936-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="90936-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="90936-145">Response</span></span>
<span data-ttu-id="90936-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="90936-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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
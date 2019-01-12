---
title: 'Range: clear'
description: Löschen von Bereichswerten, Format, Füllung, Rahmen usw.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a32c21763c18371d3f0efe649b795135d4752b87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991629"
---
# <a name="range-clear"></a><span data-ttu-id="041ab-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="041ab-103">Range: clear</span></span>

> <span data-ttu-id="041ab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="041ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="041ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="041ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="041ab-106">Löschen von Bereichswerten, Format, Füllung, Rahmen usw.</span><span class="sxs-lookup"><span data-stu-id="041ab-106">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="041ab-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="041ab-107">Permissions</span></span>
<span data-ttu-id="041ab-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="041ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="041ab-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="041ab-110">Permission type</span></span>      | <span data-ttu-id="041ab-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="041ab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="041ab-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="041ab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="041ab-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041ab-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="041ab-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="041ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="041ab-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="041ab-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="041ab-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="041ab-116">Application</span></span> | <span data-ttu-id="041ab-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="041ab-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="041ab-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="041ab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="041ab-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="041ab-119">Request headers</span></span>
| <span data-ttu-id="041ab-120">Name</span><span class="sxs-lookup"><span data-stu-id="041ab-120">Name</span></span>       | <span data-ttu-id="041ab-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="041ab-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="041ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="041ab-122">Authorization</span></span>  | <span data-ttu-id="041ab-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="041ab-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="041ab-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="041ab-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="041ab-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="041ab-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="041ab-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="041ab-128">Request body</span></span>
<span data-ttu-id="041ab-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="041ab-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="041ab-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="041ab-130">Parameter</span></span>    | <span data-ttu-id="041ab-131">Typ</span><span class="sxs-lookup"><span data-stu-id="041ab-131">Type</span></span>   |<span data-ttu-id="041ab-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="041ab-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="041ab-133">applyTo</span><span class="sxs-lookup"><span data-stu-id="041ab-133">applyTo</span></span>|<span data-ttu-id="041ab-134">string</span><span class="sxs-lookup"><span data-stu-id="041ab-134">string</span></span>|<span data-ttu-id="041ab-p105">Optional. Bestimmt den Typ der Löschaktion.  Mögliche Werte: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="041ab-p105">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="041ab-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="041ab-138">Response</span></span>

<span data-ttu-id="041ab-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="041ab-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="041ab-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="041ab-141">Example</span></span>
<span data-ttu-id="041ab-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="041ab-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="041ab-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="041ab-143">Request</span></span>
<span data-ttu-id="041ab-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="041ab-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="041ab-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="041ab-145">Response</span></span>
<span data-ttu-id="041ab-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="041ab-146">Here is an example of the response.</span></span> 
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

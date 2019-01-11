---
title: 'WorksheetProtection: Schützen'
description: Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: ba6909ce9a6a1bd025eb5364bf1a6ad100105134
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830233"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="3b441-104">WorksheetProtection: Schützen</span><span class="sxs-lookup"><span data-stu-id="3b441-104">WorksheetProtection: protect</span></span>

> <span data-ttu-id="3b441-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b441-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b441-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b441-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b441-p103">Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="3b441-p103">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b441-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b441-109">Permissions</span></span>
<span data-ttu-id="3b441-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b441-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b441-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b441-112">Permission type</span></span>      | <span data-ttu-id="3b441-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b441-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b441-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b441-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3b441-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b441-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b441-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b441-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b441-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b441-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b441-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b441-118">Application</span></span> | <span data-ttu-id="3b441-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b441-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b441-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b441-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="3b441-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b441-121">Request headers</span></span>
| <span data-ttu-id="3b441-122">Name</span><span class="sxs-lookup"><span data-stu-id="3b441-122">Name</span></span>       | <span data-ttu-id="3b441-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b441-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3b441-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b441-124">Authorization</span></span>  | <span data-ttu-id="3b441-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b441-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b441-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3b441-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="3b441-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3b441-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b441-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b441-130">Request body</span></span>
<span data-ttu-id="3b441-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="3b441-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3b441-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="3b441-132">Parameter</span></span>    | <span data-ttu-id="3b441-133">Typ</span><span class="sxs-lookup"><span data-stu-id="3b441-133">Type</span></span>   |<span data-ttu-id="3b441-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b441-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b441-135">options</span><span class="sxs-lookup"><span data-stu-id="3b441-135">options</span></span>|<span data-ttu-id="3b441-136">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="3b441-136">WorksheetProtectionOptions</span></span>|<span data-ttu-id="3b441-p107">Optional. Optionen für den Arbeitsblattschutz.</span><span class="sxs-lookup"><span data-stu-id="3b441-p107">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="3b441-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b441-139">Response</span></span>

<span data-ttu-id="3b441-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b441-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b441-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b441-142">Example</span></span>
<span data-ttu-id="3b441-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3b441-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3b441-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b441-144">Request</span></span>
<span data-ttu-id="3b441-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b441-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="3b441-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b441-146">Response</span></span>
<span data-ttu-id="3b441-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b441-147">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

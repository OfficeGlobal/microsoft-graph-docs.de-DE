---
title: 'WorksheetProtection: Schützen'
description: Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2cfc65a067207ea947e8d6b5b5d3cbe72a48466f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921108"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="79997-104">WorksheetProtection: Schützen</span><span class="sxs-lookup"><span data-stu-id="79997-104">WorksheetProtection: protect</span></span>

<span data-ttu-id="79997-p102">Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.</span><span class="sxs-lookup"><span data-stu-id="79997-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="79997-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79997-107">Permissions</span></span>
<span data-ttu-id="79997-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79997-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79997-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79997-110">Permission type</span></span>      | <span data-ttu-id="79997-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79997-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79997-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79997-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79997-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79997-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79997-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79997-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79997-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79997-115">Not supported.</span></span>    |
|<span data-ttu-id="79997-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79997-116">Application</span></span> | <span data-ttu-id="79997-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79997-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79997-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79997-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="79997-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79997-119">Request headers</span></span>
| <span data-ttu-id="79997-120">Name</span><span class="sxs-lookup"><span data-stu-id="79997-120">Name</span></span>       | <span data-ttu-id="79997-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79997-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79997-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79997-122">Authorization</span></span>  | <span data-ttu-id="79997-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79997-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79997-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="79997-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="79997-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="79997-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79997-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79997-128">Request body</span></span>
<span data-ttu-id="79997-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="79997-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79997-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="79997-130">Parameter</span></span>    | <span data-ttu-id="79997-131">Typ</span><span class="sxs-lookup"><span data-stu-id="79997-131">Type</span></span>   |<span data-ttu-id="79997-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79997-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79997-133">options</span><span class="sxs-lookup"><span data-stu-id="79997-133">options</span></span>|<span data-ttu-id="79997-134">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="79997-134">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="79997-p106">Optional. Optionen für den Arbeitsblattschutz.</span><span class="sxs-lookup"><span data-stu-id="79997-p106">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="79997-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="79997-137">Response</span></span>

<span data-ttu-id="79997-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79997-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79997-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79997-140">Example</span></span>
<span data-ttu-id="79997-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="79997-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79997-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79997-142">Request</span></span>
<span data-ttu-id="79997-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79997-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
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

##### <a name="response"></a><span data-ttu-id="79997-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="79997-144">Response</span></span>
<span data-ttu-id="79997-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="79997-145">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

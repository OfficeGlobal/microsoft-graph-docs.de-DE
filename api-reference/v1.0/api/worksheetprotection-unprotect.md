---
title: 'WorksheetProtection: Schutz aufheben'
description: Schutz eines Arbeitsblatts aufheben.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 662f047966f0d0e94c3facea8c3badbd8c775cdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823394"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="b39ed-103">WorksheetProtection: Schutz aufheben</span><span class="sxs-lookup"><span data-stu-id="b39ed-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="b39ed-104">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="b39ed-104">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="b39ed-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b39ed-105">Permissions</span></span>
<span data-ttu-id="b39ed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b39ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b39ed-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b39ed-108">Permission type</span></span>      | <span data-ttu-id="b39ed-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b39ed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b39ed-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b39ed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b39ed-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b39ed-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b39ed-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b39ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b39ed-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b39ed-113">Not supported.</span></span>    |
|<span data-ttu-id="b39ed-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b39ed-114">Application</span></span> | <span data-ttu-id="b39ed-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b39ed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b39ed-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b39ed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="b39ed-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b39ed-117">Request headers</span></span>
| <span data-ttu-id="b39ed-118">Name</span><span class="sxs-lookup"><span data-stu-id="b39ed-118">Name</span></span>       | <span data-ttu-id="b39ed-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b39ed-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b39ed-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b39ed-120">Authorization</span></span>  | <span data-ttu-id="b39ed-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b39ed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b39ed-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b39ed-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b39ed-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b39ed-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b39ed-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b39ed-126">Request body</span></span>
<span data-ttu-id="b39ed-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b39ed-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b39ed-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="b39ed-128">Parameter</span></span>    | <span data-ttu-id="b39ed-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b39ed-129">Type</span></span>   |<span data-ttu-id="b39ed-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b39ed-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b39ed-131">password</span><span class="sxs-lookup"><span data-stu-id="b39ed-131">password</span></span>|<span data-ttu-id="b39ed-132">string</span><span class="sxs-lookup"><span data-stu-id="b39ed-132">string</span></span>|<span data-ttu-id="b39ed-p104">Optional. Kennwort für den Arbeitsblattschutz.</span><span class="sxs-lookup"><span data-stu-id="b39ed-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="b39ed-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b39ed-135">Response</span></span>

<span data-ttu-id="b39ed-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b39ed-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b39ed-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b39ed-138">Example</span></span>
<span data-ttu-id="b39ed-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b39ed-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b39ed-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b39ed-140">Request</span></span>
<span data-ttu-id="b39ed-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b39ed-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="b39ed-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="b39ed-142">Response</span></span>
<span data-ttu-id="b39ed-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b39ed-143">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

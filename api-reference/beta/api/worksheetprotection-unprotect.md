---
title: 'WorksheetProtection: Schutz aufheben'
description: Schutz eines Arbeitsblatts aufheben.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 52feaf77964949fee9bbedbf3ced2967226bb486
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850519"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="19ae6-103">WorksheetProtection: Schutz aufheben</span><span class="sxs-lookup"><span data-stu-id="19ae6-103">WorksheetProtection: unprotect</span></span>

> <span data-ttu-id="19ae6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="19ae6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19ae6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ae6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19ae6-106">Schutz eines Arbeitsblatts aufheben.</span><span class="sxs-lookup"><span data-stu-id="19ae6-106">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="19ae6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="19ae6-107">Permissions</span></span>
<span data-ttu-id="19ae6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19ae6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19ae6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19ae6-110">Permission type</span></span>      | <span data-ttu-id="19ae6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19ae6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19ae6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19ae6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19ae6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19ae6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19ae6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19ae6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19ae6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19ae6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19ae6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19ae6-116">Application</span></span> | <span data-ttu-id="19ae6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19ae6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19ae6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19ae6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="19ae6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19ae6-119">Request headers</span></span>
| <span data-ttu-id="19ae6-120">Name</span><span class="sxs-lookup"><span data-stu-id="19ae6-120">Name</span></span>       | <span data-ttu-id="19ae6-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19ae6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19ae6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19ae6-122">Authorization</span></span>  | <span data-ttu-id="19ae6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19ae6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19ae6-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="19ae6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="19ae6-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="19ae6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19ae6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19ae6-128">Request body</span></span>
<span data-ttu-id="19ae6-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="19ae6-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19ae6-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="19ae6-130">Parameter</span></span>    | <span data-ttu-id="19ae6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="19ae6-131">Type</span></span>   |<span data-ttu-id="19ae6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19ae6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19ae6-133">password</span><span class="sxs-lookup"><span data-stu-id="19ae6-133">password</span></span>|<span data-ttu-id="19ae6-134">string</span><span class="sxs-lookup"><span data-stu-id="19ae6-134">string</span></span>|<span data-ttu-id="19ae6-p105">Optional. Kennwort für den Arbeitsblattschutz.</span><span class="sxs-lookup"><span data-stu-id="19ae6-p105">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="19ae6-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="19ae6-137">Response</span></span>

<span data-ttu-id="19ae6-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19ae6-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ae6-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19ae6-140">Example</span></span>
<span data-ttu-id="19ae6-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="19ae6-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19ae6-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19ae6-142">Request</span></span>
<span data-ttu-id="19ae6-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19ae6-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="19ae6-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="19ae6-144">Response</span></span>
<span data-ttu-id="19ae6-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="19ae6-145">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'Range: merge'
description: Führt die Zellen des Bereichs in einen Bereich im Arbeitsblatt zusammen.
ms.openlocfilehash: be9ef68a6f3f62e3f9396a4b51a34b9f7e63199b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016119"
---
# <a name="range-merge"></a><span data-ttu-id="b6af2-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="b6af2-103">Range: merge</span></span>

<span data-ttu-id="b6af2-104">Führt die Zellen des Bereichs in einen Bereich im Arbeitsblatt zusammen.</span><span class="sxs-lookup"><span data-stu-id="b6af2-104">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6af2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b6af2-105">Permissions</span></span>
<span data-ttu-id="b6af2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6af2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6af2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6af2-108">Permission type</span></span>      | <span data-ttu-id="b6af2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6af2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6af2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6af2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6af2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6af2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b6af2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6af2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6af2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6af2-113">Not supported.</span></span>    |
|<span data-ttu-id="b6af2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6af2-114">Application</span></span> | <span data-ttu-id="b6af2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6af2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6af2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6af2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="b6af2-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6af2-117">Request headers</span></span>
| <span data-ttu-id="b6af2-118">Name</span><span class="sxs-lookup"><span data-stu-id="b6af2-118">Name</span></span>       | <span data-ttu-id="b6af2-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6af2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6af2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6af2-120">Authorization</span></span>  | <span data-ttu-id="b6af2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b6af2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6af2-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b6af2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b6af2-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b6af2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6af2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6af2-126">Request body</span></span>
<span data-ttu-id="b6af2-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b6af2-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b6af2-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="b6af2-128">Parameter</span></span>    | <span data-ttu-id="b6af2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b6af2-129">Type</span></span>   |<span data-ttu-id="b6af2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6af2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6af2-131">across</span><span class="sxs-lookup"><span data-stu-id="b6af2-131">across</span></span>|<span data-ttu-id="b6af2-132">boolean</span><span class="sxs-lookup"><span data-stu-id="b6af2-132">boolean</span></span>|<span data-ttu-id="b6af2-p104">Optional. Mit „true“ werden Zellen in allen Zeilen des angegebenen Bereichs als einzelne zusammengeführte Zellen zusammengeführt. Der Standardwert lautet „false“.</span><span class="sxs-lookup"><span data-stu-id="b6af2-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="b6af2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6af2-136">Response</span></span>

<span data-ttu-id="b6af2-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6af2-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6af2-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6af2-139">Example</span></span>
<span data-ttu-id="b6af2-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b6af2-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b6af2-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6af2-141">Request</span></span>
<span data-ttu-id="b6af2-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6af2-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="b6af2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6af2-143">Response</span></span>
<span data-ttu-id="b6af2-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b6af2-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: 'TableSort: apply'
description: Führt einen Sortiervorgang aus.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2dc8d9c0619e434d3799ae03e0ef54354c868852
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844100"
---
# <a name="tablesort-apply"></a><span data-ttu-id="861ca-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="861ca-103">TableSort: apply</span></span>

> <span data-ttu-id="861ca-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="861ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="861ca-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="861ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="861ca-106">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="861ca-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="861ca-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="861ca-107">Permissions</span></span>
<span data-ttu-id="861ca-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861ca-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="861ca-110">Permission type</span></span>      | <span data-ttu-id="861ca-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="861ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="861ca-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="861ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="861ca-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="861ca-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="861ca-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="861ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="861ca-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="861ca-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="861ca-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="861ca-116">Application</span></span> | <span data-ttu-id="861ca-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="861ca-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="861ca-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="861ca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="861ca-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="861ca-119">Request headers</span></span>
| <span data-ttu-id="861ca-120">Name</span><span class="sxs-lookup"><span data-stu-id="861ca-120">Name</span></span>       | <span data-ttu-id="861ca-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="861ca-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="861ca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="861ca-122">Authorization</span></span>  | <span data-ttu-id="861ca-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="861ca-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="861ca-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="861ca-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="861ca-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="861ca-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="861ca-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="861ca-128">Request body</span></span>
<span data-ttu-id="861ca-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="861ca-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="861ca-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="861ca-130">Parameter</span></span>    | <span data-ttu-id="861ca-131">Typ</span><span class="sxs-lookup"><span data-stu-id="861ca-131">Type</span></span>   |<span data-ttu-id="861ca-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="861ca-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="861ca-133">fields</span><span class="sxs-lookup"><span data-stu-id="861ca-133">fields</span></span>|<span data-ttu-id="861ca-134">SortField</span><span class="sxs-lookup"><span data-stu-id="861ca-134">SortField</span></span>|<span data-ttu-id="861ca-135">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="861ca-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="861ca-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="861ca-136">matchCase</span></span>|<span data-ttu-id="861ca-137">boolean</span><span class="sxs-lookup"><span data-stu-id="861ca-137">boolean</span></span>|<span data-ttu-id="861ca-p105">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="861ca-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="861ca-140">method</span><span class="sxs-lookup"><span data-stu-id="861ca-140">method</span></span>|<span data-ttu-id="861ca-141">string</span><span class="sxs-lookup"><span data-stu-id="861ca-141">string</span></span>|<span data-ttu-id="861ca-p106">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="861ca-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="861ca-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="861ca-145">Response</span></span>

<span data-ttu-id="861ca-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="861ca-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="861ca-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="861ca-148">Example</span></span>
<span data-ttu-id="861ca-149">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="861ca-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="861ca-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="861ca-150">Request</span></span>
<span data-ttu-id="861ca-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="861ca-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="861ca-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="861ca-152">Response</span></span>
<span data-ttu-id="861ca-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="861ca-153">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

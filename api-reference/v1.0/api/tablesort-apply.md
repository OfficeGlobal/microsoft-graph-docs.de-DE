---
title: 'TableSort: apply'
description: Führt einen Sortiervorgang aus.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 682cacd558d42cc32b092bd7421aa14967f9c5b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877042"
---
# <a name="tablesort-apply"></a><span data-ttu-id="a769c-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="a769c-103">TableSort: apply</span></span>

<span data-ttu-id="a769c-104">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="a769c-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="a769c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a769c-105">Permissions</span></span>
<span data-ttu-id="a769c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a769c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a769c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a769c-108">Permission type</span></span>      | <span data-ttu-id="a769c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a769c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a769c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a769c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a769c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a769c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a769c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a769c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a769c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a769c-113">Not supported.</span></span>    |
|<span data-ttu-id="a769c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a769c-114">Application</span></span> | <span data-ttu-id="a769c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a769c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a769c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a769c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="a769c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a769c-117">Request headers</span></span>
| <span data-ttu-id="a769c-118">Name</span><span class="sxs-lookup"><span data-stu-id="a769c-118">Name</span></span>       | <span data-ttu-id="a769c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a769c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a769c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a769c-120">Authorization</span></span>  | <span data-ttu-id="a769c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a769c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a769c-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a769c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a769c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a769c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a769c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a769c-126">Request body</span></span>
<span data-ttu-id="a769c-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a769c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a769c-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="a769c-128">Parameter</span></span>    | <span data-ttu-id="a769c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a769c-129">Type</span></span>   |<span data-ttu-id="a769c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a769c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a769c-131">fields</span><span class="sxs-lookup"><span data-stu-id="a769c-131">fields</span></span>|<span data-ttu-id="a769c-132">WorkbookSortField-Auflistung</span><span class="sxs-lookup"><span data-stu-id="a769c-132">WorkbookSortField collection</span></span>|<span data-ttu-id="a769c-133">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a769c-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="a769c-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="a769c-134">matchCase</span></span>|<span data-ttu-id="a769c-135">boolean</span><span class="sxs-lookup"><span data-stu-id="a769c-135">boolean</span></span>|<span data-ttu-id="a769c-p104">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="a769c-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="a769c-138">method</span><span class="sxs-lookup"><span data-stu-id="a769c-138">method</span></span>|<span data-ttu-id="a769c-139">string</span><span class="sxs-lookup"><span data-stu-id="a769c-139">string</span></span>|<span data-ttu-id="a769c-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="a769c-140">Optional.</span></span> <span data-ttu-id="a769c-141">Die Sortiermethode für chinesischen Schriftzeichen verwendet.</span><span class="sxs-lookup"><span data-stu-id="a769c-141">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="a769c-142">Die möglichen Werte sind: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="a769c-142">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="a769c-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="a769c-143">Response</span></span>

<span data-ttu-id="a769c-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a769c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a769c-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a769c-146">Example</span></span>
<span data-ttu-id="a769c-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a769c-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a769c-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a769c-148">Request</span></span>
<span data-ttu-id="a769c-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a769c-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
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

##### <a name="response"></a><span data-ttu-id="a769c-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="a769c-150">Response</span></span>
<span data-ttu-id="a769c-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a769c-151">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'RangeSort: apply'
description: Führt einen Sortiervorgang aus.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6298bc4368126debc384b4eafcbb05154c35aab6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825627"
---
# <a name="rangesort-apply"></a><span data-ttu-id="fc7af-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="fc7af-103">RangeSort: apply</span></span>

<span data-ttu-id="fc7af-104">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="fc7af-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc7af-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fc7af-105">Permissions</span></span>
<span data-ttu-id="fc7af-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc7af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc7af-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc7af-108">Permission type</span></span>      | <span data-ttu-id="fc7af-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc7af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc7af-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc7af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc7af-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc7af-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc7af-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc7af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc7af-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc7af-113">Not supported.</span></span>    |
|<span data-ttu-id="fc7af-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc7af-114">Application</span></span> | <span data-ttu-id="fc7af-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc7af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc7af-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc7af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="fc7af-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc7af-117">Request headers</span></span>
| <span data-ttu-id="fc7af-118">Name</span><span class="sxs-lookup"><span data-stu-id="fc7af-118">Name</span></span>       | <span data-ttu-id="fc7af-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc7af-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc7af-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc7af-120">Authorization</span></span>  | <span data-ttu-id="fc7af-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc7af-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc7af-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="fc7af-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc7af-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="fc7af-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc7af-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc7af-126">Request body</span></span>
<span data-ttu-id="fc7af-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="fc7af-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc7af-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="fc7af-128">Parameter</span></span>    | <span data-ttu-id="fc7af-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fc7af-129">Type</span></span>   |<span data-ttu-id="fc7af-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc7af-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc7af-131">fields</span><span class="sxs-lookup"><span data-stu-id="fc7af-131">fields</span></span>|<span data-ttu-id="fc7af-132">WorkbookSortField-Auflistung</span><span class="sxs-lookup"><span data-stu-id="fc7af-132">WorkbookSortField collection</span></span>|<span data-ttu-id="fc7af-133">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="fc7af-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="fc7af-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="fc7af-134">matchCase</span></span>|<span data-ttu-id="fc7af-135">boolean</span><span class="sxs-lookup"><span data-stu-id="fc7af-135">boolean</span></span>|<span data-ttu-id="fc7af-p104">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="fc7af-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="fc7af-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="fc7af-138">hasHeaders</span></span>|<span data-ttu-id="fc7af-139">boolean</span><span class="sxs-lookup"><span data-stu-id="fc7af-139">boolean</span></span>|<span data-ttu-id="fc7af-p105">Optional. Gibt an, ob der Bereich eine Kopfzeile aufweist.</span><span class="sxs-lookup"><span data-stu-id="fc7af-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="fc7af-142">orientation</span><span class="sxs-lookup"><span data-stu-id="fc7af-142">orientation</span></span>|<span data-ttu-id="fc7af-143">string</span><span class="sxs-lookup"><span data-stu-id="fc7af-143">string</span></span>|<span data-ttu-id="fc7af-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="fc7af-144">Optional.</span></span> <span data-ttu-id="fc7af-145">Gibt an, ob der Vorgang Zeilen oder Spalten sortiert wird.</span><span class="sxs-lookup"><span data-stu-id="fc7af-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="fc7af-146">Die möglichen Werte sind: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="fc7af-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="fc7af-147">Methode</span><span class="sxs-lookup"><span data-stu-id="fc7af-147">method</span></span>|<span data-ttu-id="fc7af-148">string</span><span class="sxs-lookup"><span data-stu-id="fc7af-148">string</span></span>|<span data-ttu-id="fc7af-149">Optional.</span><span class="sxs-lookup"><span data-stu-id="fc7af-149">Optional.</span></span> <span data-ttu-id="fc7af-150">Die Sortiermethode für chinesischen Schriftzeichen verwendet.</span><span class="sxs-lookup"><span data-stu-id="fc7af-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="fc7af-151">Die möglichen Werte sind: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="fc7af-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="fc7af-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc7af-152">Response</span></span>

<span data-ttu-id="fc7af-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc7af-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc7af-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc7af-155">Example</span></span>
<span data-ttu-id="fc7af-156">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="fc7af-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc7af-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc7af-157">Request</span></span>
<span data-ttu-id="fc7af-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc7af-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="fc7af-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc7af-159">Response</span></span>
<span data-ttu-id="fc7af-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fc7af-160">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

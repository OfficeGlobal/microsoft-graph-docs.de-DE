---
title: 'RangeSort: apply'
description: Führt einen Sortiervorgang aus.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be024f3eacbb4e2d1178ec7b82a8e8ca604aff60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967105"
---
# <a name="rangesort-apply"></a><span data-ttu-id="c7681-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="c7681-103">RangeSort: apply</span></span>

<span data-ttu-id="c7681-104">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="c7681-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7681-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c7681-105">Permissions</span></span>
<span data-ttu-id="c7681-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7681-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7681-108">Permission type</span></span>      | <span data-ttu-id="c7681-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7681-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7681-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7681-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7681-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7681-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7681-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7681-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7681-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7681-113">Not supported.</span></span>    |
|<span data-ttu-id="c7681-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7681-114">Application</span></span> | <span data-ttu-id="c7681-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7681-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7681-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7681-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="c7681-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7681-117">Request headers</span></span>
| <span data-ttu-id="c7681-118">Name</span><span class="sxs-lookup"><span data-stu-id="c7681-118">Name</span></span>       | <span data-ttu-id="c7681-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7681-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c7681-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7681-120">Authorization</span></span>  | <span data-ttu-id="c7681-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c7681-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7681-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c7681-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c7681-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c7681-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7681-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7681-126">Request body</span></span>
<span data-ttu-id="c7681-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c7681-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c7681-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="c7681-128">Parameter</span></span>    | <span data-ttu-id="c7681-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c7681-129">Type</span></span>   |<span data-ttu-id="c7681-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7681-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7681-131">fields</span><span class="sxs-lookup"><span data-stu-id="c7681-131">fields</span></span>|<span data-ttu-id="c7681-132">WorkbookSortField-Auflistung</span><span class="sxs-lookup"><span data-stu-id="c7681-132">WorkbookSortField collection</span></span>|<span data-ttu-id="c7681-133">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c7681-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="c7681-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="c7681-134">matchCase</span></span>|<span data-ttu-id="c7681-135">boolean</span><span class="sxs-lookup"><span data-stu-id="c7681-135">boolean</span></span>|<span data-ttu-id="c7681-p104">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="c7681-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="c7681-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="c7681-138">hasHeaders</span></span>|<span data-ttu-id="c7681-139">boolean</span><span class="sxs-lookup"><span data-stu-id="c7681-139">boolean</span></span>|<span data-ttu-id="c7681-p105">Optional. Gibt an, ob der Bereich eine Kopfzeile aufweist.</span><span class="sxs-lookup"><span data-stu-id="c7681-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="c7681-142">orientation</span><span class="sxs-lookup"><span data-stu-id="c7681-142">orientation</span></span>|<span data-ttu-id="c7681-143">string</span><span class="sxs-lookup"><span data-stu-id="c7681-143">string</span></span>|<span data-ttu-id="c7681-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="c7681-144">Optional.</span></span> <span data-ttu-id="c7681-145">Gibt an, ob der Vorgang Zeilen oder Spalten sortiert wird.</span><span class="sxs-lookup"><span data-stu-id="c7681-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="c7681-146">Die möglichen Werte sind: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="c7681-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="c7681-147">Methode</span><span class="sxs-lookup"><span data-stu-id="c7681-147">method</span></span>|<span data-ttu-id="c7681-148">string</span><span class="sxs-lookup"><span data-stu-id="c7681-148">string</span></span>|<span data-ttu-id="c7681-149">Optional.</span><span class="sxs-lookup"><span data-stu-id="c7681-149">Optional.</span></span> <span data-ttu-id="c7681-150">Die Sortiermethode für chinesischen Schriftzeichen verwendet.</span><span class="sxs-lookup"><span data-stu-id="c7681-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="c7681-151">Die möglichen Werte sind: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="c7681-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="c7681-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7681-152">Response</span></span>

<span data-ttu-id="c7681-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7681-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7681-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7681-155">Example</span></span>
<span data-ttu-id="c7681-156">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c7681-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7681-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7681-157">Request</span></span>
<span data-ttu-id="c7681-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7681-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c7681-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7681-159">Response</span></span>
<span data-ttu-id="c7681-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c7681-160">Here is an example of the response.</span></span> 
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

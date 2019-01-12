---
title: 'RangeSort: apply'
description: Führt einen Sortiervorgang aus.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 66006bafdc26ecca85dda3dc0eb0999a387dddc5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968365"
---
# <a name="rangesort-apply"></a><span data-ttu-id="0439a-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="0439a-103">RangeSort: apply</span></span>

> <span data-ttu-id="0439a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0439a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0439a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0439a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0439a-106">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="0439a-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="0439a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0439a-107">Permissions</span></span>
<span data-ttu-id="0439a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0439a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0439a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0439a-110">Permission type</span></span>      | <span data-ttu-id="0439a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0439a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0439a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0439a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0439a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0439a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0439a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0439a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0439a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0439a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0439a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0439a-116">Application</span></span> | <span data-ttu-id="0439a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0439a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0439a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0439a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="0439a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0439a-119">Request headers</span></span>
| <span data-ttu-id="0439a-120">Name</span><span class="sxs-lookup"><span data-stu-id="0439a-120">Name</span></span>       | <span data-ttu-id="0439a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0439a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0439a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0439a-122">Authorization</span></span>  | <span data-ttu-id="0439a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0439a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0439a-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="0439a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0439a-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="0439a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0439a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0439a-128">Request body</span></span>
<span data-ttu-id="0439a-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0439a-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0439a-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="0439a-130">Parameter</span></span>    | <span data-ttu-id="0439a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0439a-131">Type</span></span>   |<span data-ttu-id="0439a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0439a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0439a-133">fields</span><span class="sxs-lookup"><span data-stu-id="0439a-133">fields</span></span>|<span data-ttu-id="0439a-134">SortField</span><span class="sxs-lookup"><span data-stu-id="0439a-134">SortField</span></span>|<span data-ttu-id="0439a-135">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0439a-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="0439a-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="0439a-136">matchCase</span></span>|<span data-ttu-id="0439a-137">boolean</span><span class="sxs-lookup"><span data-stu-id="0439a-137">boolean</span></span>|<span data-ttu-id="0439a-p105">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="0439a-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="0439a-140">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="0439a-140">hasHeaders</span></span>|<span data-ttu-id="0439a-141">boolean</span><span class="sxs-lookup"><span data-stu-id="0439a-141">boolean</span></span>|<span data-ttu-id="0439a-p106">Optional. Gibt an, ob der Bereich eine Kopfzeile aufweist.</span><span class="sxs-lookup"><span data-stu-id="0439a-p106">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="0439a-144">orientation</span><span class="sxs-lookup"><span data-stu-id="0439a-144">orientation</span></span>|<span data-ttu-id="0439a-145">string</span><span class="sxs-lookup"><span data-stu-id="0439a-145">string</span></span>|<span data-ttu-id="0439a-p107">Optional. Gibt an, ob der Vorgang Zeilen oder Spalten sortiert.  Die folgenden Werte sind möglich: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="0439a-p107">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="0439a-149">Methode</span><span class="sxs-lookup"><span data-stu-id="0439a-149">method</span></span>|<span data-ttu-id="0439a-150">string</span><span class="sxs-lookup"><span data-stu-id="0439a-150">string</span></span>|<span data-ttu-id="0439a-p108">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="0439a-p108">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="0439a-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="0439a-154">Response</span></span>

<span data-ttu-id="0439a-p109">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0439a-p109">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0439a-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0439a-157">Example</span></span>
<span data-ttu-id="0439a-158">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0439a-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0439a-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0439a-159">Request</span></span>
<span data-ttu-id="0439a-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0439a-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="0439a-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="0439a-161">Response</span></span>
<span data-ttu-id="0439a-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0439a-162">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

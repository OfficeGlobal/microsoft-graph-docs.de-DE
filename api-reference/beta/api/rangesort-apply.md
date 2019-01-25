---
title: 'RangeSort: apply'
description: Führt einen Sortiervorgang aus.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7979033ce520f0d29172a910f4935c428bee383f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523582"
---
# <a name="rangesort-apply"></a><span data-ttu-id="148a8-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="148a8-103">RangeSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="148a8-104">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="148a8-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="148a8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="148a8-105">Permissions</span></span>
<span data-ttu-id="148a8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="148a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="148a8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="148a8-108">Permission type</span></span>      | <span data-ttu-id="148a8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="148a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="148a8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="148a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="148a8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="148a8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="148a8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="148a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="148a8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="148a8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="148a8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="148a8-114">Application</span></span> | <span data-ttu-id="148a8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="148a8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="148a8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="148a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="148a8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="148a8-117">Request headers</span></span>
| <span data-ttu-id="148a8-118">Name</span><span class="sxs-lookup"><span data-stu-id="148a8-118">Name</span></span>       | <span data-ttu-id="148a8-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="148a8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="148a8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="148a8-120">Authorization</span></span>  | <span data-ttu-id="148a8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="148a8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="148a8-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="148a8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="148a8-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="148a8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="148a8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="148a8-126">Request body</span></span>
<span data-ttu-id="148a8-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="148a8-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="148a8-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="148a8-128">Parameter</span></span>    | <span data-ttu-id="148a8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="148a8-129">Type</span></span>   |<span data-ttu-id="148a8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="148a8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="148a8-131">fields</span><span class="sxs-lookup"><span data-stu-id="148a8-131">fields</span></span>|<span data-ttu-id="148a8-132">SortField</span><span class="sxs-lookup"><span data-stu-id="148a8-132">SortField</span></span>|<span data-ttu-id="148a8-133">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="148a8-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="148a8-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="148a8-134">matchCase</span></span>|<span data-ttu-id="148a8-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="148a8-135">boolean</span></span>|<span data-ttu-id="148a8-p104">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="148a8-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="148a8-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="148a8-138">hasHeaders</span></span>|<span data-ttu-id="148a8-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="148a8-139">boolean</span></span>|<span data-ttu-id="148a8-p105">Optional. Gibt an, ob der Bereich eine Kopfzeile aufweist.</span><span class="sxs-lookup"><span data-stu-id="148a8-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="148a8-142">orientation</span><span class="sxs-lookup"><span data-stu-id="148a8-142">orientation</span></span>|<span data-ttu-id="148a8-143">string</span><span class="sxs-lookup"><span data-stu-id="148a8-143">string</span></span>|<span data-ttu-id="148a8-p106">Optional. Gibt an, ob der Vorgang Zeilen oder Spalten sortiert.  Die folgenden Werte sind möglich: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="148a8-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="148a8-147">Methode</span><span class="sxs-lookup"><span data-stu-id="148a8-147">method</span></span>|<span data-ttu-id="148a8-148">string</span><span class="sxs-lookup"><span data-stu-id="148a8-148">string</span></span>|<span data-ttu-id="148a8-p107">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="148a8-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="148a8-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="148a8-152">Response</span></span>

<span data-ttu-id="148a8-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="148a8-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="148a8-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="148a8-155">Example</span></span>
<span data-ttu-id="148a8-156">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="148a8-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="148a8-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="148a8-157">Request</span></span>
<span data-ttu-id="148a8-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="148a8-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="148a8-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="148a8-159">Response</span></span>
<span data-ttu-id="148a8-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="148a8-160">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangesort-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

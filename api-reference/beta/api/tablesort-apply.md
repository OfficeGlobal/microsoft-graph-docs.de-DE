---
title: 'TableSort: apply'
description: Führt einen Sortiervorgang aus.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2279109f83758958cb00940604854c4edeecd45
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523442"
---
# <a name="tablesort-apply"></a><span data-ttu-id="5eeb6-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="5eeb6-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eeb6-104">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="5eeb6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5eeb6-105">Permissions</span></span>
<span data-ttu-id="5eeb6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eeb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eeb6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5eeb6-108">Permission type</span></span>      | <span data-ttu-id="5eeb6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5eeb6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eeb6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5eeb6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5eeb6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eeb6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5eeb6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5eeb6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eeb6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eeb6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5eeb6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5eeb6-114">Application</span></span> | <span data-ttu-id="5eeb6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5eeb6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eeb6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5eeb6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="5eeb6-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5eeb6-117">Request headers</span></span>
| <span data-ttu-id="5eeb6-118">Name</span><span class="sxs-lookup"><span data-stu-id="5eeb6-118">Name</span></span>       | <span data-ttu-id="5eeb6-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5eeb6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5eeb6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eeb6-120">Authorization</span></span>  | <span data-ttu-id="5eeb6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5eeb6-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5eeb6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5eeb6-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eeb6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5eeb6-126">Request body</span></span>
<span data-ttu-id="5eeb6-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5eeb6-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="5eeb6-128">Parameter</span></span>    | <span data-ttu-id="5eeb6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5eeb6-129">Type</span></span>   |<span data-ttu-id="5eeb6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5eeb6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5eeb6-131">fields</span><span class="sxs-lookup"><span data-stu-id="5eeb6-131">fields</span></span>|<span data-ttu-id="5eeb6-132">SortField</span><span class="sxs-lookup"><span data-stu-id="5eeb6-132">SortField</span></span>|<span data-ttu-id="5eeb6-133">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="5eeb6-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="5eeb6-134">matchCase</span></span>|<span data-ttu-id="5eeb6-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5eeb6-135">boolean</span></span>|<span data-ttu-id="5eeb6-p104">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="5eeb6-138">method</span><span class="sxs-lookup"><span data-stu-id="5eeb6-138">method</span></span>|<span data-ttu-id="5eeb6-139">string</span><span class="sxs-lookup"><span data-stu-id="5eeb6-139">string</span></span>|<span data-ttu-id="5eeb6-p105">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="5eeb6-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="5eeb6-143">Response</span></span>

<span data-ttu-id="5eeb6-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eeb6-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5eeb6-146">Example</span></span>
<span data-ttu-id="5eeb6-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5eeb6-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5eeb6-148">Request</span></span>
<span data-ttu-id="5eeb6-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5eeb6-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="5eeb6-150">Response</span></span>
<span data-ttu-id="5eeb6-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5eeb6-151">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablesort-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

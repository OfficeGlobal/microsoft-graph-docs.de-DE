---
title: 'TableSort: apply'
description: Führt einen Sortiervorgang aus.
ms.openlocfilehash: 4c99ff84e88154cc4eb287f4a834590f685d535b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058411"
---
# <a name="tablesort-apply"></a><span data-ttu-id="ade83-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="ade83-103">TableSort: apply</span></span>

> <span data-ttu-id="ade83-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ade83-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ade83-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ade83-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ade83-106">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="ade83-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="ade83-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ade83-107">Permissions</span></span>
<span data-ttu-id="ade83-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ade83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ade83-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ade83-110">Permission type</span></span>      | <span data-ttu-id="ade83-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ade83-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ade83-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ade83-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ade83-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ade83-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ade83-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ade83-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ade83-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ade83-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ade83-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ade83-116">Application</span></span> | <span data-ttu-id="ade83-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ade83-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ade83-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ade83-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="ade83-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ade83-119">Request headers</span></span>
| <span data-ttu-id="ade83-120">Name</span><span class="sxs-lookup"><span data-stu-id="ade83-120">Name</span></span>       | <span data-ttu-id="ade83-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ade83-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ade83-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ade83-122">Authorization</span></span>  | <span data-ttu-id="ade83-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ade83-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ade83-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="ade83-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ade83-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="ade83-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ade83-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ade83-128">Request body</span></span>
<span data-ttu-id="ade83-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ade83-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ade83-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="ade83-130">Parameter</span></span>    | <span data-ttu-id="ade83-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ade83-131">Type</span></span>   |<span data-ttu-id="ade83-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ade83-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ade83-133">fields</span><span class="sxs-lookup"><span data-stu-id="ade83-133">fields</span></span>|<span data-ttu-id="ade83-134">SortField</span><span class="sxs-lookup"><span data-stu-id="ade83-134">SortField</span></span>|<span data-ttu-id="ade83-135">Die Liste der Bedingungen, nach denen sortiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ade83-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="ade83-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="ade83-136">matchCase</span></span>|<span data-ttu-id="ade83-137">boolean</span><span class="sxs-lookup"><span data-stu-id="ade83-137">boolean</span></span>|<span data-ttu-id="ade83-p105">Optional. Gibt an, ob sich die Groß-/Kleinschreibung auf die Zeichenfolgensortierung auswirkt.</span><span class="sxs-lookup"><span data-stu-id="ade83-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="ade83-140">method</span><span class="sxs-lookup"><span data-stu-id="ade83-140">method</span></span>|<span data-ttu-id="ade83-141">string</span><span class="sxs-lookup"><span data-stu-id="ade83-141">string</span></span>|<span data-ttu-id="ade83-p106">Optional. Die Sortiermethode für chinesische Zeichen.  Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="ade83-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="ade83-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="ade83-145">Response</span></span>

<span data-ttu-id="ade83-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ade83-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ade83-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ade83-148">Example</span></span>
<span data-ttu-id="ade83-149">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ade83-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ade83-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ade83-150">Request</span></span>
<span data-ttu-id="ade83-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ade83-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ade83-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="ade83-152">Response</span></span>
<span data-ttu-id="ade83-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ade83-153">Here is an example of the response.</span></span> 
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
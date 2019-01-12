---
title: 'Range: merge'
description: Führt die Zellen des Bereichs in einen Bereich im Arbeitsblatt zusammen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 151163604bc7eada167daebdb325857cc6e87ce4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990523"
---
# <a name="range-merge"></a><span data-ttu-id="0b2cf-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="0b2cf-103">Range: merge</span></span>

> <span data-ttu-id="0b2cf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b2cf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b2cf-106">Führt die Zellen des Bereichs in einen Bereich im Arbeitsblatt zusammen.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-106">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b2cf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0b2cf-107">Permissions</span></span>
<span data-ttu-id="0b2cf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b2cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b2cf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b2cf-110">Permission type</span></span>      | <span data-ttu-id="0b2cf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b2cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b2cf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b2cf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0b2cf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b2cf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b2cf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b2cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b2cf-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b2cf-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b2cf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b2cf-116">Application</span></span> | <span data-ttu-id="0b2cf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b2cf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b2cf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b2cf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="0b2cf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b2cf-119">Request headers</span></span>
| <span data-ttu-id="0b2cf-120">Name</span><span class="sxs-lookup"><span data-stu-id="0b2cf-120">Name</span></span>       | <span data-ttu-id="0b2cf-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b2cf-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0b2cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b2cf-122">Authorization</span></span>  | <span data-ttu-id="0b2cf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b2cf-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="0b2cf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b2cf-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b2cf-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b2cf-128">Request body</span></span>
<span data-ttu-id="0b2cf-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0b2cf-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="0b2cf-130">Parameter</span></span>    | <span data-ttu-id="0b2cf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0b2cf-131">Type</span></span>   |<span data-ttu-id="0b2cf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b2cf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b2cf-133">across</span><span class="sxs-lookup"><span data-stu-id="0b2cf-133">across</span></span>|<span data-ttu-id="0b2cf-134">boolean</span><span class="sxs-lookup"><span data-stu-id="0b2cf-134">boolean</span></span>|<span data-ttu-id="0b2cf-p105">Optional. Mit „true“ werden Zellen in allen Zeilen des angegebenen Bereichs als einzelne zusammengeführte Zellen zusammengeführt. Der Standardwert lautet „false“.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-p105">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="0b2cf-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b2cf-138">Response</span></span>

<span data-ttu-id="0b2cf-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b2cf-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b2cf-141">Example</span></span>
<span data-ttu-id="0b2cf-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0b2cf-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b2cf-143">Request</span></span>
<span data-ttu-id="0b2cf-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="0b2cf-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b2cf-145">Response</span></span>
<span data-ttu-id="0b2cf-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0b2cf-146">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

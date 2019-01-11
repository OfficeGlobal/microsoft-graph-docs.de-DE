---
title: 'Range: delete'
description: Löscht die einem Bereich zugeordneten Zellen.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 1817a1c1481d86e08de4146215da6f6fc8de6a8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871785"
---
# <a name="range-delete"></a><span data-ttu-id="59037-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="59037-103">Range: delete</span></span>

> <span data-ttu-id="59037-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="59037-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59037-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59037-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59037-106">Löscht die einem Bereich zugeordneten Zellen.</span><span class="sxs-lookup"><span data-stu-id="59037-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="59037-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="59037-107">Permissions</span></span>
<span data-ttu-id="59037-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59037-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59037-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59037-110">Permission type</span></span>      | <span data-ttu-id="59037-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59037-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59037-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59037-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59037-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59037-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59037-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59037-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59037-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59037-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59037-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59037-116">Application</span></span> | <span data-ttu-id="59037-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59037-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59037-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59037-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="59037-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59037-119">Request headers</span></span>
| <span data-ttu-id="59037-120">Name</span><span class="sxs-lookup"><span data-stu-id="59037-120">Name</span></span>       | <span data-ttu-id="59037-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59037-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59037-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59037-122">Authorization</span></span>  | <span data-ttu-id="59037-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="59037-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59037-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="59037-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="59037-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="59037-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59037-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59037-128">Request body</span></span>
<span data-ttu-id="59037-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="59037-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59037-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="59037-130">Parameter</span></span>    | <span data-ttu-id="59037-131">Typ</span><span class="sxs-lookup"><span data-stu-id="59037-131">Type</span></span>   |<span data-ttu-id="59037-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59037-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59037-133">Shift</span><span class="sxs-lookup"><span data-stu-id="59037-133">shift</span></span>|<span data-ttu-id="59037-134">string</span><span class="sxs-lookup"><span data-stu-id="59037-134">string</span></span>|<span data-ttu-id="59037-p105">Gibt an, wohin die Zellen verschoben werden.  Mögliche Werte: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="59037-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="59037-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="59037-137">Response</span></span>

<span data-ttu-id="59037-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59037-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59037-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59037-140">Example</span></span>
<span data-ttu-id="59037-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="59037-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="59037-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59037-142">Request</span></span>
<span data-ttu-id="59037-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59037-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="59037-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="59037-144">Response</span></span>
<span data-ttu-id="59037-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="59037-145">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

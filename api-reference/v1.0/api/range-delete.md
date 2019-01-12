---
title: 'Range: delete'
description: Löscht die einem Bereich zugeordneten Zellen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 671dc5785aae4d912d60c2356fc7b1a204630c3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941600"
---
# <a name="range-delete"></a><span data-ttu-id="be504-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="be504-103">Range: delete</span></span>

<span data-ttu-id="be504-104">Löscht die einem Bereich zugeordneten Zellen.</span><span class="sxs-lookup"><span data-stu-id="be504-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="be504-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be504-105">Permissions</span></span>
<span data-ttu-id="be504-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be504-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be504-108">Permission type</span></span>      | <span data-ttu-id="be504-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be504-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be504-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be504-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be504-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be504-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be504-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be504-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be504-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be504-113">Not supported.</span></span>    |
|<span data-ttu-id="be504-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be504-114">Application</span></span> | <span data-ttu-id="be504-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="be504-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be504-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be504-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="be504-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be504-117">Request headers</span></span>
| <span data-ttu-id="be504-118">Name</span><span class="sxs-lookup"><span data-stu-id="be504-118">Name</span></span>       | <span data-ttu-id="be504-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be504-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be504-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="be504-120">Authorization</span></span>  | <span data-ttu-id="be504-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="be504-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be504-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="be504-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="be504-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="be504-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be504-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be504-126">Request body</span></span>
<span data-ttu-id="be504-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="be504-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="be504-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="be504-128">Parameter</span></span>    | <span data-ttu-id="be504-129">Typ</span><span class="sxs-lookup"><span data-stu-id="be504-129">Type</span></span>   |<span data-ttu-id="be504-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be504-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be504-131">Shift</span><span class="sxs-lookup"><span data-stu-id="be504-131">shift</span></span>|<span data-ttu-id="be504-132">string</span><span class="sxs-lookup"><span data-stu-id="be504-132">string</span></span>|<span data-ttu-id="be504-133">Gibt an, wie die Zellen verschoben.</span><span class="sxs-lookup"><span data-stu-id="be504-133">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="be504-134">Die möglichen Werte sind: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="be504-134">The possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="be504-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="be504-135">Response</span></span>

<span data-ttu-id="be504-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be504-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be504-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be504-138">Example</span></span>
<span data-ttu-id="be504-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="be504-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="be504-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="be504-140">Request</span></span>
<span data-ttu-id="be504-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="be504-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="be504-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="be504-142">Response</span></span>
<span data-ttu-id="be504-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be504-143">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'Range: delete'
description: Löscht die einem Bereich zugeordneten Zellen.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2a3ea63884964f1c1eb2b423c459fcae3ba6bfb1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931342"
---
# <a name="range-delete"></a><span data-ttu-id="c378b-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="c378b-103">Range: delete</span></span>

> <span data-ttu-id="c378b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c378b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c378b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c378b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c378b-106">Löscht die einem Bereich zugeordneten Zellen.</span><span class="sxs-lookup"><span data-stu-id="c378b-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="c378b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c378b-107">Permissions</span></span>
<span data-ttu-id="c378b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c378b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c378b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c378b-110">Permission type</span></span>      | <span data-ttu-id="c378b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c378b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c378b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c378b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c378b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c378b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c378b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c378b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c378b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c378b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c378b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c378b-116">Application</span></span> | <span data-ttu-id="c378b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c378b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c378b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c378b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="c378b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c378b-119">Request headers</span></span>
| <span data-ttu-id="c378b-120">Name</span><span class="sxs-lookup"><span data-stu-id="c378b-120">Name</span></span>       | <span data-ttu-id="c378b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c378b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c378b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c378b-122">Authorization</span></span>  | <span data-ttu-id="c378b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c378b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c378b-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c378b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c378b-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c378b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c378b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c378b-128">Request body</span></span>
<span data-ttu-id="c378b-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c378b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c378b-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="c378b-130">Parameter</span></span>    | <span data-ttu-id="c378b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c378b-131">Type</span></span>   |<span data-ttu-id="c378b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c378b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c378b-133">Shift</span><span class="sxs-lookup"><span data-stu-id="c378b-133">shift</span></span>|<span data-ttu-id="c378b-134">string</span><span class="sxs-lookup"><span data-stu-id="c378b-134">string</span></span>|<span data-ttu-id="c378b-p105">Gibt an, wohin die Zellen verschoben werden.  Mögliche Werte: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="c378b-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="c378b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c378b-137">Response</span></span>

<span data-ttu-id="c378b-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c378b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c378b-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c378b-140">Example</span></span>
<span data-ttu-id="c378b-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c378b-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c378b-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c378b-142">Request</span></span>
<span data-ttu-id="c378b-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c378b-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c378b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="c378b-144">Response</span></span>
<span data-ttu-id="c378b-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c378b-145">Here is an example of the response.</span></span> 
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

---
title: 'TableRow: delete'
description: Löscht die Zeile aus der Tabelle.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: cea9f8a0801fed24f8767c6929573c729db82d17
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861431"
---
# <a name="tablerow-delete"></a><span data-ttu-id="5034f-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="5034f-103">TableRow: delete</span></span>

> <span data-ttu-id="5034f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5034f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5034f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5034f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5034f-106">Löscht die Zeile aus der Tabelle.</span><span class="sxs-lookup"><span data-stu-id="5034f-106">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5034f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5034f-107">Permissions</span></span>
<span data-ttu-id="5034f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5034f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5034f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5034f-110">Permission type</span></span>      | <span data-ttu-id="5034f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5034f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5034f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5034f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5034f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5034f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5034f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5034f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5034f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5034f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5034f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5034f-116">Application</span></span> | <span data-ttu-id="5034f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5034f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5034f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5034f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="5034f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5034f-119">Request headers</span></span>
| <span data-ttu-id="5034f-120">Name</span><span class="sxs-lookup"><span data-stu-id="5034f-120">Name</span></span>       | <span data-ttu-id="5034f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5034f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5034f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5034f-122">Authorization</span></span>  | <span data-ttu-id="5034f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5034f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5034f-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5034f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5034f-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5034f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5034f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5034f-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5034f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5034f-129">Response</span></span>

<span data-ttu-id="5034f-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5034f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5034f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5034f-132">Example</span></span>
<span data-ttu-id="5034f-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5034f-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5034f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5034f-134">Request</span></span>
<span data-ttu-id="5034f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5034f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/delete
```

##### <a name="response"></a><span data-ttu-id="5034f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5034f-136">Response</span></span>
<span data-ttu-id="5034f-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5034f-137">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

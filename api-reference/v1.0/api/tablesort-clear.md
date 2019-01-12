---
title: 'TableSort: clear'
description: Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 90ac8b30c3b8513bdd73fa40746268212a8c0df9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912190"
---
# <a name="tablesort-clear"></a><span data-ttu-id="105f3-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="105f3-104">TableSort: clear</span></span>

<span data-ttu-id="105f3-p102">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="105f3-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="105f3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="105f3-107">Permissions</span></span>
<span data-ttu-id="105f3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="105f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="105f3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="105f3-110">Permission type</span></span>      | <span data-ttu-id="105f3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="105f3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="105f3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="105f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="105f3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="105f3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="105f3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="105f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="105f3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="105f3-115">Not supported.</span></span>    |
|<span data-ttu-id="105f3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="105f3-116">Application</span></span> | <span data-ttu-id="105f3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="105f3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="105f3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="105f3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="105f3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="105f3-119">Request headers</span></span>
| <span data-ttu-id="105f3-120">Name</span><span class="sxs-lookup"><span data-stu-id="105f3-120">Name</span></span>       | <span data-ttu-id="105f3-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="105f3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="105f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="105f3-122">Authorization</span></span>  | <span data-ttu-id="105f3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="105f3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="105f3-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="105f3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="105f3-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="105f3-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="105f3-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="105f3-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="105f3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="105f3-129">Response</span></span>

<span data-ttu-id="105f3-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="105f3-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="105f3-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="105f3-132">Example</span></span>
<span data-ttu-id="105f3-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="105f3-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="105f3-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="105f3-134">Request</span></span>
<span data-ttu-id="105f3-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="105f3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="105f3-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="105f3-136">Response</span></span>
<span data-ttu-id="105f3-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="105f3-137">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

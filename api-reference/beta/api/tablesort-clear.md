---
title: 'TableSort: clear'
description: Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.
ms.openlocfilehash: f93b640188faedc228c56b6e13497ade84190765
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065017"
---
# <a name="tablesort-clear"></a><span data-ttu-id="80f94-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="80f94-104">TableSort: clear</span></span>

> <span data-ttu-id="80f94-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80f94-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80f94-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80f94-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80f94-p103">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="80f94-p103">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="80f94-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="80f94-109">Permissions</span></span>
<span data-ttu-id="80f94-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80f94-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80f94-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80f94-112">Permission type</span></span>      | <span data-ttu-id="80f94-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80f94-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80f94-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80f94-114">Delegated (work or school account)</span></span> | <span data-ttu-id="80f94-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80f94-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="80f94-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80f94-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80f94-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80f94-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="80f94-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80f94-118">Application</span></span> | <span data-ttu-id="80f94-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80f94-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80f94-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80f94-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="80f94-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80f94-121">Request headers</span></span>
| <span data-ttu-id="80f94-122">Name</span><span class="sxs-lookup"><span data-stu-id="80f94-122">Name</span></span>       | <span data-ttu-id="80f94-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80f94-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80f94-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="80f94-124">Authorization</span></span>  | <span data-ttu-id="80f94-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80f94-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80f94-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="80f94-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="80f94-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="80f94-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80f94-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80f94-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="80f94-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="80f94-131">Response</span></span>

<span data-ttu-id="80f94-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80f94-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80f94-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80f94-134">Example</span></span>
<span data-ttu-id="80f94-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="80f94-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80f94-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80f94-136">Request</span></span>
<span data-ttu-id="80f94-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80f94-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="80f94-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="80f94-138">Response</span></span>
<span data-ttu-id="80f94-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="80f94-139">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
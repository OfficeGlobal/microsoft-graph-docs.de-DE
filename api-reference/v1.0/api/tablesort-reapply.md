---
title: 'TableSort: reapply'
description: Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.
author: lumine2008
ms.openlocfilehash: 4ce369ed95d8940a34b02f6e406042123529cf5e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306860"
---
# <a name="tablesort-reapply"></a><span data-ttu-id="41f03-103">TableSort: reapply</span><span class="sxs-lookup"><span data-stu-id="41f03-103">TableSort: reapply</span></span>

<span data-ttu-id="41f03-104">Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="41f03-104">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="41f03-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="41f03-105">Permissions</span></span>
<span data-ttu-id="41f03-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41f03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41f03-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41f03-108">Permission type</span></span>      | <span data-ttu-id="41f03-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41f03-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41f03-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41f03-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41f03-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41f03-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="41f03-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41f03-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41f03-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41f03-113">Not supported.</span></span>    |
|<span data-ttu-id="41f03-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41f03-114">Application</span></span> | <span data-ttu-id="41f03-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41f03-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41f03-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41f03-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="41f03-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41f03-117">Request headers</span></span>
| <span data-ttu-id="41f03-118">Name</span><span class="sxs-lookup"><span data-stu-id="41f03-118">Name</span></span>       | <span data-ttu-id="41f03-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41f03-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="41f03-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="41f03-120">Authorization</span></span>  | <span data-ttu-id="41f03-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="41f03-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41f03-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="41f03-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="41f03-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="41f03-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41f03-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="41f03-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="41f03-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="41f03-127">Response</span></span>

<span data-ttu-id="41f03-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41f03-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41f03-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41f03-130">Example</span></span>
<span data-ttu-id="41f03-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="41f03-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="41f03-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41f03-132">Request</span></span>
<span data-ttu-id="41f03-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41f03-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```

##### <a name="response"></a><span data-ttu-id="41f03-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="41f03-134">Response</span></span>
<span data-ttu-id="41f03-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="41f03-135">Here is an example of the response.</span></span> 
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
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
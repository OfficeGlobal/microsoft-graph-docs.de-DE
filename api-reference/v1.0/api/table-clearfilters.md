---
title: 'Table: clearFilters'
description: Löscht alle Filter, die derzeit in der Tabelle verwendet werden.
ms.openlocfilehash: a7f560fad24727e1af49cb69ce754036f83b4345
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016961"
---
# <a name="table-clearfilters"></a><span data-ttu-id="152bf-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="152bf-103">Table: clearFilters</span></span>

<span data-ttu-id="152bf-104">Löscht alle Filter, die derzeit in der Tabelle verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="152bf-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="152bf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="152bf-105">Permissions</span></span>
<span data-ttu-id="152bf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="152bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="152bf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="152bf-108">Permission type</span></span>      | <span data-ttu-id="152bf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="152bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="152bf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="152bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="152bf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="152bf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="152bf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="152bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="152bf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="152bf-113">Not supported.</span></span>    |
|<span data-ttu-id="152bf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="152bf-114">Application</span></span> | <span data-ttu-id="152bf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="152bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="152bf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="152bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="152bf-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="152bf-117">Request headers</span></span>
| <span data-ttu-id="152bf-118">Name</span><span class="sxs-lookup"><span data-stu-id="152bf-118">Name</span></span>       | <span data-ttu-id="152bf-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="152bf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="152bf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="152bf-120">Authorization</span></span>  | <span data-ttu-id="152bf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="152bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="152bf-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="152bf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="152bf-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="152bf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="152bf-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="152bf-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="152bf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="152bf-127">Response</span></span>

<span data-ttu-id="152bf-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="152bf-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="152bf-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="152bf-130">Example</span></span>
<span data-ttu-id="152bf-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="152bf-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="152bf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="152bf-132">Request</span></span>
<span data-ttu-id="152bf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="152bf-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```

##### <a name="response"></a><span data-ttu-id="152bf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="152bf-134">Response</span></span>
<span data-ttu-id="152bf-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="152bf-135">Here is an example of the response.</span></span> 
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
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
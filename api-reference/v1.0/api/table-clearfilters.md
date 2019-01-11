---
title: 'Table: clearFilters'
description: Löscht alle Filter, die derzeit in der Tabelle verwendet werden.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 781af9b09270d2e165113edd03dcb25fc0ecfeab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889754"
---
# <a name="table-clearfilters"></a><span data-ttu-id="de9c7-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="de9c7-103">Table: clearFilters</span></span>

<span data-ttu-id="de9c7-104">Löscht alle Filter, die derzeit in der Tabelle verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="de9c7-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="de9c7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="de9c7-105">Permissions</span></span>
<span data-ttu-id="de9c7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de9c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de9c7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de9c7-108">Permission type</span></span>      | <span data-ttu-id="de9c7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de9c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de9c7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de9c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de9c7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de9c7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de9c7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de9c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de9c7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de9c7-113">Not supported.</span></span>    |
|<span data-ttu-id="de9c7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de9c7-114">Application</span></span> | <span data-ttu-id="de9c7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de9c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de9c7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de9c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="de9c7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de9c7-117">Request headers</span></span>
| <span data-ttu-id="de9c7-118">Name</span><span class="sxs-lookup"><span data-stu-id="de9c7-118">Name</span></span>       | <span data-ttu-id="de9c7-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de9c7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="de9c7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de9c7-120">Authorization</span></span>  | <span data-ttu-id="de9c7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de9c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de9c7-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="de9c7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="de9c7-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="de9c7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de9c7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de9c7-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="de9c7-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="de9c7-127">Response</span></span>

<span data-ttu-id="de9c7-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de9c7-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de9c7-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de9c7-130">Example</span></span>
<span data-ttu-id="de9c7-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="de9c7-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="de9c7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de9c7-132">Request</span></span>
<span data-ttu-id="de9c7-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de9c7-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```

##### <a name="response"></a><span data-ttu-id="de9c7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="de9c7-134">Response</span></span>
<span data-ttu-id="de9c7-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="de9c7-135">Here is an example of the response.</span></span> 
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

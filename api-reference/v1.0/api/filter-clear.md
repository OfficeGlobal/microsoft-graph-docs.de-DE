---
title: Filter deaktivieren
description: Deaktiviert den Filter für die angegebene Spalte.
ms.openlocfilehash: 85a9249cf70ffdd44b8b84e0d28bec63ca743ca1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017958"
---
# <a name="filter-clear"></a><span data-ttu-id="50ef4-103">Filter deaktivieren</span><span class="sxs-lookup"><span data-stu-id="50ef4-103">Filter: clear</span></span>

<span data-ttu-id="50ef4-104">Deaktiviert den Filter für die angegebene Spalte.</span><span class="sxs-lookup"><span data-stu-id="50ef4-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="50ef4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="50ef4-105">Permissions</span></span>
<span data-ttu-id="50ef4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50ef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ef4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50ef4-108">Permission type</span></span>      | <span data-ttu-id="50ef4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50ef4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50ef4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50ef4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50ef4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50ef4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50ef4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50ef4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50ef4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50ef4-113">Not supported.</span></span>    |
|<span data-ttu-id="50ef4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50ef4-114">Application</span></span> | <span data-ttu-id="50ef4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50ef4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50ef4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50ef4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="50ef4-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50ef4-117">Request headers</span></span>
| <span data-ttu-id="50ef4-118">Name</span><span class="sxs-lookup"><span data-stu-id="50ef4-118">Name</span></span>       | <span data-ttu-id="50ef4-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50ef4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="50ef4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="50ef4-120">Authorization</span></span>  | <span data-ttu-id="50ef4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50ef4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50ef4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50ef4-123">Request body</span></span>
<span data-ttu-id="50ef4-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="50ef4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50ef4-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="50ef4-125">Response</span></span>

<span data-ttu-id="50ef4-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50ef4-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50ef4-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50ef4-128">Example</span></span>
<span data-ttu-id="50ef4-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="50ef4-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="50ef4-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50ef4-130">Request</span></span>
<span data-ttu-id="50ef4-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50ef4-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="50ef4-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="50ef4-132">Response</span></span>
<span data-ttu-id="50ef4-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="50ef4-133">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
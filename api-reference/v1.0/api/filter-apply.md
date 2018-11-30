---
title: 'Filter: apply'
description: Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.
ms.openlocfilehash: b60c3da521f2b5700650450d308b7f26fcd4d1a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017361"
---
# <a name="filter-apply"></a><span data-ttu-id="366b9-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="366b9-103">Filter: apply</span></span>

<span data-ttu-id="366b9-104">Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.</span><span class="sxs-lookup"><span data-stu-id="366b9-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="366b9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="366b9-105">Permissions</span></span>
<span data-ttu-id="366b9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="366b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="366b9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="366b9-108">Permission type</span></span>      | <span data-ttu-id="366b9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="366b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="366b9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="366b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="366b9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="366b9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="366b9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="366b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="366b9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="366b9-113">Not supported.</span></span>    |
|<span data-ttu-id="366b9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="366b9-114">Application</span></span> | <span data-ttu-id="366b9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="366b9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="366b9-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="366b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="366b9-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="366b9-117">Request headers</span></span>
| <span data-ttu-id="366b9-118">Name</span><span class="sxs-lookup"><span data-stu-id="366b9-118">Name</span></span>       | <span data-ttu-id="366b9-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="366b9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="366b9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="366b9-120">Authorization</span></span>  | <span data-ttu-id="366b9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="366b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="366b9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="366b9-123">Request body</span></span>
<span data-ttu-id="366b9-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="366b9-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="366b9-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="366b9-125">Parameter</span></span>    | <span data-ttu-id="366b9-126">Typ</span><span class="sxs-lookup"><span data-stu-id="366b9-126">Type</span></span>   |<span data-ttu-id="366b9-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="366b9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="366b9-128">criteria</span><span class="sxs-lookup"><span data-stu-id="366b9-128">criteria</span></span>|<span data-ttu-id="366b9-129">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="366b9-129">WorkbookFilterCriteria</span></span>|<span data-ttu-id="366b9-130">Die Kriterien, die angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="366b9-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="366b9-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="366b9-131">Response</span></span>

<span data-ttu-id="366b9-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="366b9-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="366b9-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="366b9-134">Example</span></span>
<span data-ttu-id="366b9-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="366b9-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="366b9-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="366b9-136">Request</span></span>
<span data-ttu-id="366b9-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="366b9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="366b9-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="366b9-138">Response</span></span>
<span data-ttu-id="366b9-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="366b9-139">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
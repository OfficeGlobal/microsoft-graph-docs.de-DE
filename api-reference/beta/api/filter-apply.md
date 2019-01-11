---
title: 'Filter: apply'
description: Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.
localization_priority: Normal
ms.openlocfilehash: 3b37344ae3047b54488fa0dd95944c0f34e3bd2b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882901"
---
# <a name="filter-apply"></a><span data-ttu-id="6de3d-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="6de3d-103">Filter: apply</span></span>

> <span data-ttu-id="6de3d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6de3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6de3d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6de3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6de3d-106">Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.</span><span class="sxs-lookup"><span data-stu-id="6de3d-106">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="6de3d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6de3d-107">Permissions</span></span>
<span data-ttu-id="6de3d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6de3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6de3d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6de3d-110">Permission type</span></span>      | <span data-ttu-id="6de3d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6de3d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6de3d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6de3d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6de3d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6de3d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6de3d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6de3d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6de3d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6de3d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6de3d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6de3d-116">Application</span></span> | <span data-ttu-id="6de3d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6de3d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6de3d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6de3d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="6de3d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6de3d-119">Request headers</span></span>
| <span data-ttu-id="6de3d-120">Name</span><span class="sxs-lookup"><span data-stu-id="6de3d-120">Name</span></span>       | <span data-ttu-id="6de3d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6de3d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6de3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6de3d-122">Authorization</span></span>  | <span data-ttu-id="6de3d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6de3d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6de3d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6de3d-125">Request body</span></span>
<span data-ttu-id="6de3d-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6de3d-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6de3d-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="6de3d-127">Parameter</span></span>    | <span data-ttu-id="6de3d-128">Typ</span><span class="sxs-lookup"><span data-stu-id="6de3d-128">Type</span></span>   |<span data-ttu-id="6de3d-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6de3d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6de3d-130">criteria</span><span class="sxs-lookup"><span data-stu-id="6de3d-130">criteria</span></span>|<span data-ttu-id="6de3d-131">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="6de3d-131">FilterCriteria</span></span>|<span data-ttu-id="6de3d-132">Die Kriterien, die angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6de3d-132">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="6de3d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6de3d-133">Response</span></span>

<span data-ttu-id="6de3d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6de3d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6de3d-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6de3d-136">Example</span></span>
<span data-ttu-id="6de3d-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6de3d-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6de3d-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6de3d-138">Request</span></span>
<span data-ttu-id="6de3d-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6de3d-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
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

##### <a name="response"></a><span data-ttu-id="6de3d-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="6de3d-140">Response</span></span>
<span data-ttu-id="6de3d-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6de3d-141">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

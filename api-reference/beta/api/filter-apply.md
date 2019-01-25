---
title: 'Filter: apply'
description: Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.
localization_priority: Normal
ms.openlocfilehash: 03afb7b3bbbf190abdffba888f4b01d5be04f980
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513592"
---
# <a name="filter-apply"></a><span data-ttu-id="3e03a-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="3e03a-103">Filter: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e03a-104">Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.</span><span class="sxs-lookup"><span data-stu-id="3e03a-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e03a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3e03a-105">Permissions</span></span>
<span data-ttu-id="3e03a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e03a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e03a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e03a-108">Permission type</span></span>      | <span data-ttu-id="3e03a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e03a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e03a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e03a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e03a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e03a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e03a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e03a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e03a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e03a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e03a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e03a-114">Application</span></span> | <span data-ttu-id="3e03a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e03a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e03a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e03a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="3e03a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e03a-117">Request headers</span></span>
| <span data-ttu-id="3e03a-118">Name</span><span class="sxs-lookup"><span data-stu-id="3e03a-118">Name</span></span>       | <span data-ttu-id="3e03a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e03a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e03a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e03a-120">Authorization</span></span>  | <span data-ttu-id="3e03a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e03a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e03a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e03a-123">Request body</span></span>
<span data-ttu-id="3e03a-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="3e03a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e03a-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="3e03a-125">Parameter</span></span>    | <span data-ttu-id="3e03a-126">Typ</span><span class="sxs-lookup"><span data-stu-id="3e03a-126">Type</span></span>   |<span data-ttu-id="3e03a-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e03a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e03a-128">criteria</span><span class="sxs-lookup"><span data-stu-id="3e03a-128">criteria</span></span>|<span data-ttu-id="3e03a-129">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="3e03a-129">FilterCriteria</span></span>|<span data-ttu-id="3e03a-130">Die Kriterien, die angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3e03a-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="3e03a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e03a-131">Response</span></span>

<span data-ttu-id="3e03a-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e03a-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e03a-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e03a-134">Example</span></span>
<span data-ttu-id="3e03a-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3e03a-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3e03a-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e03a-136">Request</span></span>
<span data-ttu-id="3e03a-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e03a-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3e03a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e03a-138">Response</span></span>
<span data-ttu-id="3e03a-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3e03a-139">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/filter-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

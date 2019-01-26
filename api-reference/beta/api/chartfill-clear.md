---
title: 'ChartFill: clear'
description: Dient zum Löschen der Füllfarbe eines Diagrammelements.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6a053814b1be4fdee947d4d28911263b7e53d55d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573039"
---
# <a name="chartfill-clear"></a><span data-ttu-id="d7b90-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="d7b90-103">ChartFill: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7b90-104">Dient zum Löschen der Füllfarbe eines Diagrammelements.</span><span class="sxs-lookup"><span data-stu-id="d7b90-104">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7b90-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7b90-105">Permissions</span></span>
<span data-ttu-id="d7b90-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7b90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7b90-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7b90-108">Permission type</span></span>      | <span data-ttu-id="d7b90-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7b90-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7b90-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7b90-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7b90-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7b90-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7b90-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7b90-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7b90-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7b90-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7b90-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7b90-114">Application</span></span> | <span data-ttu-id="d7b90-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7b90-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7b90-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7b90-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="d7b90-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7b90-117">Request headers</span></span>
| <span data-ttu-id="d7b90-118">Name</span><span class="sxs-lookup"><span data-stu-id="d7b90-118">Name</span></span>       | <span data-ttu-id="d7b90-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7b90-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7b90-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7b90-120">Authorization</span></span>  | <span data-ttu-id="d7b90-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7b90-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7b90-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="d7b90-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7b90-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="d7b90-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7b90-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7b90-126">Request body</span></span>
<span data-ttu-id="d7b90-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7b90-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7b90-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7b90-128">Response</span></span>

<span data-ttu-id="d7b90-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7b90-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7b90-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7b90-131">Example</span></span>
<span data-ttu-id="d7b90-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="d7b90-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7b90-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7b90-133">Request</span></span>
<span data-ttu-id="d7b90-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7b90-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="d7b90-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7b90-135">Response</span></span>
<span data-ttu-id="d7b90-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d7b90-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartfill-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

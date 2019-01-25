---
title: 'Tabelle: reapplyFilters'
description: Wendet alle Filter erneut an, die derzeit in der Tabelle vorhanden sind.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b687d3cbf89d68f89d7e854bb3d7171427d8e466
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522889"
---
# <a name="table-reapplyfilters"></a><span data-ttu-id="354bb-103">Tabelle: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="354bb-103">Table: reapplyFilters</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="354bb-104">Wendet alle Filter erneut an, die derzeit in der Tabelle vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="354bb-104">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="354bb-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="354bb-105">Permissions</span></span>
<span data-ttu-id="354bb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="354bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="354bb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="354bb-108">Permission type</span></span>      | <span data-ttu-id="354bb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="354bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="354bb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="354bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="354bb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="354bb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="354bb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="354bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="354bb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="354bb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="354bb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="354bb-114">Application</span></span> | <span data-ttu-id="354bb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="354bb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="354bb-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="354bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="354bb-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="354bb-117">Request headers</span></span>
| <span data-ttu-id="354bb-118">Name</span><span class="sxs-lookup"><span data-stu-id="354bb-118">Name</span></span>       | <span data-ttu-id="354bb-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="354bb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="354bb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="354bb-120">Authorization</span></span>  | <span data-ttu-id="354bb-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="354bb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="354bb-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="354bb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="354bb-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="354bb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="354bb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="354bb-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="354bb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="354bb-127">Response</span></span>

<span data-ttu-id="354bb-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="354bb-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="354bb-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="354bb-130">Example</span></span>
<span data-ttu-id="354bb-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="354bb-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="354bb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="354bb-132">Request</span></span>
<span data-ttu-id="354bb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="354bb-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="354bb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="354bb-134">Response</span></span>
<span data-ttu-id="354bb-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="354bb-135">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-reapplyfilters.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

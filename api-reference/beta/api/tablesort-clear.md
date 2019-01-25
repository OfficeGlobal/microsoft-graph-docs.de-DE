---
title: 'TableSort: clear'
description: Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5097498c1221a7cfd2e231232540cbef2d34a66e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521460"
---
# <a name="tablesort-clear"></a><span data-ttu-id="32ed6-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="32ed6-104">TableSort: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32ed6-p102">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="32ed6-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="32ed6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="32ed6-107">Permissions</span></span>
<span data-ttu-id="32ed6-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32ed6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32ed6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32ed6-110">Permission type</span></span>      | <span data-ttu-id="32ed6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32ed6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32ed6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32ed6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="32ed6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32ed6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="32ed6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32ed6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32ed6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32ed6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="32ed6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32ed6-116">Application</span></span> | <span data-ttu-id="32ed6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32ed6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32ed6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32ed6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="32ed6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32ed6-119">Request headers</span></span>
| <span data-ttu-id="32ed6-120">Name</span><span class="sxs-lookup"><span data-stu-id="32ed6-120">Name</span></span>       | <span data-ttu-id="32ed6-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32ed6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="32ed6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32ed6-122">Authorization</span></span>  | <span data-ttu-id="32ed6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32ed6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32ed6-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="32ed6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="32ed6-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="32ed6-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32ed6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32ed6-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="32ed6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="32ed6-129">Response</span></span>

<span data-ttu-id="32ed6-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32ed6-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32ed6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32ed6-132">Example</span></span>
<span data-ttu-id="32ed6-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="32ed6-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="32ed6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32ed6-134">Request</span></span>
<span data-ttu-id="32ed6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32ed6-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="32ed6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="32ed6-136">Response</span></span>
<span data-ttu-id="32ed6-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="32ed6-137">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablesort-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

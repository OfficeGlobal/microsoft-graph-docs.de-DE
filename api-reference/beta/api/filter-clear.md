---
title: Filter deaktivieren
description: Deaktiviert den Filter für die angegebene Spalte.
localization_priority: Normal
ms.openlocfilehash: 3567ee187a9b3becb1afa296c97cc7c3442bf667
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518037"
---
# <a name="filter-clear"></a><span data-ttu-id="4b357-103">Filter deaktivieren</span><span class="sxs-lookup"><span data-stu-id="4b357-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b357-104">Deaktiviert den Filter für die angegebene Spalte.</span><span class="sxs-lookup"><span data-stu-id="4b357-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b357-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4b357-105">Permissions</span></span>
<span data-ttu-id="4b357-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b357-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b357-108">Permission type</span></span>      | <span data-ttu-id="4b357-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b357-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b357-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b357-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b357-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b357-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b357-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b357-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b357-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b357-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b357-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b357-114">Application</span></span> | <span data-ttu-id="4b357-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b357-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b357-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b357-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="4b357-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b357-117">Request headers</span></span>
| <span data-ttu-id="4b357-118">Name</span><span class="sxs-lookup"><span data-stu-id="4b357-118">Name</span></span>       | <span data-ttu-id="4b357-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b357-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b357-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b357-120">Authorization</span></span>  | <span data-ttu-id="4b357-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b357-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b357-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b357-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4b357-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b357-124">Response</span></span>

<span data-ttu-id="4b357-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b357-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b357-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b357-127">Example</span></span>
<span data-ttu-id="4b357-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4b357-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b357-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b357-129">Request</span></span>
<span data-ttu-id="4b357-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b357-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="4b357-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b357-131">Response</span></span>
<span data-ttu-id="4b357-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4b357-132">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/filter-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

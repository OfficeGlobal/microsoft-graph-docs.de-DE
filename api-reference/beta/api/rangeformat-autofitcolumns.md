---
title: 'RangeFormat: autofitColumns'
description: Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 3093bfc1dfb77d05c1ed270cfa625a12ac763888
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517946"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="89471-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="89471-103">RangeFormat: autofitColumns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89471-104">Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="89471-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="89471-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="89471-105">Permissions</span></span>
<span data-ttu-id="89471-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89471-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89471-108">Permission type</span></span>      | <span data-ttu-id="89471-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89471-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89471-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89471-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89471-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89471-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89471-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89471-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89471-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89471-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89471-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89471-114">Application</span></span> | <span data-ttu-id="89471-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89471-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89471-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89471-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="89471-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89471-117">Request headers</span></span>
| <span data-ttu-id="89471-118">Name</span><span class="sxs-lookup"><span data-stu-id="89471-118">Name</span></span>       | <span data-ttu-id="89471-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89471-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89471-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="89471-120">Authorization</span></span>  | <span data-ttu-id="89471-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="89471-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89471-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="89471-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="89471-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="89471-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89471-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89471-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="89471-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="89471-127">Response</span></span>

<span data-ttu-id="89471-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89471-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89471-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89471-130">Example</span></span>
<span data-ttu-id="89471-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="89471-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="89471-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89471-132">Request</span></span>
<span data-ttu-id="89471-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89471-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitColumns
```

##### <a name="response"></a><span data-ttu-id="89471-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="89471-134">Response</span></span>
<span data-ttu-id="89471-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="89471-135">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangeformat-autofitcolumns.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: 'Chart: delete'
description: Löscht das Diagrammobjekt.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3c2b0b051517e30e2a0275684124b26de0a355cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572122"
---
# <a name="chart-delete"></a><span data-ttu-id="fa833-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="fa833-103">Chart: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa833-104">Löscht das Diagrammobjekt.</span><span class="sxs-lookup"><span data-stu-id="fa833-104">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa833-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fa833-105">Permissions</span></span>
<span data-ttu-id="fa833-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa833-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa833-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa833-108">Permission type</span></span>      | <span data-ttu-id="fa833-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa833-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa833-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa833-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa833-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa833-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa833-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa833-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa833-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa833-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa833-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa833-114">Application</span></span> | <span data-ttu-id="fa833-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa833-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa833-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa833-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="fa833-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa833-117">Request headers</span></span>
| <span data-ttu-id="fa833-118">Name</span><span class="sxs-lookup"><span data-stu-id="fa833-118">Name</span></span>       | <span data-ttu-id="fa833-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa833-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa833-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa833-120">Authorization</span></span>  | <span data-ttu-id="fa833-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa833-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa833-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="fa833-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fa833-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="fa833-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa833-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa833-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fa833-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa833-127">Response</span></span>

<span data-ttu-id="fa833-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa833-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa833-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa833-130">Example</span></span>
<span data-ttu-id="fa833-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="fa833-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa833-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa833-132">Request</span></span>
<span data-ttu-id="fa833-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa833-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/delete
```

##### <a name="response"></a><span data-ttu-id="fa833-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa833-134">Response</span></span>
<span data-ttu-id="fa833-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa833-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

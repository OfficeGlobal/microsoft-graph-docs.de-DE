---
title: 'workbookPivotTable: Aktualisierung'
description: Aktualisiert die PivotTable.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3238f67fc7f017e64ab327619a4f4f90fba71d1f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970780"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="b249d-103">workbookPivotTable: Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="b249d-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="b249d-104">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="b249d-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="b249d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b249d-105">Permissions</span></span>
<span data-ttu-id="b249d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b249d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b249d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b249d-108">Permission type</span></span>      | <span data-ttu-id="b249d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b249d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b249d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b249d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b249d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b249d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b249d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b249d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b249d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b249d-113">Not supported.</span></span>    |
|<span data-ttu-id="b249d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b249d-114">Application</span></span> | <span data-ttu-id="b249d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b249d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b249d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b249d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="b249d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b249d-117">Request headers</span></span>
| <span data-ttu-id="b249d-118">Name</span><span class="sxs-lookup"><span data-stu-id="b249d-118">Name</span></span>       | <span data-ttu-id="b249d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b249d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b249d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b249d-120">Authorization</span></span>  | <span data-ttu-id="b249d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b249d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b249d-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b249d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b249d-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b249d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b249d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b249d-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="b249d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b249d-127">Response</span></span>
<span data-ttu-id="b249d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b249d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b249d-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b249d-130">Example</span></span>
<span data-ttu-id="b249d-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b249d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b249d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b249d-132">Request</span></span>
<span data-ttu-id="b249d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b249d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="b249d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b249d-134">Response</span></span>
<span data-ttu-id="b249d-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b249d-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

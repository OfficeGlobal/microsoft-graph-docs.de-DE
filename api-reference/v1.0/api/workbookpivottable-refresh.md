---
title: 'workbookPivotTable: Aktualisierung'
description: Aktualisiert die PivotTable.
ms.openlocfilehash: 3acbe6efb29d6846b48bfae250731640ad533dad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017167"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="72d63-103">workbookPivotTable: Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="72d63-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="72d63-104">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="72d63-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="72d63-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="72d63-105">Permissions</span></span>
<span data-ttu-id="72d63-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72d63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="72d63-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="72d63-108">Permission type</span></span>      | <span data-ttu-id="72d63-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="72d63-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72d63-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="72d63-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72d63-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72d63-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="72d63-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="72d63-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72d63-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72d63-113">Not supported.</span></span>    |
|<span data-ttu-id="72d63-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="72d63-114">Application</span></span> | <span data-ttu-id="72d63-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72d63-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72d63-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="72d63-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="72d63-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="72d63-117">Request headers</span></span>
| <span data-ttu-id="72d63-118">Name</span><span class="sxs-lookup"><span data-stu-id="72d63-118">Name</span></span>       | <span data-ttu-id="72d63-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72d63-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72d63-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="72d63-120">Authorization</span></span>  | <span data-ttu-id="72d63-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="72d63-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72d63-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="72d63-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="72d63-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="72d63-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72d63-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="72d63-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="72d63-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="72d63-127">Response</span></span>
<span data-ttu-id="72d63-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="72d63-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72d63-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="72d63-130">Example</span></span>
<span data-ttu-id="72d63-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="72d63-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="72d63-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="72d63-132">Request</span></span>
<span data-ttu-id="72d63-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="72d63-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="72d63-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="72d63-134">Response</span></span>
<span data-ttu-id="72d63-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="72d63-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
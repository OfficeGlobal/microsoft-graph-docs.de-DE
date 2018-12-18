---
title: 'workbookPivotTable: refreshAll'
description: Aktualisiert das PivotTable-Objekt in einem gegebenen Arbeitsblatt.
author: lumine2008
ms.openlocfilehash: dc94e5841440ba5110d7382abb04920e2d91015d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337912"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="e2fc1-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="e2fc1-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="e2fc1-104">Aktualisiert das PivotTable-Objekt in einem gegebenen Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="e2fc1-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2fc1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e2fc1-105">Permissions</span></span>
<span data-ttu-id="e2fc1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2fc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2fc1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2fc1-108">Permission type</span></span>      | <span data-ttu-id="e2fc1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2fc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2fc1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2fc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2fc1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2fc1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e2fc1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2fc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2fc1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2fc1-113">Not supported.</span></span>    |
|<span data-ttu-id="e2fc1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2fc1-114">Application</span></span> | <span data-ttu-id="e2fc1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2fc1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2fc1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2fc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="e2fc1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2fc1-117">Request headers</span></span>
| <span data-ttu-id="e2fc1-118">Name</span><span class="sxs-lookup"><span data-stu-id="e2fc1-118">Name</span></span>       | <span data-ttu-id="e2fc1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2fc1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2fc1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2fc1-120">Authorization</span></span>  | <span data-ttu-id="e2fc1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e2fc1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2fc1-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="e2fc1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e2fc1-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="e2fc1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2fc1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2fc1-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="e2fc1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2fc1-127">Response</span></span>
<span data-ttu-id="e2fc1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2fc1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2fc1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2fc1-130">Example</span></span>
<span data-ttu-id="e2fc1-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e2fc1-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e2fc1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2fc1-132">Request</span></span>
<span data-ttu-id="e2fc1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2fc1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="e2fc1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2fc1-134">Response</span></span>
<span data-ttu-id="e2fc1-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e2fc1-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

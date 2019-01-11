---
title: 'workbookPivotTable: refreshAll'
description: Aktualisiert das PivotTable-Objekt in einem gegebenen Arbeitsblatt.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: e6289de81da5869f1cd428ef426b49afa957c874
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823352"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="db7d0-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="db7d0-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="db7d0-104">Aktualisiert das PivotTable-Objekt in einem gegebenen Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="db7d0-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="db7d0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db7d0-105">Permissions</span></span>
<span data-ttu-id="db7d0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db7d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db7d0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db7d0-108">Permission type</span></span>      | <span data-ttu-id="db7d0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db7d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db7d0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db7d0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db7d0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db7d0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db7d0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db7d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db7d0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db7d0-113">Not supported.</span></span>    |
|<span data-ttu-id="db7d0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db7d0-114">Application</span></span> | <span data-ttu-id="db7d0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db7d0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db7d0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db7d0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="db7d0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db7d0-117">Request headers</span></span>
| <span data-ttu-id="db7d0-118">Name</span><span class="sxs-lookup"><span data-stu-id="db7d0-118">Name</span></span>       | <span data-ttu-id="db7d0-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db7d0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db7d0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="db7d0-120">Authorization</span></span>  | <span data-ttu-id="db7d0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="db7d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db7d0-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="db7d0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="db7d0-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="db7d0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db7d0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db7d0-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="db7d0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="db7d0-127">Response</span></span>
<span data-ttu-id="db7d0-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db7d0-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db7d0-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db7d0-130">Example</span></span>
<span data-ttu-id="db7d0-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="db7d0-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db7d0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db7d0-132">Request</span></span>
<span data-ttu-id="db7d0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db7d0-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="db7d0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="db7d0-134">Response</span></span>
<span data-ttu-id="db7d0-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="db7d0-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

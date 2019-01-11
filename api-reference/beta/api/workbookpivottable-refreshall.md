---
title: 'workbookPivotTable: refreshAll'
description: Aktualisiert das PivotTable-Objekt in einem gegebenen Arbeitsblatt.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: cd70ed9a0f0681ac8b1f90d2839e85a419762653
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822302"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="f5662-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="f5662-103">workbookPivotTable: refreshAll</span></span>

> <span data-ttu-id="f5662-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f5662-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5662-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f5662-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5662-106">Aktualisiert das PivotTable-Objekt in einem gegebenen Arbeitsblatt.</span><span class="sxs-lookup"><span data-stu-id="f5662-106">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5662-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5662-107">Permissions</span></span>
<span data-ttu-id="f5662-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5662-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5662-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5662-110">Permission type</span></span>      | <span data-ttu-id="f5662-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5662-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5662-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5662-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5662-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5662-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5662-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5662-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5662-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5662-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5662-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5662-116">Application</span></span> | <span data-ttu-id="f5662-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5662-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5662-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5662-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="f5662-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5662-119">Request headers</span></span>
| <span data-ttu-id="f5662-120">Name</span><span class="sxs-lookup"><span data-stu-id="f5662-120">Name</span></span>       | <span data-ttu-id="f5662-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5662-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5662-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5662-122">Authorization</span></span>  | <span data-ttu-id="f5662-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5662-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5662-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="f5662-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f5662-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="f5662-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5662-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5662-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f5662-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5662-129">Response</span></span>

<span data-ttu-id="f5662-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5662-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5662-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5662-132">Example</span></span>
<span data-ttu-id="f5662-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f5662-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5662-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5662-134">Request</span></span>
<span data-ttu-id="f5662-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5662-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="f5662-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5662-136">Response</span></span>
<span data-ttu-id="f5662-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5662-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

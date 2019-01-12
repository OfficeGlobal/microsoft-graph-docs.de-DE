---
title: 'workbookRange: columnsAfter'
description: Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c74a16a84f63d0b385126e2b4b2b9b43e3ffde6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987868"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="9bb8d-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="9bb8d-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="9bb8d-104">Ruft eine bestimmte Anzahl von Spalten rechts vom gegebenen Bereich ab.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bb8d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9bb8d-105">Permissions</span></span>
<span data-ttu-id="9bb8d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bb8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bb8d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9bb8d-108">Permission type</span></span>      | <span data-ttu-id="9bb8d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9bb8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bb8d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9bb8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9bb8d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bb8d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9bb8d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9bb8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bb8d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bb8d-113">Not supported.</span></span>    |
|<span data-ttu-id="9bb8d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9bb8d-114">Application</span></span> | <span data-ttu-id="9bb8d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bb8d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bb8d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bb8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="9bb8d-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="9bb8d-117">Function parameters</span></span>

| <span data-ttu-id="9bb8d-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="9bb8d-118">Parameter</span></span>    | <span data-ttu-id="9bb8d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9bb8d-119">Type</span></span>   |<span data-ttu-id="9bb8d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bb8d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bb8d-121">count</span><span class="sxs-lookup"><span data-stu-id="9bb8d-121">count</span></span>|<span data-ttu-id="9bb8d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9bb8d-122">Int32</span></span>|<span data-ttu-id="9bb8d-123">Optional.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-123">Optional.</span></span> <span data-ttu-id="9bb8d-124">Die Anzahl der Spalten im resultierenden Bereich eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-124">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="9bb8d-125">Verwenden Sie im Allgemeinen eine positive Zahl, um einen Bereich außerhalb des aktuellen Bereichs erstellen.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-125">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="9bb8d-126">Sie können auch eine negative Zahl verwenden, einen Bereich im aktuellen Bereich erstellt.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-126">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="9bb8d-127">Der Standardwert ist 1</span><span class="sxs-lookup"><span data-stu-id="9bb8d-127">The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9bb8d-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9bb8d-128">Request headers</span></span>
| <span data-ttu-id="9bb8d-129">Name</span><span class="sxs-lookup"><span data-stu-id="9bb8d-129">Name</span></span>       | <span data-ttu-id="9bb8d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bb8d-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9bb8d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bb8d-131">Authorization</span></span>  | <span data-ttu-id="9bb8d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9bb8d-134">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9bb8d-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="9bb8d-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bb8d-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9bb8d-137">Request body</span></span>
<span data-ttu-id="9bb8d-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bb8d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bb8d-139">Response</span></span>
<span data-ttu-id="9bb8d-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bb8d-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9bb8d-141">Example</span></span>
<span data-ttu-id="9bb8d-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9bb8d-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bb8d-143">Request</span></span>
<span data-ttu-id="9bb8d-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="9bb8d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bb8d-145">Response</span></span>
<span data-ttu-id="9bb8d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bb8d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

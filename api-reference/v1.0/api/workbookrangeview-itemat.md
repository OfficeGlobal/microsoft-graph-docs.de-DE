---
title: 'workbookRangeView: itemAt'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a8d0426c86b6e2a2bdadb50dfd3fb93c5495b1ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960525"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="072dc-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="072dc-104">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="072dc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="072dc-105">Permissions</span></span>
<span data-ttu-id="072dc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="072dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="072dc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="072dc-108">Permission type</span></span>      | <span data-ttu-id="072dc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="072dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="072dc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="072dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="072dc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="072dc-111">Files.ReadWrite</span></span> |
|<span data-ttu-id="072dc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="072dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="072dc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="072dc-113">Not supported.</span></span>    |
|<span data-ttu-id="072dc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="072dc-114">Application</span></span> | <span data-ttu-id="072dc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="072dc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="072dc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="072dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="072dc-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="072dc-117">Request headers</span></span>
| <span data-ttu-id="072dc-118">Name</span><span class="sxs-lookup"><span data-stu-id="072dc-118">Name</span></span>       | <span data-ttu-id="072dc-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="072dc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="072dc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="072dc-120">Authorization</span></span>  | <span data-ttu-id="072dc-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="072dc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="072dc-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="072dc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="072dc-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="072dc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="072dc-126">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="072dc-126">Function parameters</span></span>
<span data-ttu-id="072dc-127">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="072dc-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="072dc-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="072dc-128">Parameter</span></span>    | <span data-ttu-id="072dc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="072dc-129">Type</span></span>   |<span data-ttu-id="072dc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="072dc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="072dc-131">Index</span><span class="sxs-lookup"><span data-stu-id="072dc-131">index</span></span>|<span data-ttu-id="072dc-132">Int32</span><span class="sxs-lookup"><span data-stu-id="072dc-132">Int32</span></span>|<span data-ttu-id="072dc-133">Index des Elements, das zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="072dc-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="072dc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="072dc-134">Response</span></span>

<span data-ttu-id="072dc-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="072dc-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="072dc-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="072dc-136">Example</span></span>
<span data-ttu-id="072dc-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="072dc-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="072dc-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="072dc-138">Request</span></span>
<span data-ttu-id="072dc-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="072dc-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="072dc-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="072dc-140">Response</span></span>
<span data-ttu-id="072dc-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="072dc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```

---
title: 'workbookRangeView: itemAt'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 423c20f6cbdcbfe65a2f8db965a4765c93079f18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960581"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="953e4-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="953e4-104">workbookRangeView: itemAt</span></span>

> <span data-ttu-id="953e4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="953e4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="953e4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="953e4-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="953e4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="953e4-107">Permissions</span></span>
<span data-ttu-id="953e4-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="953e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="953e4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="953e4-110">Permission type</span></span>      | <span data-ttu-id="953e4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="953e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="953e4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="953e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="953e4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="953e4-113">Not supported.</span></span>    |
|<span data-ttu-id="953e4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="953e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="953e4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="953e4-115">Not supported.</span></span>    |
|<span data-ttu-id="953e4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="953e4-116">Application</span></span> | <span data-ttu-id="953e4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="953e4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="953e4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="953e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="953e4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="953e4-119">Request headers</span></span>
| <span data-ttu-id="953e4-120">Name</span><span class="sxs-lookup"><span data-stu-id="953e4-120">Name</span></span>       | <span data-ttu-id="953e4-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="953e4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="953e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="953e4-122">Authorization</span></span>  | <span data-ttu-id="953e4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="953e4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="953e4-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="953e4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="953e4-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="953e4-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="953e4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="953e4-128">Request body</span></span>
<span data-ttu-id="953e4-129">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="953e4-129">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="953e4-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="953e4-130">Parameter</span></span>    | <span data-ttu-id="953e4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="953e4-131">Type</span></span>   |<span data-ttu-id="953e4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="953e4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="953e4-133">Index</span><span class="sxs-lookup"><span data-stu-id="953e4-133">index</span></span>|<span data-ttu-id="953e4-134">Int32</span><span class="sxs-lookup"><span data-stu-id="953e4-134">Int32</span></span>|<span data-ttu-id="953e4-135">Index des Elements, das zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="953e4-135">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="953e4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="953e4-136">Response</span></span>

<span data-ttu-id="953e4-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="953e4-137">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="953e4-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="953e4-138">Example</span></span>
<span data-ttu-id="953e4-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="953e4-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="953e4-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="953e4-140">Request</span></span>
<span data-ttu-id="953e4-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="953e4-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="953e4-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="953e4-142">Response</span></span>
<span data-ttu-id="953e4-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="953e4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

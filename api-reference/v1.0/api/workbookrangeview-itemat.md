---
title: 'workbookRangeView: itemAt'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
ms.openlocfilehash: b6af086e9867ca4c4d61a4102de1d2800163c453
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016070"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="76835-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="76835-104">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="76835-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="76835-105">Permissions</span></span>
<span data-ttu-id="76835-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76835-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76835-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76835-108">Permission type</span></span>      | <span data-ttu-id="76835-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76835-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76835-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76835-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76835-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76835-111">Files.ReadWrite</span></span> |
|<span data-ttu-id="76835-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76835-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76835-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76835-113">Not supported.</span></span>    |
|<span data-ttu-id="76835-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76835-114">Application</span></span> | <span data-ttu-id="76835-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76835-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76835-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76835-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="76835-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76835-117">Request headers</span></span>
| <span data-ttu-id="76835-118">Name</span><span class="sxs-lookup"><span data-stu-id="76835-118">Name</span></span>       | <span data-ttu-id="76835-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76835-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="76835-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="76835-120">Authorization</span></span>  | <span data-ttu-id="76835-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="76835-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76835-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="76835-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="76835-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="76835-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="76835-126">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="76835-126">Function parameters</span></span>
<span data-ttu-id="76835-127">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="76835-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="76835-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="76835-128">Parameter</span></span>    | <span data-ttu-id="76835-129">Typ</span><span class="sxs-lookup"><span data-stu-id="76835-129">Type</span></span>   |<span data-ttu-id="76835-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76835-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76835-131">Index</span><span class="sxs-lookup"><span data-stu-id="76835-131">index</span></span>|<span data-ttu-id="76835-132">Int32</span><span class="sxs-lookup"><span data-stu-id="76835-132">Int32</span></span>|<span data-ttu-id="76835-133">Index des Elements, das zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="76835-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="76835-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="76835-134">Response</span></span>

<span data-ttu-id="76835-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76835-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76835-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76835-136">Example</span></span>
<span data-ttu-id="76835-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="76835-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76835-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76835-138">Request</span></span>
<span data-ttu-id="76835-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76835-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="76835-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="76835-140">Response</span></span>
<span data-ttu-id="76835-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76835-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
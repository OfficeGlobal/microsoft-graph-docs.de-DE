---
title: 'workbookRangeView: itemAt'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 85dcf4efd1cbbeae56b1f200ef53f48d19641369
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529901"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="5fc42-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="5fc42-104">workbookRangeView: itemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="5fc42-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5fc42-105">Permissions</span></span>
<span data-ttu-id="5fc42-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fc42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fc42-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5fc42-108">Permission type</span></span>      | <span data-ttu-id="5fc42-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5fc42-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fc42-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5fc42-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5fc42-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fc42-111">Not supported.</span></span>    |
|<span data-ttu-id="5fc42-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5fc42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fc42-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fc42-113">Not supported.</span></span>    |
|<span data-ttu-id="5fc42-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5fc42-114">Application</span></span> | <span data-ttu-id="5fc42-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fc42-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fc42-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fc42-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="5fc42-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5fc42-117">Request headers</span></span>
| <span data-ttu-id="5fc42-118">Name</span><span class="sxs-lookup"><span data-stu-id="5fc42-118">Name</span></span>       | <span data-ttu-id="5fc42-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fc42-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5fc42-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fc42-120">Authorization</span></span>  | <span data-ttu-id="5fc42-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5fc42-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5fc42-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5fc42-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5fc42-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5fc42-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fc42-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5fc42-126">Request body</span></span>
<span data-ttu-id="5fc42-127">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="5fc42-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="5fc42-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="5fc42-128">Parameter</span></span>    | <span data-ttu-id="5fc42-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5fc42-129">Type</span></span>   |<span data-ttu-id="5fc42-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fc42-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fc42-131">Index</span><span class="sxs-lookup"><span data-stu-id="5fc42-131">index</span></span>|<span data-ttu-id="5fc42-132">Int32</span><span class="sxs-lookup"><span data-stu-id="5fc42-132">Int32</span></span>|<span data-ttu-id="5fc42-133">Index des Elements, das zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="5fc42-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="5fc42-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fc42-134">Response</span></span>

<span data-ttu-id="5fc42-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fc42-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fc42-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5fc42-136">Example</span></span>
<span data-ttu-id="5fc42-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5fc42-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5fc42-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fc42-138">Request</span></span>
<span data-ttu-id="5fc42-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5fc42-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="5fc42-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fc42-140">Response</span></span>
<span data-ttu-id="5fc42-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fc42-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

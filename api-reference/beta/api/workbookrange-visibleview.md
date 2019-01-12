---
title: 'workbookRange: visibleView'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: eaa4fd44cc976281348f658eda7ecc358f19efc8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952909"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="2264d-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="2264d-104">workbookRange: visibleView</span></span>

> <span data-ttu-id="2264d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2264d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2264d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2264d-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="2264d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2264d-107">Permissions</span></span>
<span data-ttu-id="2264d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2264d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2264d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2264d-110">Permission type</span></span>      | <span data-ttu-id="2264d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2264d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2264d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2264d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2264d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2264d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2264d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2264d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2264d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2264d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2264d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2264d-116">Application</span></span> | <span data-ttu-id="2264d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2264d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2264d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2264d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="2264d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2264d-119">Request headers</span></span>
| <span data-ttu-id="2264d-120">Name</span><span class="sxs-lookup"><span data-stu-id="2264d-120">Name</span></span>       | <span data-ttu-id="2264d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2264d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2264d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2264d-122">Authorization</span></span>  | <span data-ttu-id="2264d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2264d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2264d-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2264d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2264d-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2264d-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2264d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2264d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2264d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2264d-129">Response</span></span>

<span data-ttu-id="2264d-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2264d-130">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2264d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2264d-131">Example</span></span>
<span data-ttu-id="2264d-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2264d-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2264d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2264d-133">Request</span></span>
<span data-ttu-id="2264d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2264d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="2264d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2264d-135">Response</span></span>
<span data-ttu-id="2264d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2264d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

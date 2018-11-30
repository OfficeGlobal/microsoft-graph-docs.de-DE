---
title: 'workbookRange: visibleView'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
ms.openlocfilehash: 18b8e4567eb40dd8861b94b72bfeb3cad9aa004f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016145"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="d2bbb-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="d2bbb-104">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="d2bbb-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d2bbb-105">Permissions</span></span>
<span data-ttu-id="d2bbb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2bbb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2bbb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2bbb-108">Permission type</span></span>      | <span data-ttu-id="d2bbb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2bbb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2bbb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2bbb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2bbb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2bbb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2bbb-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2bbb-113">Not supported.</span></span>    |
|<span data-ttu-id="d2bbb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2bbb-114">Application</span></span> | <span data-ttu-id="d2bbb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2bbb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2bbb-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2bbb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="d2bbb-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2bbb-117">Request headers</span></span>
| <span data-ttu-id="d2bbb-118">Name</span><span class="sxs-lookup"><span data-stu-id="d2bbb-118">Name</span></span>       | <span data-ttu-id="d2bbb-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2bbb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d2bbb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2bbb-120">Authorization</span></span>  | <span data-ttu-id="d2bbb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2bbb-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="d2bbb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2bbb-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2bbb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2bbb-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="d2bbb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2bbb-127">Response</span></span>
<span data-ttu-id="d2bbb-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2bbb-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2bbb-129">Example</span></span>
<span data-ttu-id="d2bbb-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2bbb-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2bbb-131">Request</span></span>
<span data-ttu-id="d2bbb-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="d2bbb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2bbb-133">Response</span></span>
<span data-ttu-id="d2bbb-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2bbb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
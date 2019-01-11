---
title: 'workbookRange: visibleView'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
localization_priority: Normal
ms.openlocfilehash: f994866c8f55ec2ffbc0b680d4576fbc6a8b7bb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875166"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="c0c2e-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="c0c2e-104">workbookRange: visibleView</span></span>

> <span data-ttu-id="c0c2e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0c2e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0c2e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c0c2e-107">Permissions</span></span>
<span data-ttu-id="c0c2e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c2e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c2e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0c2e-110">Permission type</span></span>      | <span data-ttu-id="c0c2e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0c2e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0c2e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0c2e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c0c2e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0c2e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0c2e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0c2e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c2e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0c2e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c0c2e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0c2e-116">Application</span></span> | <span data-ttu-id="c0c2e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0c2e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0c2e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0c2e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="c0c2e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0c2e-119">Request headers</span></span>
| <span data-ttu-id="c0c2e-120">Name</span><span class="sxs-lookup"><span data-stu-id="c0c2e-120">Name</span></span>       | <span data-ttu-id="c0c2e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0c2e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c0c2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0c2e-122">Authorization</span></span>  | <span data-ttu-id="c0c2e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0c2e-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c0c2e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c0c2e-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c2e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0c2e-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c0c2e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0c2e-129">Response</span></span>

<span data-ttu-id="c0c2e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-130">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c2e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0c2e-131">Example</span></span>
<span data-ttu-id="c0c2e-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c0c2e-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0c2e-133">Request</span></span>
<span data-ttu-id="c0c2e-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="c0c2e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0c2e-135">Response</span></span>
<span data-ttu-id="c0c2e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

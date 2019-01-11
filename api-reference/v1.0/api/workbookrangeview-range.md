---
title: 'workbookRangeView: Bereich'
description: Geben Sie den Bereich zurück, der der rangeView-Ressource zugeordnet ist.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4e707bb4a1ff31526f6a2aafcb569c7dd8328279
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808736"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="0ee4b-103">workbookRangeView: Bereich</span><span class="sxs-lookup"><span data-stu-id="0ee4b-103">workbookRangeView: range</span></span>
<span data-ttu-id="0ee4b-104">Geben Sie den Bereich zurück, der der rangeView-Ressource zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="0ee4b-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ee4b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0ee4b-105">Permissions</span></span>
<span data-ttu-id="0ee4b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0ee4b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ee4b-108">Permission type</span></span>      | <span data-ttu-id="0ee4b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ee4b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ee4b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ee4b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ee4b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ee4b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ee4b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ee4b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ee4b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ee4b-113">Not supported.</span></span>    |
|<span data-ttu-id="0ee4b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ee4b-114">Application</span></span> | <span data-ttu-id="0ee4b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ee4b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ee4b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ee4b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="0ee4b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ee4b-117">Request headers</span></span>
| <span data-ttu-id="0ee4b-118">Name</span><span class="sxs-lookup"><span data-stu-id="0ee4b-118">Name</span></span>       | <span data-ttu-id="0ee4b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ee4b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ee4b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ee4b-120">Authorization</span></span>  | <span data-ttu-id="0ee4b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0ee4b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ee4b-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="0ee4b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ee4b-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="0ee4b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee4b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ee4b-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="0ee4b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ee4b-127">Response</span></span>
<span data-ttu-id="0ee4b-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ee4b-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee4b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ee4b-129">Example</span></span>
<span data-ttu-id="0ee4b-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0ee4b-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0ee4b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ee4b-131">Request</span></span>
<span data-ttu-id="0ee4b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ee4b-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="0ee4b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ee4b-133">Response</span></span>
<span data-ttu-id="0ee4b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ee4b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

---
title: 'workbookRangeView: Bereich'
description: Geben Sie den Bereich zurück, der der rangeView-Ressource zugeordnet ist.
ms.openlocfilehash: 7210501eaad8b99eb57f002292fcbef6a2f4c73c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065887"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="2ce04-103">workbookRangeView: Bereich</span><span class="sxs-lookup"><span data-stu-id="2ce04-103">workbookRangeView: range</span></span>

> <span data-ttu-id="2ce04-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2ce04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ce04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ce04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ce04-106">Geben Sie den Bereich zurück, der der rangeView-Ressource zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="2ce04-106">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ce04-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2ce04-107">Permissions</span></span>
<span data-ttu-id="2ce04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ce04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2ce04-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ce04-110">Permission type</span></span>      | <span data-ttu-id="2ce04-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ce04-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ce04-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ce04-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ce04-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ce04-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ce04-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ce04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ce04-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ce04-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ce04-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ce04-116">Application</span></span> | <span data-ttu-id="2ce04-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ce04-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ce04-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ce04-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="2ce04-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ce04-119">Request headers</span></span>
| <span data-ttu-id="2ce04-120">Name</span><span class="sxs-lookup"><span data-stu-id="2ce04-120">Name</span></span>       | <span data-ttu-id="2ce04-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ce04-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ce04-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce04-122">Authorization</span></span>  | <span data-ttu-id="2ce04-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2ce04-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ce04-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2ce04-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ce04-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2ce04-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ce04-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ce04-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2ce04-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ce04-129">Response</span></span>

<span data-ttu-id="2ce04-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ce04-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ce04-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ce04-131">Example</span></span>
<span data-ttu-id="2ce04-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2ce04-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ce04-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ce04-133">Request</span></span>
<span data-ttu-id="2ce04-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2ce04-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="2ce04-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ce04-135">Response</span></span>
<span data-ttu-id="2ce04-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ce04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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

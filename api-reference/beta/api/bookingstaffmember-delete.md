---
title: BookingStaffMember löschen
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7aa2fd114a4d53b462dcd0b66e75808e52ef9ada
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946875"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="e8dc2-104">BookingStaffMember löschen</span><span class="sxs-lookup"><span data-stu-id="e8dc2-104">Delete bookingStaffMember</span></span>

 > <span data-ttu-id="e8dc2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e8dc2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8dc2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8dc2-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e8dc2-107">Löschen Sie einen [Mitarbeiter](../resources/bookingstaffmember.md) in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="e8dc2-107">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e8dc2-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e8dc2-108">Permissions</span></span>
<span data-ttu-id="e8dc2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8dc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8dc2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8dc2-111">Permission type</span></span>      | <span data-ttu-id="e8dc2-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8dc2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8dc2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8dc2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e8dc2-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e8dc2-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e8dc2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8dc2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8dc2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8dc2-116">Not supported.</span></span>   |
|<span data-ttu-id="e8dc2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8dc2-117">Application</span></span> | <span data-ttu-id="e8dc2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8dc2-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e8dc2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8dc2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e8dc2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8dc2-120">Request headers</span></span>
| <span data-ttu-id="e8dc2-121">Name</span><span class="sxs-lookup"><span data-stu-id="e8dc2-121">Name</span></span>       | <span data-ttu-id="e8dc2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8dc2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8dc2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8dc2-123">Authorization</span></span>  | <span data-ttu-id="e8dc2-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e8dc2-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8dc2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8dc2-125">Request body</span></span>
<span data-ttu-id="e8dc2-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e8dc2-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e8dc2-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8dc2-127">Response</span></span>
<span data-ttu-id="e8dc2-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8dc2-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8dc2-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8dc2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8dc2-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8dc2-131">Request</span></span>
<span data-ttu-id="e8dc2-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8dc2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
##### <a name="response"></a><span data-ttu-id="e8dc2-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8dc2-133">Response</span></span>
<span data-ttu-id="e8dc2-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e8dc2-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

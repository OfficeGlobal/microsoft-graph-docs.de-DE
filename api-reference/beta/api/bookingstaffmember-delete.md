---
title: BookingStaffMember löschen
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: cca8d7794922244e1e6eab0f43bf0ac95c752897
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058709"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="68add-104">BookingStaffMember löschen</span><span class="sxs-lookup"><span data-stu-id="68add-104">Delete bookingStaffMember</span></span>

 > <span data-ttu-id="68add-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="68add-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68add-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68add-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="68add-107">Löschen Sie einen [Mitarbeiter](../resources/bookingstaffmember.md) in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="68add-107">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="68add-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="68add-108">Permissions</span></span>
<span data-ttu-id="68add-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68add-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68add-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68add-111">Permission type</span></span>      | <span data-ttu-id="68add-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68add-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68add-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68add-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="68add-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="68add-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="68add-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68add-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68add-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68add-116">Not supported.</span></span>   |
|<span data-ttu-id="68add-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68add-117">Application</span></span> | <span data-ttu-id="68add-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68add-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="68add-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68add-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="68add-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68add-120">Request headers</span></span>
| <span data-ttu-id="68add-121">Name</span><span class="sxs-lookup"><span data-stu-id="68add-121">Name</span></span>       | <span data-ttu-id="68add-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68add-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="68add-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68add-123">Authorization</span></span>  | <span data-ttu-id="68add-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="68add-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="68add-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68add-125">Request body</span></span>
<span data-ttu-id="68add-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="68add-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="68add-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="68add-127">Response</span></span>
<span data-ttu-id="68add-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68add-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68add-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68add-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68add-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68add-131">Request</span></span>
<span data-ttu-id="68add-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68add-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
##### <a name="response"></a><span data-ttu-id="68add-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="68add-133">Response</span></span>
<span data-ttu-id="68add-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68add-134">The following is an example of the response.</span></span> 
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
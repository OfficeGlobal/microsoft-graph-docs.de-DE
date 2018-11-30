---
title: BookingCustomer löschen
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: c4ba9267e2a3fde3ac43460160ffd4bb37cfb56d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060021"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="df674-104">BookingCustomer löschen</span><span class="sxs-lookup"><span data-stu-id="df674-104">Delete bookingCustomer</span></span>

 > <span data-ttu-id="df674-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df674-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df674-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df674-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="df674-107">Das angegebene [BookingCustomer](../resources/bookingcustomer.md) -Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="df674-107">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="df674-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="df674-108">Permissions</span></span>
<span data-ttu-id="df674-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df674-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df674-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df674-111">Permission type</span></span>      | <span data-ttu-id="df674-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df674-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df674-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df674-113">Delegated (work or school account)</span></span> | <span data-ttu-id="df674-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="df674-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="df674-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df674-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df674-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df674-116">Not supported.</span></span>   |
|<span data-ttu-id="df674-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df674-117">Application</span></span> | <span data-ttu-id="df674-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df674-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="df674-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df674-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="df674-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df674-120">Request headers</span></span>
| <span data-ttu-id="df674-121">Name</span><span class="sxs-lookup"><span data-stu-id="df674-121">Name</span></span>       | <span data-ttu-id="df674-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df674-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df674-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df674-123">Authorization</span></span>  | <span data-ttu-id="df674-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="df674-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="df674-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df674-125">Request body</span></span>
<span data-ttu-id="df674-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="df674-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="df674-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="df674-127">Response</span></span>
<span data-ttu-id="df674-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df674-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df674-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df674-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df674-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df674-131">Request</span></span>
<span data-ttu-id="df674-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df674-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="df674-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="df674-133">Response</span></span>
<span data-ttu-id="df674-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="df674-134">The following is an example of the response.</span></span> <span data-ttu-id="df674-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="df674-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="df674-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df674-136">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
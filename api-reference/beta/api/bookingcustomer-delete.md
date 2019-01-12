---
title: BookingCustomer löschen
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1e2c303733b850d45b8c805f40fc42bc835cc313
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941548"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="26898-104">BookingCustomer löschen</span><span class="sxs-lookup"><span data-stu-id="26898-104">Delete bookingCustomer</span></span>

 > <span data-ttu-id="26898-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="26898-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26898-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26898-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="26898-107">Das angegebene [BookingCustomer](../resources/bookingcustomer.md) -Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="26898-107">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="26898-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="26898-108">Permissions</span></span>
<span data-ttu-id="26898-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26898-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26898-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26898-111">Permission type</span></span>      | <span data-ttu-id="26898-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26898-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26898-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26898-113">Delegated (work or school account)</span></span> | <span data-ttu-id="26898-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="26898-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="26898-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26898-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26898-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26898-116">Not supported.</span></span>   |
|<span data-ttu-id="26898-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26898-117">Application</span></span> | <span data-ttu-id="26898-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26898-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="26898-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26898-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="26898-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26898-120">Request headers</span></span>
| <span data-ttu-id="26898-121">Name</span><span class="sxs-lookup"><span data-stu-id="26898-121">Name</span></span>       | <span data-ttu-id="26898-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26898-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="26898-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26898-123">Authorization</span></span>  | <span data-ttu-id="26898-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="26898-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="26898-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26898-125">Request body</span></span>
<span data-ttu-id="26898-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="26898-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="26898-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="26898-127">Response</span></span>
<span data-ttu-id="26898-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26898-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26898-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26898-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26898-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26898-131">Request</span></span>
<span data-ttu-id="26898-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26898-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="26898-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="26898-133">Response</span></span>
<span data-ttu-id="26898-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="26898-134">The following is an example of the response.</span></span> <span data-ttu-id="26898-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="26898-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="26898-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26898-136">All of the properties will be returned from an actual call.</span></span>
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

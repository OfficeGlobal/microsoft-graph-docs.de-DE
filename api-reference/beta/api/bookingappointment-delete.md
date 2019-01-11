---
title: BookingAppointment löschen
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: a93f270326c1f1d3bcebcbd82ffdc0f29a3ed907
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809443"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="3eba5-104">BookingAppointment löschen</span><span class="sxs-lookup"><span data-stu-id="3eba5-104">Delete bookingAppointment</span></span>

 > <span data-ttu-id="3eba5-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3eba5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eba5-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3eba5-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="3eba5-107">Löschen einer [BookingAppointment](../resources/bookingappointment.md) in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3eba5-107">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3eba5-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3eba5-108">Permissions</span></span>
<span data-ttu-id="3eba5-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eba5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eba5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3eba5-111">Permission type</span></span>      | <span data-ttu-id="3eba5-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3eba5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eba5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3eba5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="3eba5-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3eba5-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3eba5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3eba5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eba5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3eba5-116">Not supported.</span></span>   |
|<span data-ttu-id="3eba5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3eba5-117">Application</span></span> | <span data-ttu-id="3eba5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3eba5-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3eba5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3eba5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3eba5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3eba5-120">Request headers</span></span>
| <span data-ttu-id="3eba5-121">Name</span><span class="sxs-lookup"><span data-stu-id="3eba5-121">Name</span></span>       | <span data-ttu-id="3eba5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3eba5-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3eba5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eba5-123">Authorization</span></span>  | <span data-ttu-id="3eba5-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3eba5-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eba5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3eba5-125">Request body</span></span>
<span data-ttu-id="3eba5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3eba5-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3eba5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="3eba5-127">Response</span></span>
<span data-ttu-id="3eba5-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3eba5-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eba5-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3eba5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3eba5-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3eba5-131">Request</span></span>
<span data-ttu-id="3eba5-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3eba5-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="3eba5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3eba5-133">Response</span></span>
<span data-ttu-id="3eba5-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3eba5-134">The following is an example of the response.</span></span> <span data-ttu-id="3eba5-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3eba5-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3eba5-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3eba5-136">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

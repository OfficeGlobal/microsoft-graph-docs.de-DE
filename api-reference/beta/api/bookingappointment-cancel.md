---
title: 'BookingAppointment: Abbrechen'
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 4cd7b511f997f32c134f70a976cd94c2ed910fb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058090"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="2f72e-104">BookingAppointment: Abbrechen</span><span class="sxs-lookup"><span data-stu-id="2f72e-104">bookingAppointment: cancel</span></span>

 > <span data-ttu-id="2f72e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2f72e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f72e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f72e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="2f72e-107">Die angegebene [BookingAppointment](../resources/bookingappointment.md) in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md)Abbrechen, und Senden einer Nachricht an die beteiligten Kunden und Mitarbeiter.</span><span class="sxs-lookup"><span data-stu-id="2f72e-107">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f72e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2f72e-108">Permissions</span></span>
<span data-ttu-id="2f72e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f72e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f72e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f72e-111">Permission type</span></span>      | <span data-ttu-id="2f72e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f72e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f72e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f72e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f72e-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="2f72e-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2f72e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f72e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f72e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f72e-116">Not supported.</span></span>   |
|<span data-ttu-id="2f72e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f72e-117">Application</span></span> | <span data-ttu-id="2f72e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f72e-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="2f72e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f72e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="2f72e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f72e-120">Request headers</span></span>
| <span data-ttu-id="2f72e-121">Name</span><span class="sxs-lookup"><span data-stu-id="2f72e-121">Name</span></span>       | <span data-ttu-id="2f72e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f72e-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f72e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f72e-123">Authorization</span></span>  | <span data-ttu-id="2f72e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2f72e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f72e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f72e-125">Request body</span></span>
<span data-ttu-id="2f72e-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2f72e-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f72e-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="2f72e-127">Parameter</span></span>    | <span data-ttu-id="2f72e-128">Typ</span><span class="sxs-lookup"><span data-stu-id="2f72e-128">Type</span></span>   |<span data-ttu-id="2f72e-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f72e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f72e-130">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="2f72e-130">cancellationMessage</span></span>|<span data-ttu-id="2f72e-131">String</span><span class="sxs-lookup"><span data-stu-id="2f72e-131">String</span></span>|<span data-ttu-id="2f72e-132">Eine Meldung mit dem Kunden zu bestätigen, dass der Termin abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="2f72e-132">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="2f72e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f72e-133">Response</span></span>
<span data-ttu-id="2f72e-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f72e-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="2f72e-136">Wenn Sie versuchen, einen Termin abzubrechen, das nicht vorhanden ist, gibt diese Methode `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="2f72e-136">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="2f72e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f72e-137">Example</span></span>
<span data-ttu-id="2f72e-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2f72e-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f72e-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f72e-139">Request</span></span>
<span data-ttu-id="2f72e-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f72e-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingappointment_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```

##### <a name="response"></a><span data-ttu-id="2f72e-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f72e-141">Response</span></span>
<span data-ttu-id="2f72e-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f72e-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
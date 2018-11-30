---
title: Abrufen von bookingAppointment
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: c3dedab3cbd5fc3848e222317d27527b19671b06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060029"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="794bd-104">Abrufen von bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="794bd-104">Get bookingAppointment</span></span>

 > <span data-ttu-id="794bd-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="794bd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="794bd-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="794bd-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="794bd-107">Rufen Sie die Eigenschaften und die Beziehungen eines [BookingAppointment](../resources/bookingappointment.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="794bd-107">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="794bd-108">Die Eigenschaften **start** und **End** sind immer in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="794bd-108">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="794bd-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="794bd-109">Permissions</span></span>
<span data-ttu-id="794bd-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="794bd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="794bd-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="794bd-112">Permission type</span></span>      | <span data-ttu-id="794bd-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="794bd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="794bd-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="794bd-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="794bd-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="794bd-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="794bd-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="794bd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="794bd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="794bd-117">Not supported.</span></span>   |
|<span data-ttu-id="794bd-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="794bd-118">Application</span></span> | <span data-ttu-id="794bd-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="794bd-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="794bd-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="794bd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="794bd-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="794bd-121">Optional query parameters</span></span>
<span data-ttu-id="794bd-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="794bd-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="794bd-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="794bd-123">Request headers</span></span>
| <span data-ttu-id="794bd-124">Name</span><span class="sxs-lookup"><span data-stu-id="794bd-124">Name</span></span>      |<span data-ttu-id="794bd-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="794bd-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="794bd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="794bd-126">Authorization</span></span>  | <span data-ttu-id="794bd-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="794bd-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="794bd-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="794bd-128">Request body</span></span>
<span data-ttu-id="794bd-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="794bd-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="794bd-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="794bd-130">Response</span></span>
<span data-ttu-id="794bd-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [BookingAppointment](../resources/bookingappointment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="794bd-131">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="794bd-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="794bd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="794bd-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="794bd-133">Request</span></span>
<span data-ttu-id="794bd-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="794bd-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="794bd-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="794bd-135">Response</span></span>
<span data-ttu-id="794bd-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="794bd-136">The following is an example of the response.</span></span> <span data-ttu-id="794bd-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="794bd-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="794bd-138">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="794bd-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADKnAAA=",
    "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
    "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
    "customerName": "Jordan Miller",
    "customerEmailAddress": "jordanm@contoso.com",
    "customerPhone": "213-555-0199",
    "customerNotes": null,
    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceName": "Catered bento",
    "duration": "PT30M",
    "preBuffer": "PT5M",
    "postBuffer": "PT10M",
    "priceType": "fixedPrice",
    "price": 10,
    "serviceNotes": "Customer requires punctual service.",
    "optOutOfCustomerEmail": false,
    "staffMemberIds": [],
    "invoiceAmount": 10,
    "invoiceId": "1001",
    "invoiceStatus": "open",
    "invoiceUrl": "theInvoiceUrl",
    "customerLocation": {
        "displayName": "Customer",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "start": {
        "dateTime": "2018-05-06T12:00:00.0000000Z",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2018-05-06T12:30:00.0000000Z",
        "timeZone": "UTC"
    },
    "serviceLocation": {
        "displayName": "Customer location (123 First Avenue, Buffalo, NY 98052, USA)",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "reminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "This service is tomorrow"
        },
        {
            "offset": "PT1H",
            "recipients": "customer",
            "message": "Please be available to enjoy your lunch service."
        },
        {
            "offset": "PT2H",
            "recipients": "staff",
            "message": "Please check traffic for next cater."
        }
    ],
    "invoiceDate": {
        "dateTime": "2018-05-06T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
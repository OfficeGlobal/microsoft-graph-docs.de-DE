---
title: Erstellen von bookingAppointment
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: df8d1ab3d4eeb93de37e51085935b121609dd023
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855076"
---
# <a name="create-bookingappointment"></a><span data-ttu-id="ec66a-104">Erstellen von bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="ec66a-104">Create bookingAppointment</span></span>

 > <span data-ttu-id="ec66a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec66a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec66a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec66a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="ec66a-107">Erstellen Sie eine neue [BookingAppointment](../resources/bookingappointment.md) für die angegebene [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="ec66a-107">Create a new [bookingAppointment](../resources/bookingappointment.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ec66a-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ec66a-108">Permissions</span></span>
<span data-ttu-id="ec66a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec66a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec66a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec66a-111">Permission type</span></span>      | <span data-ttu-id="ec66a-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec66a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec66a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec66a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="ec66a-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ec66a-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ec66a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec66a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec66a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec66a-116">Not supported.</span></span>   |
|<span data-ttu-id="ec66a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec66a-117">Application</span></span> | <span data-ttu-id="ec66a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec66a-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="ec66a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec66a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments

```
## <a name="request-headers"></a><span data-ttu-id="ec66a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec66a-120">Request headers</span></span>
| <span data-ttu-id="ec66a-121">Name</span><span class="sxs-lookup"><span data-stu-id="ec66a-121">Name</span></span>       | <span data-ttu-id="ec66a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec66a-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ec66a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec66a-123">Authorization</span></span>  | <span data-ttu-id="ec66a-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ec66a-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec66a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec66a-125">Request body</span></span>
<span data-ttu-id="ec66a-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingAppointment](../resources/bookingappointment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ec66a-126">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ec66a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec66a-127">Response</span></span>
<span data-ttu-id="ec66a-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201, Created` Antwortobjekt Code und [BookingAppointment](../resources/bookingappointment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ec66a-128">If successful, this method returns `201, Created` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec66a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec66a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec66a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec66a-130">Request</span></span>
<span data-ttu-id="ec66a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec66a-131">The following is an example of the request.</span></span> <span data-ttu-id="ec66a-132">Dieser Termin muss keine bestimmte Mitarbeiter buchen werden.</span><span class="sxs-lookup"><span data-stu-id="ec66a-132">This appointment does not involve booking specific staff members.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingappointment_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "customerEmailAddress":"jordanm@contoso.com",
    "customerLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "customerName":"Jordan Miller",
    "customerNotes":"Please be on time.",
    "customerPhone":"213-555-0199",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceAmount":10.0,
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceId":"1001",
    "invoiceStatus@odata.type":"#microsoft.graph.bookingInvoiceStatus",
    "invoiceStatus":"open",
    "invoiceUrl":"theInvoiceUrl",
    "optOutOfCustomerEmail":false,
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "price":10.0,
    "priceType@odata.type":"#microsoft.graph.bookingPriceType",
    "priceType":"fixedPrice",
    "reminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "reminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"This service is tomorrow",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be available to enjoy your lunch service.",
            "offset":"PT1H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"customer"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please check traffic for next cater.",
            "offset":"PT2H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"staff"
        }
    ],
    "serviceId":"57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer location",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "serviceName":"Catered bento",
    "serviceNotes":"Customer requires punctual service.",
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
<span data-ttu-id="ec66a-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingAppointment](../resources/bookingappointment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ec66a-133">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ec66a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec66a-134">Response</span></span>
<span data-ttu-id="ec66a-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ec66a-135">The following is an example of the response.</span></span> <span data-ttu-id="ec66a-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ec66a-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ec66a-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec66a-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADc7zF4J0AAA8v_KnAAA=",
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
        "dateTime": "2018-05-01T12:00:00.0000000Z",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2018-05-01T12:30:00.0000000Z",
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
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

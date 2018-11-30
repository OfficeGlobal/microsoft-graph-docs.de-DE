---
title: Liste Termine
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 5e0846a1671a7a566e5175a331dc7c03e02af537
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059678"
---
# <a name="list-appointments"></a><span data-ttu-id="bdd8a-104">Liste Termine</span><span class="sxs-lookup"><span data-stu-id="bdd8a-104">List appointments</span></span>

 > <span data-ttu-id="bdd8a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bdd8a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdd8a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bdd8a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bdd8a-107">Rufen Sie eine Liste von [BookingAppointment](../resources/bookingappointment.md) -Objekten für den angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="bdd8a-107">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bdd8a-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bdd8a-108">Permissions</span></span>
<span data-ttu-id="bdd8a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd8a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd8a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bdd8a-111">Permission type</span></span>      | <span data-ttu-id="bdd8a-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bdd8a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd8a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bdd8a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="bdd8a-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="bdd8a-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bdd8a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bdd8a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd8a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdd8a-116">Not supported.</span></span>   |
|<span data-ttu-id="bdd8a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bdd8a-117">Application</span></span> | <span data-ttu-id="bdd8a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdd8a-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="bdd8a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdd8a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bdd8a-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bdd8a-120">Optional query parameters</span></span>
<span data-ttu-id="bdd8a-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bdd8a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="bdd8a-122">Zum Abrufen der Reihe von Terminen eines Unternehmens Buchungen innerhalb eines Datumsbereichs anstelle von `$filter`, für diesen Datumsbereich [das CalendarView erhalten möchten](bookingbusiness-list-calendarview.md) .</span><span class="sxs-lookup"><span data-stu-id="bdd8a-122">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="bdd8a-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bdd8a-123">Request headers</span></span>
| <span data-ttu-id="bdd8a-124">Name</span><span class="sxs-lookup"><span data-stu-id="bdd8a-124">Name</span></span>      |<span data-ttu-id="bdd8a-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdd8a-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bdd8a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdd8a-126">Authorization</span></span>  | <span data-ttu-id="bdd8a-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bdd8a-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdd8a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bdd8a-128">Request body</span></span>
<span data-ttu-id="bdd8a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bdd8a-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bdd8a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdd8a-130">Response</span></span>
<span data-ttu-id="bdd8a-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingAppointment](../resources/bookingappointment.md) .</span><span class="sxs-lookup"><span data-stu-id="bdd8a-131">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bdd8a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bdd8a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdd8a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdd8a-133">Request</span></span>
<span data-ttu-id="bdd8a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bdd8a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
##### <a name="response"></a><span data-ttu-id="bdd8a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdd8a-135">Response</span></span>
<span data-ttu-id="bdd8a-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bdd8a-136">The following is an example of the response.</span></span> <span data-ttu-id="bdd8a-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="bdd8a-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bdd8a-138">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bdd8a-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments",
    "value": [
        {
            "id": "AAMkADKoAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "customerName": "Bob Kelly",
            "customerEmailAddress": "bobk@tailspintoys.com",
            "customerPhone": "213-555-0108",
            "customerNotes": null,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
            "optOutOfCustomerEmail": false,
            "staffMemberIds": [],
            "invoiceAmount": 10,
            "invoiceId": "1002",
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
                "dateTime": "2018-04-30T13:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-04-30T13:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (987 Third Avenue, Buffalo, NY 98052, USA)",
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-04-30T13:30:00.0000000Z",
                "timeZone": "UTC"
            }
        },
        {
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
            "serviceNotes": null,
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-01T12:30:00.0000000Z",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
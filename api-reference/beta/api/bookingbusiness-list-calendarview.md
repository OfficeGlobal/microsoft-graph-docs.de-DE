---
title: Liste Buchungen calendarView
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 96da0d02d58f9ea4a3503e08c0733f4394dbbd6a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956941"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="b9a7d-104">Liste Buchungen calendarView</span><span class="sxs-lookup"><span data-stu-id="b9a7d-104">List Bookings calendarView</span></span>

 > <span data-ttu-id="b9a7d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9a7d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b9a7d-107">Rufen Sie die Auflistung von [BookingAppointment](../resources/bookingappointment.md) -Objekten für ein [BookingBusiness](../resources/bookingbusiness.md), die in der angegebene Datumsbereich auftritt.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-107">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9a7d-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9a7d-108">Permissions</span></span>
<span data-ttu-id="b9a7d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a7d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a7d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9a7d-111">Permission type</span></span>      | <span data-ttu-id="b9a7d-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9a7d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9a7d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9a7d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9a7d-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b9a7d-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b9a7d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9a7d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a7d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9a7d-116">Not supported.</span></span>   |
|<span data-ttu-id="b9a7d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9a7d-117">Application</span></span> | <span data-ttu-id="b9a7d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9a7d-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="b9a7d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9a7d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="b9a7d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9a7d-120">Request headers</span></span>
| <span data-ttu-id="b9a7d-121">Name</span><span class="sxs-lookup"><span data-stu-id="b9a7d-121">Name</span></span>       | <span data-ttu-id="b9a7d-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9a7d-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9a7d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9a7d-123">Authorization</span></span>  | <span data-ttu-id="b9a7d-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b9a7d-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9a7d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9a7d-125">Request body</span></span>
<span data-ttu-id="b9a7d-126">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-126">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="b9a7d-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="b9a7d-127">Parameter</span></span>    | <span data-ttu-id="b9a7d-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b9a7d-128">Type</span></span>   |<span data-ttu-id="b9a7d-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9a7d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9a7d-130">start</span><span class="sxs-lookup"><span data-stu-id="b9a7d-130">start</span></span>|<span data-ttu-id="b9a7d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9a7d-131">DateTimeOffset</span></span>|<span data-ttu-id="b9a7d-132">Das Startdatum und die Uhrzeit der ein Zeitbereich dargestellt im ISO 8601-Format als UTC oder UTC-Offset.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-132">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="b9a7d-133">Uhr UTC auf 1 Jan 2018 könnte beispielsweise wie folgt aussehen: ' 2018-01-01T00:00:00Z ", und gleichzeitig in PST-Datei würde wie folgt aussehen: ' 2017-12-31T16:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="b9a7d-133">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="b9a7d-134">end</span><span class="sxs-lookup"><span data-stu-id="b9a7d-134">end</span></span>|<span data-ttu-id="b9a7d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9a7d-135">DateTimeOffset</span></span>|<span data-ttu-id="b9a7d-136">Das Enddatum und die Uhrzeit eines Bereichs Zeit dargestellt im ISO 8601-Format als UTC oder UTC-Offset.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-136">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="b9a7d-137">Beispielsweise 03: 00 Uhr UTC auf 1 Jan 2018 würde wie folgt aussehen: ' 2018-01-01T03:00:00Z ", und gleichzeitig in PST-Datei würde wie folgt aussehen: ' 2017-12-31T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="b9a7d-137">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="b9a7d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9a7d-138">Response</span></span>
<span data-ttu-id="b9a7d-139">Wenn der Vorgang erfolgreich war, gibt diese Methode `200, OK` Antwort Code und [BookingAppointment](../resources/bookingappointment.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-139">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a7d-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9a7d-140">Example</span></span>
<span data-ttu-id="b9a7d-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-141">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9a7d-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9a7d-142">Request</span></span>
<span data-ttu-id="b9a7d-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```

##### <a name="response"></a><span data-ttu-id="b9a7d-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9a7d-144">Response</span></span>
<span data-ttu-id="b9a7d-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-145">The following is an example of the response.</span></span> <span data-ttu-id="b9a7d-146">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b9a7d-147">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9a7d-147">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/calendarView",
    "value": [
        {
            "id": "AAMkADKpAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "customerName": "Adele Vance",
            "customerEmailAddress": "adelev@proseware.com",
            "customerPhone": "213-555-0156",
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
            "invoiceId": "1003",
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
                "dateTime": "2018-05-05T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-05T12:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (876 Tenth Avenue, Buffalo, NY 98052, USA)",
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
                "dateTime": "2018-05-05T12:30:00.0000000Z",
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-06T12:30:00.0000000Z",
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
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

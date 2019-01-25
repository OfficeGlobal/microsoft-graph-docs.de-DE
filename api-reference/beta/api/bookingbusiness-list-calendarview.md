---
title: Liste Buchungen calendarView
description: Rufen Sie die Auflistung von BookingAppointment-Objekten für ein BookingBusiness, die in der angegebene Datumsbereich auftritt.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 39b96e089d035ffd21155064252e36fd07a0a6c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526074"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="80aac-103">Liste Buchungen calendarView</span><span class="sxs-lookup"><span data-stu-id="80aac-103">List Bookings calendarView</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80aac-104">Rufen Sie die Auflistung von [BookingAppointment](../resources/bookingappointment.md) -Objekten für ein [BookingBusiness](../resources/bookingbusiness.md), die in der angegebene Datumsbereich auftritt.</span><span class="sxs-lookup"><span data-stu-id="80aac-104">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="80aac-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="80aac-105">Permissions</span></span>
<span data-ttu-id="80aac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80aac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80aac-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80aac-108">Permission type</span></span>      | <span data-ttu-id="80aac-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80aac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80aac-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80aac-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="80aac-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="80aac-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="80aac-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80aac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80aac-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80aac-113">Not supported.</span></span>   |
|<span data-ttu-id="80aac-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80aac-114">Application</span></span> | <span data-ttu-id="80aac-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80aac-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="80aac-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80aac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="80aac-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80aac-117">Request headers</span></span>
| <span data-ttu-id="80aac-118">Name</span><span class="sxs-lookup"><span data-stu-id="80aac-118">Name</span></span>       | <span data-ttu-id="80aac-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80aac-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80aac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="80aac-120">Authorization</span></span>  | <span data-ttu-id="80aac-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="80aac-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="80aac-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80aac-122">Request body</span></span>
<span data-ttu-id="80aac-123">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="80aac-123">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="80aac-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="80aac-124">Parameter</span></span>    | <span data-ttu-id="80aac-125">Typ</span><span class="sxs-lookup"><span data-stu-id="80aac-125">Type</span></span>   |<span data-ttu-id="80aac-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80aac-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80aac-127">start</span><span class="sxs-lookup"><span data-stu-id="80aac-127">start</span></span>|<span data-ttu-id="80aac-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80aac-128">DateTimeOffset</span></span>|<span data-ttu-id="80aac-129">Das Startdatum und die Uhrzeit der ein Zeitbereich dargestellt im ISO 8601-Format als UTC oder UTC-Offset.</span><span class="sxs-lookup"><span data-stu-id="80aac-129">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="80aac-130">Uhr UTC auf 1 Jan 2018 könnte beispielsweise wie folgt aussehen: ' 2018-01-01T00:00:00Z ", und gleichzeitig in PST-Datei würde wie folgt aussehen: ' 2017-12-31T16:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="80aac-130">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="80aac-131">end</span><span class="sxs-lookup"><span data-stu-id="80aac-131">end</span></span>|<span data-ttu-id="80aac-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80aac-132">DateTimeOffset</span></span>|<span data-ttu-id="80aac-133">Das Enddatum und die Uhrzeit eines Bereichs Zeit dargestellt im ISO 8601-Format als UTC oder UTC-Offset.</span><span class="sxs-lookup"><span data-stu-id="80aac-133">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="80aac-134">Beispielsweise 03: 00 Uhr UTC auf 1 Jan 2018 würde wie folgt aussehen: ' 2018-01-01T03:00:00Z ", und gleichzeitig in PST-Datei würde wie folgt aussehen: ' 2017-12-31T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="80aac-134">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="80aac-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="80aac-135">Response</span></span>
<span data-ttu-id="80aac-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `200, OK` Antwort Code und [BookingAppointment](../resources/bookingappointment.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="80aac-136">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80aac-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80aac-137">Example</span></span>
<span data-ttu-id="80aac-138">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="80aac-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80aac-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80aac-139">Request</span></span>
<span data-ttu-id="80aac-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80aac-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```

##### <a name="response"></a><span data-ttu-id="80aac-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="80aac-141">Response</span></span>
<span data-ttu-id="80aac-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="80aac-142">The following is an example of the response.</span></span> <span data-ttu-id="80aac-143">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="80aac-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="80aac-144">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80aac-144">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-calendarview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

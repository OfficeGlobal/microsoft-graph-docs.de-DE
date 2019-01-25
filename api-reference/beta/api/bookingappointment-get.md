---
title: Abrufen von bookingAppointment
description: Rufen Sie die Eigenschaften und die Beziehungen eines BookingAppointment-Objekts in der angegebenen Bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e9e9fffa3101656d4e426578185683065b4f5e5a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525269"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="bb883-103">Abrufen von bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="bb883-103">Get bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb883-104">Rufen Sie die Eigenschaften und die Beziehungen eines [BookingAppointment](../resources/bookingappointment.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="bb883-104">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="bb883-105">Die Eigenschaften **start** und **End** sind immer in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb883-105">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb883-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb883-106">Permissions</span></span>
<span data-ttu-id="bb883-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb883-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb883-109">Permission type</span></span>      | <span data-ttu-id="bb883-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb883-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb883-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb883-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="bb883-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="bb883-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bb883-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb883-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb883-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb883-114">Not supported.</span></span>   |
|<span data-ttu-id="bb883-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb883-115">Application</span></span> | <span data-ttu-id="bb883-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb883-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bb883-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb883-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb883-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bb883-118">Optional query parameters</span></span>
<span data-ttu-id="bb883-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bb883-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb883-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb883-120">Request headers</span></span>
| <span data-ttu-id="bb883-121">Name</span><span class="sxs-lookup"><span data-stu-id="bb883-121">Name</span></span>      |<span data-ttu-id="bb883-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb883-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb883-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb883-123">Authorization</span></span>  | <span data-ttu-id="bb883-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bb883-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb883-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb883-125">Request body</span></span>
<span data-ttu-id="bb883-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bb883-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bb883-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb883-127">Response</span></span>
<span data-ttu-id="bb883-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [BookingAppointment](../resources/bookingappointment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bb883-128">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb883-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb883-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb883-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb883-130">Request</span></span>
<span data-ttu-id="bb883-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb883-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="bb883-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb883-132">Response</span></span>
<span data-ttu-id="bb883-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bb883-133">The following is an example of the response.</span></span> <span data-ttu-id="bb883-134">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="bb883-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bb883-135">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb883-135">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

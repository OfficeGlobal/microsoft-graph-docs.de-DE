---
title: Erstellen von bookingService
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 9dfc2381d12e1fb48922ef95b405f5cbe3e24ed8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059683"
---
# <a name="create-bookingservice"></a><span data-ttu-id="d9539-104">Erstellen von bookingService</span><span class="sxs-lookup"><span data-stu-id="d9539-104">Create bookingService</span></span>

 > <span data-ttu-id="d9539-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d9539-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9539-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9539-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d9539-107">Erstellen Sie eine neue [BookingService](../resources/bookingservice.md) für die angegebene [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="d9539-107">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d9539-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9539-108">Permissions</span></span>
<span data-ttu-id="d9539-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9539-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9539-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9539-111">Permission type</span></span>      | <span data-ttu-id="d9539-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9539-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9539-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9539-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="d9539-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d9539-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d9539-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9539-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9539-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9539-116">Not supported.</span></span>   |
|<span data-ttu-id="d9539-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9539-117">Application</span></span> | <span data-ttu-id="d9539-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9539-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d9539-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9539-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="d9539-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9539-120">Request headers</span></span>
| <span data-ttu-id="d9539-121">Name</span><span class="sxs-lookup"><span data-stu-id="d9539-121">Name</span></span>       | <span data-ttu-id="d9539-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9539-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9539-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9539-123">Authorization</span></span>  | <span data-ttu-id="d9539-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d9539-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9539-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9539-125">Request body</span></span>
<span data-ttu-id="d9539-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingService](../resources/bookingservice.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d9539-126">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d9539-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9539-127">Response</span></span>
<span data-ttu-id="d9539-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `201, Created` Antwortobjekt Code und [BookingService](../resources/bookingservice.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d9539-128">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9539-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9539-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9539-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9539-130">Request</span></span>
<span data-ttu-id="d9539-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9539-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingservice_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT1H30M",
    "defaultLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"4567 First Street",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Contoso Lunch Delivery",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "defaultPrice":10.0,
    "defaultPriceType@odata.type":"#microsoft.graph.bookingPriceType",
    "defaultPriceType":"fixedPrice",
    "defaultReminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "defaultReminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be reminded that this service is tomorrow.",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        }
    ],
    "description":"Individual bento box lunch delivery",
    "displayName":"Bento",
    "isHiddenFromCustomers":false,
    "notes":"Home-cooked special",
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "schedulingPolicy":{
        "@odata.type":"#microsoft.graph.bookingSchedulingPolicy",
        "allowStaffSelection":true,
        "maximumAdvance":"P10D",
        "minimumLeadTime":"PT10H",
        "sendConfirmationsToOwner":true,
        "timeSlotInterval":"PT1H"
    },
    "staffMemberIds@odata.type":"#Collection(String)",
    "staffMemberIds":[
        "d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
        "2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
    ]
}
```
<span data-ttu-id="d9539-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingService](../resources/bookingservice.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d9539-132">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d9539-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9539-133">Response</span></span>
<span data-ttu-id="d9539-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d9539-134">The following is an example of the response.</span></span> <span data-ttu-id="d9539-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="d9539-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d9539-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9539-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT1H30M",
    "defaultPrice": 10,
    "defaultPriceType": "fixedPrice",
    "description": "Individual bento box lunch delivery",
    "isHiddenFromCustomers": false,
    "notes": "Home-cooked special",
    "preBuffer": "PT5M",
    "postBuffer": "PT10M",
    "staffMemberIds": [],
    "defaultLocation": {
        "displayName": "Contoso Lunch Delivery",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "4567 First Street",
            "city": "Buffalo",
            "state": "NY",
            "countryOrRegion": "USA",
            "postalCode": "98052"
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "defaultReminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "Please be reminded that this service is tomorrow."
        }
    ],
    "schedulingPolicy": {
        "timeSlotInterval": "PT1H",
        "minimumLeadTime": "PT10H",
        "maximumAdvance": "P10D",
        "sendConfirmationsToOwner": true,
        "allowStaffSelection": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
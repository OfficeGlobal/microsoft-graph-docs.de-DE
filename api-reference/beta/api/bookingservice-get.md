---
title: Abrufen von bookingService
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 7a309e076f480d051a1da47265dedaf4c32207d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819691"
---
# <a name="get-bookingservice"></a><span data-ttu-id="8ac97-104">Abrufen von bookingService</span><span class="sxs-lookup"><span data-stu-id="8ac97-104">Get bookingService</span></span>

 > <span data-ttu-id="8ac97-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ac97-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ac97-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ac97-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="8ac97-107">Rufen Sie die Eigenschaften und die Beziehungen eines [BookingService](../resources/bookingservice.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8ac97-107">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8ac97-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ac97-108">Permissions</span></span>
<span data-ttu-id="8ac97-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ac97-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ac97-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ac97-111">Permission type</span></span>      | <span data-ttu-id="8ac97-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ac97-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ac97-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ac97-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="8ac97-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="8ac97-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8ac97-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ac97-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ac97-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ac97-116">Not supported.</span></span>   |
|<span data-ttu-id="8ac97-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ac97-117">Application</span></span> | <span data-ttu-id="8ac97-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ac97-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8ac97-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ac97-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8ac97-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8ac97-120">Optional query parameters</span></span>
<span data-ttu-id="8ac97-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ac97-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ac97-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ac97-122">Request headers</span></span>
| <span data-ttu-id="8ac97-123">Name</span><span class="sxs-lookup"><span data-stu-id="8ac97-123">Name</span></span>      |<span data-ttu-id="8ac97-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ac97-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ac97-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ac97-125">Authorization</span></span>  | <span data-ttu-id="8ac97-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8ac97-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ac97-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ac97-127">Request body</span></span>
<span data-ttu-id="8ac97-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ac97-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8ac97-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ac97-129">Response</span></span>
<span data-ttu-id="8ac97-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [BookingService](../resources/bookingservice.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8ac97-130">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ac97-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ac97-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ac97-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ac97-132">Request</span></span>
<span data-ttu-id="8ac97-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ac97-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="8ac97-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ac97-134">Response</span></span>
<span data-ttu-id="8ac97-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ac97-135">The following is an example of the response.</span></span> <span data-ttu-id="8ac97-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="8ac97-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8ac97-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ac97-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT30M",
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
  "description": "Get bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

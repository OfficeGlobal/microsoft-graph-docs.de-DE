---
title: Abrufen von bookingBusiness
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 6df16d3c4dbb77c2e97e55fda1881a38c9270c22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809520"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="4bf13-104">Abrufen von bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="4bf13-104">Get bookingBusiness</span></span>

 > <span data-ttu-id="4bf13-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4bf13-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bf13-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4bf13-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="4bf13-107">Rufen Sie die Eigenschaften und die Beziehungen eines [BookingBusiness](../resources/bookingbusiness.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4bf13-107">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bf13-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4bf13-108">Permissions</span></span>
<span data-ttu-id="4bf13-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bf13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bf13-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4bf13-111">Permission type</span></span>      | <span data-ttu-id="4bf13-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4bf13-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bf13-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4bf13-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="4bf13-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4bf13-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4bf13-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4bf13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bf13-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bf13-116">Not supported.</span></span>   |
|<span data-ttu-id="4bf13-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4bf13-117">Application</span></span> | <span data-ttu-id="4bf13-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bf13-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="4bf13-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bf13-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4bf13-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4bf13-120">Optional query parameters</span></span>
<span data-ttu-id="4bf13-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4bf13-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bf13-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4bf13-122">Request headers</span></span>
| <span data-ttu-id="4bf13-123">Name</span><span class="sxs-lookup"><span data-stu-id="4bf13-123">Name</span></span>      |<span data-ttu-id="4bf13-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bf13-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4bf13-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bf13-125">Authorization</span></span>  | <span data-ttu-id="4bf13-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4bf13-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bf13-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4bf13-127">Request body</span></span>
<span data-ttu-id="4bf13-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4bf13-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4bf13-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bf13-129">Response</span></span>
<span data-ttu-id="4bf13-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [BookingBusiness](../resources/bookingbusiness.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4bf13-130">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4bf13-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4bf13-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bf13-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bf13-132">Request</span></span>
<span data-ttu-id="4bf13-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4bf13-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="4bf13-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bf13-134">Response</span></span>
<span data-ttu-id="4bf13-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4bf13-135">The following is an example of the response.</span></span> <span data-ttu-id="4bf13-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="4bf13-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4bf13-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4bf13-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"Fabrikam@M365B489948.onmicrosoft.com",
    "displayName":"Fabrikam",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fabrikam.com",
    "webSiteUrl":"https://www.fabrikam.com/",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"home",
        "postOfficeBox":"",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
        {
            "day":"monday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"tuesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"wednesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"thursday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"friday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"saturday",
            "timeSlots":[

            ]
        },
        {
            "day":"sunday",
            "timeSlots":[

            ]
        }
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

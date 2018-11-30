---
title: Erstellen von bookingBusiness
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 2da2a36624664238badd63c73bc2967ace25635b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058718"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="ffb64-104">Erstellen von bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="ffb64-104">Create bookingBusiness</span></span>

 > <span data-ttu-id="ffb64-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ffb64-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffb64-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ffb64-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="ffb64-107">Erstellen Sie ein neues Microsoft Bookings Unternehmen in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ffb64-107">Create a new Microsoft Bookings business in a tenant.</span></span> 

<span data-ttu-id="ffb64-108">Dies ist der erste Schritt beim Einrichten eines Unternehmens Buchungen, müssen Sie den Anzeigenamen Business angeben.</span><span class="sxs-lookup"><span data-stu-id="ffb64-108">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="ffb64-109">Sie können enthalten andere Informationen wie Geschäftsadresse, Websiteadresse und scheduling-Richtlinie, oder legen Sie diese Informationen später durch [Aktualisieren](bookingbusiness-update.md) der **BookingBusiness**.</span><span class="sxs-lookup"><span data-stu-id="ffb64-109">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="ffb64-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ffb64-110">Permissions</span></span>
<span data-ttu-id="ffb64-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffb64-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffb64-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ffb64-113">Permission type</span></span>      | <span data-ttu-id="ffb64-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ffb64-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffb64-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ffb64-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="ffb64-116">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ffb64-116">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="ffb64-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ffb64-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffb64-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffb64-118">Not supported.</span></span>   |
|<span data-ttu-id="ffb64-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffb64-119">Application</span></span> | <span data-ttu-id="ffb64-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffb64-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ffb64-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffb64-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="ffb64-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ffb64-122">Request headers</span></span>
| <span data-ttu-id="ffb64-123">Name</span><span class="sxs-lookup"><span data-stu-id="ffb64-123">Name</span></span>       | <span data-ttu-id="ffb64-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffb64-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ffb64-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffb64-125">Authorization</span></span>  | <span data-ttu-id="ffb64-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ffb64-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb64-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ffb64-127">Request body</span></span>
<span data-ttu-id="ffb64-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingBusiness](../resources/bookingbusiness.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ffb64-128">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ffb64-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffb64-129">Response</span></span>
<span data-ttu-id="ffb64-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `201, Created` Antwortobjekt Code und [BookingBusiness](../resources/bookingbusiness.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ffb64-130">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb64-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ffb64-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffb64-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffb64-132">Request</span></span>
<span data-ttu-id="ffb64-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ffb64-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingbusiness_from_bookingbusinesses"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Content-type: application/json

{
    "displayName":"Fourth Coffee",
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD"
}
```
<span data-ttu-id="ffb64-134">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingBusiness](../resources/bookingbusiness.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ffb64-134">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ffb64-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffb64-135">Response</span></span>
<span data-ttu-id="ffb64-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ffb64-136">The following is an example of the response.</span></span> <span data-ttu-id="ffb64-137">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ffb64-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ffb64-138">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffb64-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"fourthcoffee@M365B489948.onmicrosoft.com",
    "displayName":"Fourth Coffee",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
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
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
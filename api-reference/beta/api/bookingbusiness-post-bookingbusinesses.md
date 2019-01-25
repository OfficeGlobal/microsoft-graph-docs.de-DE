---
title: Erstellen von bookingBusiness
description: Erstellen Sie ein neues Microsoft Bookings Unternehmen in einem Mandanten.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 95a9217392953d287689dca7a7b6f4c74fbe6383
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519248"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="59e0a-103">Erstellen von bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="59e0a-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59e0a-104">Erstellen Sie ein neues Microsoft Bookings Unternehmen in einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="59e0a-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="59e0a-105">Dies ist der erste Schritt beim Einrichten eines Unternehmens Buchungen, müssen Sie den Anzeigenamen Business angeben.</span><span class="sxs-lookup"><span data-stu-id="59e0a-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="59e0a-106">Sie können enthalten andere Informationen wie Geschäftsadresse, Websiteadresse und scheduling-Richtlinie, oder legen Sie diese Informationen später durch [Aktualisieren](bookingbusiness-update.md) der **BookingBusiness**.</span><span class="sxs-lookup"><span data-stu-id="59e0a-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="59e0a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="59e0a-107">Permissions</span></span>
<span data-ttu-id="59e0a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59e0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59e0a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59e0a-110">Permission type</span></span>      | <span data-ttu-id="59e0a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59e0a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59e0a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59e0a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="59e0a-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="59e0a-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="59e0a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59e0a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59e0a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59e0a-115">Not supported.</span></span>   |
|<span data-ttu-id="59e0a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59e0a-116">Application</span></span> | <span data-ttu-id="59e0a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59e0a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59e0a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59e0a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="59e0a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59e0a-119">Request headers</span></span>
| <span data-ttu-id="59e0a-120">Name</span><span class="sxs-lookup"><span data-stu-id="59e0a-120">Name</span></span>       | <span data-ttu-id="59e0a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59e0a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59e0a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59e0a-122">Authorization</span></span>  | <span data-ttu-id="59e0a-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="59e0a-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="59e0a-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59e0a-124">Request body</span></span>
<span data-ttu-id="59e0a-125">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingBusiness](../resources/bookingbusiness.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="59e0a-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="59e0a-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="59e0a-126">Response</span></span>
<span data-ttu-id="59e0a-127">Wenn der Vorgang erfolgreich war, gibt diese Methode `201, Created` Antwortobjekt Code und [BookingBusiness](../resources/bookingbusiness.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="59e0a-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59e0a-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59e0a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59e0a-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59e0a-129">Request</span></span>
<span data-ttu-id="59e0a-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59e0a-130">The following is an example of the request.</span></span>
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
<span data-ttu-id="59e0a-131">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingBusiness](../resources/bookingbusiness.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="59e0a-131">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="59e0a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="59e0a-132">Response</span></span>
<span data-ttu-id="59e0a-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="59e0a-133">The following is an example of the response.</span></span> <span data-ttu-id="59e0a-134">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="59e0a-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="59e0a-135">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59e0a-135">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

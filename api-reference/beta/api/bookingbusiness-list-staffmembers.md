---
title: Liste staffMembers
description: Rufen Sie eine Liste der BookingStaffMember-Objekte in der angegebenen Bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4d8cfcfcab5478149404f4ac990ab45aa0d61c1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527549"
---
# <a name="list-staffmembers"></a><span data-ttu-id="2e5b3-103">Liste staffMembers</span><span class="sxs-lookup"><span data-stu-id="2e5b3-103">List staffMembers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e5b3-104">Rufen Sie eine Liste der [BookingStaffMember](../resources/bookingstaffmember.md) -Objekte in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="2e5b3-104">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2e5b3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2e5b3-105">Permissions</span></span>
<span data-ttu-id="2e5b3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e5b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e5b3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e5b3-108">Permission type</span></span>      | <span data-ttu-id="2e5b3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e5b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e5b3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e5b3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2e5b3-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="2e5b3-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2e5b3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e5b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e5b3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e5b3-113">Not supported.</span></span>   |
|<span data-ttu-id="2e5b3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e5b3-114">Application</span></span> | <span data-ttu-id="2e5b3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e5b3-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2e5b3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e5b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e5b3-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2e5b3-117">Optional query parameters</span></span>
<span data-ttu-id="2e5b3-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2e5b3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e5b3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e5b3-119">Request headers</span></span>
| <span data-ttu-id="2e5b3-120">Name</span><span class="sxs-lookup"><span data-stu-id="2e5b3-120">Name</span></span>      |<span data-ttu-id="2e5b3-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e5b3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e5b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e5b3-122">Authorization</span></span>  | <span data-ttu-id="2e5b3-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2e5b3-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e5b3-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e5b3-124">Request body</span></span>
<span data-ttu-id="2e5b3-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2e5b3-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2e5b3-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e5b3-126">Response</span></span>
<span data-ttu-id="2e5b3-127">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="2e5b3-127">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e5b3-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e5b3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e5b3-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e5b3-129">Request</span></span>
<span data-ttu-id="2e5b3-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e5b3-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
##### <a name="response"></a><span data-ttu-id="2e5b3-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e5b3-131">Response</span></span>
<span data-ttu-id="2e5b3-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2e5b3-132">The following is an example of the response.</span></span> <span data-ttu-id="2e5b3-133">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="2e5b3-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2e5b3-134">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e5b3-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers",
    "value":[
        {
            "id":"8ee1c803-a1fa-406d-8259-7ab53233f148",
            "displayName":"Dana Swope",
            "emailAddress":"danas@contoso.com",
            "availabilityIsAffectedByPersonalCalendar":false,
            "colorIndex":1,
            "role":"externalGuest",
            "useBusinessHours":true,
            "workingHours":[
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
                }
            ]
        },
        {
            "id":"71d64d0e-7225-49b6-b0b1-070d476cda51",
            "displayName":"Samantha Booth",
            "emailAddress":"samanthab@M365B489948.OnMicrosoft.com",
            "availabilityIsAffectedByPersonalCalendar":true,
            "colorIndex":0,
            "role":"administrator",
            "useBusinessHours":true,
            "workingHours":[
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
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-staffmembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

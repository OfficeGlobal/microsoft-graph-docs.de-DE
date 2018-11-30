---
title: Erstellen von bookingStaffMember
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 01983d5a0831b47c2eddfa45dad917f30bdd7b8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060031"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="fe179-104">Erstellen von bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="fe179-104">Create bookingStaffMember</span></span>

 > <span data-ttu-id="fe179-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fe179-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe179-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe179-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="fe179-107">Erstellen Sie einen neuen [Mitarbeiter](../resources/bookingstaffmember.md) in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="fe179-107">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="fe179-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe179-108">Permissions</span></span>
<span data-ttu-id="fe179-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe179-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe179-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe179-111">Permission type</span></span>      | <span data-ttu-id="fe179-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe179-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe179-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe179-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fe179-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="fe179-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fe179-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe179-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe179-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe179-116">Not supported.</span></span>   |
|<span data-ttu-id="fe179-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe179-117">Application</span></span> | <span data-ttu-id="fe179-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe179-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fe179-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe179-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="fe179-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe179-120">Request headers</span></span>
| <span data-ttu-id="fe179-121">Name</span><span class="sxs-lookup"><span data-stu-id="fe179-121">Name</span></span>       | <span data-ttu-id="fe179-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe179-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fe179-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe179-123">Authorization</span></span>  | <span data-ttu-id="fe179-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fe179-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe179-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe179-125">Request body</span></span>
<span data-ttu-id="fe179-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingStaffMember](../resources/bookingstaffmember.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fe179-126">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="fe179-127">Sie müssen die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="fe179-127">You must include the following properties:</span></span>

- <span data-ttu-id="fe179-128">**displayName**</span><span class="sxs-lookup"><span data-stu-id="fe179-128">**displayName**</span></span>
- <span data-ttu-id="fe179-129">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="fe179-129">**emailAddress**</span></span>
- <span data-ttu-id="fe179-130">**role**</span><span class="sxs-lookup"><span data-stu-id="fe179-130">**role**</span></span>


## <a name="response"></a><span data-ttu-id="fe179-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe179-131">Response</span></span>
<span data-ttu-id="fe179-132">Wenn der Vorgang erfolgreich war, gibt diese Methode `201, Created` Antwortobjekt Code und [BookingStaffMember](../resources/bookingstaffmember.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fe179-132">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe179-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe179-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe179-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe179-134">Request</span></span>
<span data-ttu-id="fe179-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe179-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingstaffmember_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Content-type: application/json
Content-length: 309

{
    "@odata.type":"#microsoft.graph.bookingStaffMember",
    "colorIndex":1,
    "displayName":"Dana Swope",
    "emailAddress":"danas@contoso.com",
    "role@odata.type":"#microsoft.graph.bookingStaffRole",
    "role":"externalGuest",
    "useBusinessHours":true,
    "workingHours@odata.type":"#Collection(microsoft.graph.bookingWorkHours)",
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
<span data-ttu-id="fe179-136">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingStaffMember](../resources/bookingstaffmember.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fe179-136">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fe179-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe179-137">Response</span></span>
<span data-ttu-id="fe179-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fe179-138">The following is an example of the response.</span></span> <span data-ttu-id="fe179-139">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="fe179-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe179-140">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe179-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
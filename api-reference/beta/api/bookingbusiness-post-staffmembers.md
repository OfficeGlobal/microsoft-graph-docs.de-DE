---
title: Erstellen von bookingStaffMember
description: Erstellen Sie einen neuen Mitarbeiter in der angegebenen Bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f3f13f30f646da8bf0fc8e32075002c0e591e902
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518611"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="8ec08-103">Erstellen von bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="8ec08-103">Create bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ec08-104">Erstellen Sie einen neuen [Mitarbeiter](../resources/bookingstaffmember.md) in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8ec08-104">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8ec08-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ec08-105">Permissions</span></span>
<span data-ttu-id="8ec08-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ec08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ec08-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ec08-108">Permission type</span></span>      | <span data-ttu-id="8ec08-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ec08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ec08-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ec08-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8ec08-111">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="8ec08-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8ec08-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ec08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ec08-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ec08-113">Not supported.</span></span>   |
|<span data-ttu-id="8ec08-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ec08-114">Application</span></span> | <span data-ttu-id="8ec08-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ec08-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8ec08-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ec08-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="8ec08-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ec08-117">Request headers</span></span>
| <span data-ttu-id="8ec08-118">Name</span><span class="sxs-lookup"><span data-stu-id="8ec08-118">Name</span></span>       | <span data-ttu-id="8ec08-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ec08-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ec08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ec08-120">Authorization</span></span>  | <span data-ttu-id="8ec08-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8ec08-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ec08-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ec08-122">Request body</span></span>
<span data-ttu-id="8ec08-123">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingStaffMember](../resources/bookingstaffmember.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ec08-123">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="8ec08-124">Sie müssen die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="8ec08-124">You must include the following properties:</span></span>

- <span data-ttu-id="8ec08-125">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8ec08-125">**displayName**</span></span>
- <span data-ttu-id="8ec08-126">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="8ec08-126">**emailAddress**</span></span>
- <span data-ttu-id="8ec08-127">Rolle</span><span class="sxs-lookup"><span data-stu-id="8ec08-127">**role**</span></span>


## <a name="response"></a><span data-ttu-id="8ec08-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ec08-128">Response</span></span>
<span data-ttu-id="8ec08-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `201, Created` Antwortobjekt Code und [BookingStaffMember](../resources/bookingstaffmember.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8ec08-129">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ec08-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ec08-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ec08-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ec08-131">Request</span></span>
<span data-ttu-id="8ec08-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ec08-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="8ec08-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [BookingStaffMember](../resources/bookingstaffmember.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ec08-133">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8ec08-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ec08-134">Response</span></span>
<span data-ttu-id="8ec08-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ec08-135">The following is an example of the response.</span></span> <span data-ttu-id="8ec08-136">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="8ec08-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8ec08-137">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ec08-137">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-staffmembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

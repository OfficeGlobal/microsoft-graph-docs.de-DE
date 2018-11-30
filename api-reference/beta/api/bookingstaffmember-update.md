---
title: Bookingstaffmember aktualisieren
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 99501f31ccd2b810d6a0c7f836d5b70bb98f223b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059123"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="ee2a0-104">Bookingstaffmember aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ee2a0-104">Update bookingstaffmember</span></span>

 > <span data-ttu-id="ee2a0-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee2a0-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="ee2a0-107">Aktualisieren Sie die Eigenschaften einer [BookingStaffMember](../resources/bookingstaffmember.md) in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="ee2a0-107">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ee2a0-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ee2a0-108">Permissions</span></span>
<span data-ttu-id="ee2a0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee2a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee2a0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee2a0-111">Permission type</span></span>      | <span data-ttu-id="ee2a0-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee2a0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee2a0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee2a0-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="ee2a0-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ee2a0-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ee2a0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee2a0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee2a0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee2a0-116">Not supported.</span></span>   |
|<span data-ttu-id="ee2a0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee2a0-117">Application</span></span> | <span data-ttu-id="ee2a0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee2a0-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ee2a0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee2a0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ee2a0-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee2a0-120">Optional request headers</span></span>
| <span data-ttu-id="ee2a0-121">Name</span><span class="sxs-lookup"><span data-stu-id="ee2a0-121">Name</span></span>       | <span data-ttu-id="ee2a0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee2a0-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ee2a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee2a0-123">Authorization</span></span>  | <span data-ttu-id="ee2a0-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ee2a0-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee2a0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee2a0-125">Request body</span></span>
<span data-ttu-id="ee2a0-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ee2a0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee2a0-129">Property</span></span>     | <span data-ttu-id="ee2a0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ee2a0-130">Type</span></span>   |<span data-ttu-id="ee2a0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee2a0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee2a0-132">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="ee2a0-132">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="ee2a0-133">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ee2a0-133">Boolean</span></span>|<span data-ttu-id="ee2a0-134">True gibt an, wenn der Mitarbeiter Office 365-Benutzer ist, die API Buchungen der Mitarbeiter persönlichen Kalender in Office 365 sowie die **WorkingHours** -Eigenschaft verwendet, um Verfügbarkeit zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-134">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="ee2a0-135">colorIndex</span><span class="sxs-lookup"><span data-stu-id="ee2a0-135">colorIndex</span></span>|<span data-ttu-id="ee2a0-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ee2a0-136">Int32</span></span>|<span data-ttu-id="ee2a0-137">Identifiziert eine Farbe, um die Mitarbeiter darstellen.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-137">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="ee2a0-138">Die Farbe entspricht der Farbpalette in der Detailseite für **Mitarbeiter** in der app Buchungen.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-138">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="ee2a0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ee2a0-139">displayName</span></span>|<span data-ttu-id="ee2a0-140">String</span><span class="sxs-lookup"><span data-stu-id="ee2a0-140">String</span></span>|<span data-ttu-id="ee2a0-141">Der Name des Mitarbeiters, wie Kunden angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-141">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="ee2a0-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ee2a0-142">emailAddress</span></span>|<span data-ttu-id="ee2a0-143">String</span><span class="sxs-lookup"><span data-stu-id="ee2a0-143">String</span></span>|<span data-ttu-id="ee2a0-144">Die e-Mail-Adresse des Mitarbeiters.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-144">The email address of the staff member.</span></span> <span data-ttu-id="ee2a0-145">Dies kann in der gleichen Office 365-Mandanten als das Unternehmen oder in eine andere e-Mail-Domäne sein.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-145">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="ee2a0-146">Diese e-Mail-Adresse wird verwendet, wenn die **SendConfirmationsToOwner** -Eigenschaft festgelegt ist, auf "true" in der scheduling Richtlinie des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-146">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="ee2a0-147">role</span><span class="sxs-lookup"><span data-stu-id="ee2a0-147">role</span></span>|<span data-ttu-id="ee2a0-148">string</span><span class="sxs-lookup"><span data-stu-id="ee2a0-148">string</span></span>| <span data-ttu-id="ee2a0-149">Die Rolle des Mitarbeiters im Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-149">The role of the staff member in the business.</span></span> <span data-ttu-id="ee2a0-150">Mögliche Werte: sind `guest`, `administrator`, `viewer` und `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-150">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="ee2a0-151">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="ee2a0-151">useBusinessHours</span></span>|<span data-ttu-id="ee2a0-152">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ee2a0-152">Boolean</span></span>|<span data-ttu-id="ee2a0-153">"True" bedeutet, dass die Mitarbeiter Verfügbarkeit durch die **BusinessHours** -Eigenschaft des Unternehmens bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-153">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="ee2a0-154">False bedeutet, dass die Verfügbarkeit durch die Einstellung für die Mitarbeiter **WorkingHouse** -Eigenschaft bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-154">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="ee2a0-155">workingHours</span><span class="sxs-lookup"><span data-stu-id="ee2a0-155">workingHours</span></span>|<span data-ttu-id="ee2a0-156">[BookingWorkHours](../resources/bookingworkhours.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ee2a0-156">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="ee2a0-157">Der Bereich der Stunden jeden Tag der Woche, die der Mitarbeiter für buchen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-157">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="ee2a0-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee2a0-158">Response</span></span>
<span data-ttu-id="ee2a0-p109">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-p109">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee2a0-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee2a0-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee2a0-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee2a0-162">Request</span></span>
<span data-ttu-id="ee2a0-163">Das folgende Beispiel ändert die Mitarbeiter Zeitplan montags deaktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-163">The following example changes the staff member's schedule to have Mondays off.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
   
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
##### <a name="response"></a><span data-ttu-id="ee2a0-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee2a0-164">Response</span></span>
<span data-ttu-id="ee2a0-165">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ee2a0-165">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
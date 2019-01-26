---
title: Ereignis aktualisieren
description: Aktualisieren Sie die Eigenschaften des Event-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ec895230ab981e4ccf9b2520a83f40a159386d64
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571821"
---
# <a name="update-event"></a><span data-ttu-id="6d60a-103">Ereignis aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6d60a-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d60a-104">Aktualisieren Sie die Eigenschaften des [Event](../resources/event.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d60a-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6d60a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6d60a-105">Permissions</span></span>
<span data-ttu-id="6d60a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d60a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d60a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d60a-108">Permission type</span></span>      | <span data-ttu-id="6d60a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d60a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d60a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d60a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d60a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d60a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6d60a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d60a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d60a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d60a-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6d60a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d60a-114">Application</span></span> | <span data-ttu-id="6d60a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d60a-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d60a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d60a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6d60a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d60a-117">Request headers</span></span>
| <span data-ttu-id="6d60a-118">Name</span><span class="sxs-lookup"><span data-stu-id="6d60a-118">Name</span></span>       | <span data-ttu-id="6d60a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="6d60a-119">Type</span></span> | <span data-ttu-id="6d60a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d60a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d60a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d60a-121">Authorization</span></span>  | <span data-ttu-id="6d60a-122">string</span><span class="sxs-lookup"><span data-stu-id="6d60a-122">string</span></span>  | <span data-ttu-id="6d60a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6d60a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d60a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d60a-125">Request body</span></span>
<span data-ttu-id="6d60a-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="6d60a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6d60a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d60a-129">Property</span></span>       | <span data-ttu-id="6d60a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6d60a-130">Type</span></span>    | <span data-ttu-id="6d60a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d60a-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="6d60a-132">attendees</span><span class="sxs-lookup"><span data-stu-id="6d60a-132">attendees</span></span>|<span data-ttu-id="6d60a-133">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="6d60a-133">Attendee</span></span>|<span data-ttu-id="6d60a-134">Die Sammlung der Teilnehmer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="6d60a-134">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="6d60a-135">body</span><span class="sxs-lookup"><span data-stu-id="6d60a-135">body</span></span>|<span data-ttu-id="6d60a-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="6d60a-136">ItemBody</span></span>|<span data-ttu-id="6d60a-137">Der Text der Nachricht, die mit diesem Ereignis verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="6d60a-137">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="6d60a-138">categories</span><span class="sxs-lookup"><span data-stu-id="6d60a-138">categories</span></span>|<span data-ttu-id="6d60a-139">String</span><span class="sxs-lookup"><span data-stu-id="6d60a-139">String</span></span>|<span data-ttu-id="6d60a-140">Die Kategorien, die mit dem Ereignis verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="6d60a-140">The categories associated with the event.</span></span>|
| <span data-ttu-id="6d60a-141">end</span><span class="sxs-lookup"><span data-stu-id="6d60a-141">end</span></span>|<span data-ttu-id="6d60a-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d60a-142">DateTimeTimeZone</span></span>|<span data-ttu-id="6d60a-143">Datum und Uhrzeit für das Ende des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6d60a-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="6d60a-p104">Standardmäßig ist die Endzeit in UTC angegeben. Sie können eine optionale Zeitzone in EndTimeZone angeben, die Endzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von EndTimeZone auch ein Wert für StartTimeZone angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="6d60a-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="6d60a-147">In diesem Beispiel wird der 25. Februar 2015 21:34 in PST angegeben: „2015-02-25T21:34:00-08:00“.</span><span class="sxs-lookup"><span data-stu-id="6d60a-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="6d60a-148">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="6d60a-148">importance</span></span>|<span data-ttu-id="6d60a-149">String</span><span class="sxs-lookup"><span data-stu-id="6d60a-149">String</span></span>|<span data-ttu-id="6d60a-150">Die Wichtigkeit des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6d60a-150">The importance of the event.</span></span> <span data-ttu-id="6d60a-151">Mögliche Werte sind: `low`, `normal` und `high`.</span><span class="sxs-lookup"><span data-stu-id="6d60a-151">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="6d60a-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="6d60a-152">isAllDay</span></span>|<span data-ttu-id="6d60a-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d60a-153">Boolean</span></span>|<span data-ttu-id="6d60a-154">True, wenn das Ereignis den ganzen Tag andauert.</span><span class="sxs-lookup"><span data-stu-id="6d60a-154">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="6d60a-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="6d60a-155">isReminderOn</span></span>|<span data-ttu-id="6d60a-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d60a-156">Boolean</span></span>|<span data-ttu-id="6d60a-157">True, wenn eine Benachrichtigung den Benutzer an das Ereignis erinnern soll.</span><span class="sxs-lookup"><span data-stu-id="6d60a-157">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="6d60a-158">location</span><span class="sxs-lookup"><span data-stu-id="6d60a-158">location</span></span>| [<span data-ttu-id="6d60a-159">location</span><span class="sxs-lookup"><span data-stu-id="6d60a-159">location</span></span>](../resources/location.md) |<span data-ttu-id="6d60a-160">Der Ort des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6d60a-160">The location of the event.</span></span>|
| <span data-ttu-id="6d60a-161">locations</span><span class="sxs-lookup"><span data-stu-id="6d60a-161">locations</span></span>| <span data-ttu-id="6d60a-162">[location](../resources/location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d60a-162">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="6d60a-163">Die Orte, an denen die Veranstaltung stattfindet.</span><span class="sxs-lookup"><span data-stu-id="6d60a-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="6d60a-164">Die Eigenschaften **location** und **locations** entsprechen sich immer gegenseitig.</span><span class="sxs-lookup"><span data-stu-id="6d60a-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="6d60a-165">Wenn Sie die **location**-Eigenschaft aktualisieren, werden alle früheren Orte in der **locations**-Sammlung entfernt und durch den neuen **location**-Wert ersetzt.</span><span class="sxs-lookup"><span data-stu-id="6d60a-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="6d60a-166">recurrence</span><span class="sxs-lookup"><span data-stu-id="6d60a-166">recurrence</span></span>| [<span data-ttu-id="6d60a-167">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="6d60a-167">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) |<span data-ttu-id="6d60a-168">Das Serienmuster für das Ereignis.</span><span class="sxs-lookup"><span data-stu-id="6d60a-168">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="6d60a-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="6d60a-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="6d60a-170">Int32</span><span class="sxs-lookup"><span data-stu-id="6d60a-170">Int32</span></span>|<span data-ttu-id="6d60a-171">Festlegung, wie viele Minuten vor Beginn des Ereignisses die Erinnerung angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="6d60a-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="6d60a-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="6d60a-172">responseRequested</span></span>|<span data-ttu-id="6d60a-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d60a-173">Boolean</span></span>|<span data-ttu-id="6d60a-174">Legen Sie „True“ fest, wenn der Absender eine Antwort erhalten soll, wenn das Ereignis akzeptiert oder abgelehnt wird.</span><span class="sxs-lookup"><span data-stu-id="6d60a-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="6d60a-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="6d60a-175">sensitivity</span></span>|<span data-ttu-id="6d60a-176">String</span><span class="sxs-lookup"><span data-stu-id="6d60a-176">String</span></span>| <span data-ttu-id="6d60a-177">Mögliche Werte: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="6d60a-177">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="6d60a-178">showAs</span><span class="sxs-lookup"><span data-stu-id="6d60a-178">showAs</span></span>|<span data-ttu-id="6d60a-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d60a-179">String</span></span>|<span data-ttu-id="6d60a-180">Der anzuzeigende Status.</span><span class="sxs-lookup"><span data-stu-id="6d60a-180">The status to show.</span></span> <span data-ttu-id="6d60a-181">Mögliche Werte sind: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6d60a-181">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="6d60a-182">start</span><span class="sxs-lookup"><span data-stu-id="6d60a-182">start</span></span>|<span data-ttu-id="6d60a-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d60a-183">DateTimeTimeZone</span></span>|<span data-ttu-id="6d60a-184">Die Startzeit des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6d60a-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="6d60a-p108">Standardmäßig ist die Startzeit in UTC angegeben. Sie können eine optionale Zeitzone in StartTimeZone angeben, die Startzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von StartTimeZone auch ein Wert für EndTimeZone angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="6d60a-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="6d60a-188">In diesem Beispiel wird 25. Februar 2015 19:34 in PST angegeben: „2015-02-25T19:34:00-08:00“.</span><span class="sxs-lookup"><span data-stu-id="6d60a-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="6d60a-189">Betreff</span><span class="sxs-lookup"><span data-stu-id="6d60a-189">subject</span></span>|<span data-ttu-id="6d60a-190">String</span><span class="sxs-lookup"><span data-stu-id="6d60a-190">String</span></span>|<span data-ttu-id="6d60a-191">Der Text der Betreffzeile des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="6d60a-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="6d60a-192">Da die Ressource **Ereignis** [Extensions](/graph/extensibility-overview)unterstützt, können Sie mithilfe der `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz **Ereignis** .</span><span class="sxs-lookup"><span data-stu-id="6d60a-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="6d60a-193">Wenn das **Ereignis** sind Sie aktualisieren das master-Ereignis einer Terminserie ist, mehrere Teilnehmer und enthält Instanzen, die separat aktualisiert wurden, mehrere Benachrichtigung-e-Mails gesendet werden: einen für die master-Serie und jeweils eine pro Instanz, die hat aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="6d60a-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="6d60a-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d60a-194">Response</span></span>

<span data-ttu-id="6d60a-195">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [vent](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d60a-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="6d60a-196">**Hinweis:** Diese Methode kann eine HTTP-400-Bad Request Antwort mit den Fehlercode zurückgeben `ErrorOccurrenceCrossingBoundary` und die folgende Fehlermeldung angezeigt: geändertes Serienelement crossing oder überlappende benachbarten Serienelement ist.</span><span class="sxs-lookup"><span data-stu-id="6d60a-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="6d60a-197">Dies gibt an, dass das Update die folgenden Outlook-Einschränkung auf Serienausnahmen verletzt: das auftreten ein Serientermins kann nicht verschoben werden, auf oder vor dem Tag des vorherigen Vorkommens und kann nicht an oder nach dem Tag des folgenden Vorkommens verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="6d60a-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="6d60a-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d60a-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6d60a-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d60a-199">Request</span></span>

<span data-ttu-id="6d60a-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d60a-200">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

##### <a name="response"></a><span data-ttu-id="6d60a-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d60a-201">Response</span></span>
<span data-ttu-id="6d60a-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d60a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a><span data-ttu-id="6d60a-205">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6d60a-205">See also</span></span>

- [<span data-ttu-id="6d60a-206">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="6d60a-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6d60a-207">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="6d60a-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="6d60a-208">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="6d60a-208">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

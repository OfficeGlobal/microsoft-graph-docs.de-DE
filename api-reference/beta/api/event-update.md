---
title: Ereignis aktualisieren
description: Aktualisieren Sie die Eigenschaften des Event-Objekts.
ms.openlocfilehash: b6ae7d818b68bfa1288a80f24383210e8a5d2909
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065022"
---
# <a name="update-event"></a><span data-ttu-id="f33ca-103">Ereignis aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f33ca-103">Update event</span></span>

> <span data-ttu-id="f33ca-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f33ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f33ca-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f33ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f33ca-106">Aktualisieren Sie die Eigenschaften des [Event](../resources/event.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f33ca-106">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f33ca-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f33ca-107">Permissions</span></span>
<span data-ttu-id="f33ca-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f33ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f33ca-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f33ca-110">Permission type</span></span>      | <span data-ttu-id="f33ca-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f33ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f33ca-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f33ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f33ca-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f33ca-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f33ca-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f33ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f33ca-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f33ca-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f33ca-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f33ca-116">Application</span></span> | <span data-ttu-id="f33ca-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f33ca-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f33ca-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f33ca-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f33ca-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f33ca-119">Request headers</span></span>
| <span data-ttu-id="f33ca-120">Name</span><span class="sxs-lookup"><span data-stu-id="f33ca-120">Name</span></span>       | <span data-ttu-id="f33ca-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f33ca-121">Type</span></span> | <span data-ttu-id="f33ca-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f33ca-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f33ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f33ca-123">Authorization</span></span>  | <span data-ttu-id="f33ca-124">string</span><span class="sxs-lookup"><span data-stu-id="f33ca-124">string</span></span>  | <span data-ttu-id="f33ca-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f33ca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f33ca-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f33ca-127">Request body</span></span>
<span data-ttu-id="f33ca-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f33ca-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f33ca-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f33ca-131">Property</span></span>       | <span data-ttu-id="f33ca-132">Typ</span><span class="sxs-lookup"><span data-stu-id="f33ca-132">Type</span></span>    | <span data-ttu-id="f33ca-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f33ca-133">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="f33ca-134">attendees</span><span class="sxs-lookup"><span data-stu-id="f33ca-134">attendees</span></span>|<span data-ttu-id="f33ca-135">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="f33ca-135">Attendee</span></span>|<span data-ttu-id="f33ca-136">Die Sammlung der Teilnehmer des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="f33ca-136">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="f33ca-137">body</span><span class="sxs-lookup"><span data-stu-id="f33ca-137">body</span></span>|<span data-ttu-id="f33ca-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="f33ca-138">ItemBody</span></span>|<span data-ttu-id="f33ca-139">Der Text der Nachricht, die mit diesem Ereignis verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="f33ca-139">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="f33ca-140">categories</span><span class="sxs-lookup"><span data-stu-id="f33ca-140">categories</span></span>|<span data-ttu-id="f33ca-141">String</span><span class="sxs-lookup"><span data-stu-id="f33ca-141">String</span></span>|<span data-ttu-id="f33ca-142">Die Kategorien, die mit dem Ereignis verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="f33ca-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="f33ca-143">end</span><span class="sxs-lookup"><span data-stu-id="f33ca-143">end</span></span>|<span data-ttu-id="f33ca-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f33ca-144">DateTimeTimeZone</span></span>|<span data-ttu-id="f33ca-145">Datum und Uhrzeit für das Ende des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="f33ca-145">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="f33ca-p105">Standardmäßig ist die Endzeit in UTC angegeben. Sie können eine optionale Zeitzone in EndTimeZone angeben, die Endzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von EndTimeZone auch ein Wert für StartTimeZone angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="f33ca-p105">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="f33ca-149">In diesem Beispiel wird der 25. Februar 2015 21:34 in PST angegeben: „2015-02-25T21:34:00-08:00“.</span><span class="sxs-lookup"><span data-stu-id="f33ca-149">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="f33ca-150">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="f33ca-150">importance</span></span>|<span data-ttu-id="f33ca-151">String</span><span class="sxs-lookup"><span data-stu-id="f33ca-151">String</span></span>|<span data-ttu-id="f33ca-152">Die Wichtigkeit des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="f33ca-152">The importance of the event.</span></span> <span data-ttu-id="f33ca-153">Mögliche Werte sind: `low`, `normal` und `high`.</span><span class="sxs-lookup"><span data-stu-id="f33ca-153">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="f33ca-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="f33ca-154">isAllDay</span></span>|<span data-ttu-id="f33ca-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="f33ca-155">Boolean</span></span>|<span data-ttu-id="f33ca-156">True, wenn das Ereignis den ganzen Tag andauert.</span><span class="sxs-lookup"><span data-stu-id="f33ca-156">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="f33ca-157">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="f33ca-157">isReminderOn</span></span>|<span data-ttu-id="f33ca-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="f33ca-158">Boolean</span></span>|<span data-ttu-id="f33ca-159">True, wenn eine Benachrichtigung den Benutzer an das Ereignis erinnern soll.</span><span class="sxs-lookup"><span data-stu-id="f33ca-159">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="f33ca-160">location</span><span class="sxs-lookup"><span data-stu-id="f33ca-160">location</span></span>|<span data-ttu-id="f33ca-161">Ort</span><span class="sxs-lookup"><span data-stu-id="f33ca-161">Location</span></span>|<span data-ttu-id="f33ca-162">Der Ort des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="f33ca-162">The location of the event.</span></span>|
|<span data-ttu-id="f33ca-163">locations</span><span class="sxs-lookup"><span data-stu-id="f33ca-163">locations</span></span>|<span data-ttu-id="f33ca-164">[Standort](../resources/location.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f33ca-164">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="f33ca-165">Die Orte, an denen die Veranstaltung stattfindet.</span><span class="sxs-lookup"><span data-stu-id="f33ca-165">The locations where the event is held or attended from.</span></span> <span data-ttu-id="f33ca-166">Die Eigenschaften **location** und **locations** entsprechen sich immer gegenseitig.</span><span class="sxs-lookup"><span data-stu-id="f33ca-166">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="f33ca-167">Wenn Sie die **location**-Eigenschaft aktualisieren, werden alle früheren Orte in der **locations**-Sammlung entfernt und durch den neuen **location**-Wert ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f33ca-167">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="f33ca-168">recurrence</span><span class="sxs-lookup"><span data-stu-id="f33ca-168">recurrence</span></span>|<span data-ttu-id="f33ca-169">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f33ca-169">PatternedRecurrence</span></span>|<span data-ttu-id="f33ca-170">Das Serienmuster für das Ereignis.</span><span class="sxs-lookup"><span data-stu-id="f33ca-170">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="f33ca-171">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="f33ca-171">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="f33ca-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f33ca-172">Int32</span></span>|<span data-ttu-id="f33ca-173">Festlegung, wie viele Minuten vor Beginn des Ereignisses die Erinnerung angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="f33ca-173">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="f33ca-174">responseRequested</span><span class="sxs-lookup"><span data-stu-id="f33ca-174">responseRequested</span></span>|<span data-ttu-id="f33ca-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="f33ca-175">Boolean</span></span>|<span data-ttu-id="f33ca-176">Legen Sie „True“ fest, wenn der Absender eine Antwort erhalten soll, wenn das Ereignis akzeptiert oder abgelehnt wird.</span><span class="sxs-lookup"><span data-stu-id="f33ca-176">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="f33ca-177">sensitivity</span><span class="sxs-lookup"><span data-stu-id="f33ca-177">sensitivity</span></span>|<span data-ttu-id="f33ca-178">String</span><span class="sxs-lookup"><span data-stu-id="f33ca-178">String</span></span>| <span data-ttu-id="f33ca-179">Mögliche Werte: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="f33ca-179">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="f33ca-180">showAs</span><span class="sxs-lookup"><span data-stu-id="f33ca-180">showAs</span></span>|<span data-ttu-id="f33ca-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f33ca-181">String</span></span>|<span data-ttu-id="f33ca-182">Der anzuzeigende Status.</span><span class="sxs-lookup"><span data-stu-id="f33ca-182">The status to show.</span></span> <span data-ttu-id="f33ca-183">Mögliche Werte sind: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f33ca-183">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="f33ca-184">start</span><span class="sxs-lookup"><span data-stu-id="f33ca-184">start</span></span>|<span data-ttu-id="f33ca-185">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f33ca-185">DateTimeTimeZone</span></span>|<span data-ttu-id="f33ca-186">Die Startzeit des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="f33ca-186">The start time of the event.</span></span> <br/><br/><span data-ttu-id="f33ca-p109">Standardmäßig ist die Startzeit in UTC angegeben. Sie können eine optionale Zeitzone in StartTimeZone angeben, die Startzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von StartTimeZone auch ein Wert für EndTimeZone angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="f33ca-p109">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="f33ca-190">In diesem Beispiel wird 25. Februar 2015 19:34 in PST angegeben: „2015-02-25T19:34:00-08:00“.</span><span class="sxs-lookup"><span data-stu-id="f33ca-190">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="f33ca-191">Betreff</span><span class="sxs-lookup"><span data-stu-id="f33ca-191">subject</span></span>|<span data-ttu-id="f33ca-192">String</span><span class="sxs-lookup"><span data-stu-id="f33ca-192">String</span></span>|<span data-ttu-id="f33ca-193">Der Text der Betreffzeile des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="f33ca-193">The text of the event's subject line.</span></span>|

<span data-ttu-id="f33ca-194">Da die Ressource **Ereignis** [Extensions](/graph/extensibility-overview)unterstützt, können Sie mithilfe der `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz **Ereignis** .</span><span class="sxs-lookup"><span data-stu-id="f33ca-194">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="f33ca-195">Wenn das **Ereignis** sind Sie aktualisieren das master-Ereignis einer Terminserie ist, mehrere Teilnehmer und enthält Instanzen, die separat aktualisiert wurden, mehrere Benachrichtigung-e-Mails gesendet werden: einen für die master-Serie und jeweils eine pro Instanz, die hat aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="f33ca-195">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="f33ca-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="f33ca-196">Response</span></span>

<span data-ttu-id="f33ca-197">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [vent](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f33ca-197">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="f33ca-198">**Hinweis:** Diese Methode kann eine HTTP-400-Bad Request Antwort mit den Fehlercode zurückgeben `ErrorOccurrenceCrossingBoundary` und die folgende Fehlermeldung angezeigt: geändertes Serienelement crossing oder überlappende benachbarten Serienelement ist.</span><span class="sxs-lookup"><span data-stu-id="f33ca-198">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="f33ca-199">Dies gibt an, dass das Update die folgenden Outlook-Einschränkung auf Serienausnahmen verletzt: das auftreten ein Serientermins kann nicht verschoben werden, auf oder vor dem Tag des vorherigen Vorkommens und kann nicht an oder nach dem Tag des folgenden Vorkommens verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="f33ca-199">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="f33ca-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f33ca-200">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f33ca-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f33ca-201">Request</span></span>

<span data-ttu-id="f33ca-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f33ca-202">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f33ca-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="f33ca-203">Response</span></span>
<span data-ttu-id="f33ca-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f33ca-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="f33ca-207">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f33ca-207">See also</span></span>

- [<span data-ttu-id="f33ca-208">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="f33ca-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f33ca-209">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="f33ca-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f33ca-210">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="f33ca-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

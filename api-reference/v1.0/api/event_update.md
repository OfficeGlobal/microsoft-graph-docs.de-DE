# <a name="update-event"></a><span data-ttu-id="ffd40-101">Ereignis aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ffd40-101">Update event</span></span>

<span data-ttu-id="ffd40-102">Mit dieser API können Sie die Eigenschaften eines Ereignisobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="ffd40-102">Update the properties of event object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ffd40-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ffd40-103">Permissions</span></span>
<span data-ttu-id="ffd40-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffd40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ffd40-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ffd40-106">Permission type</span></span>      | <span data-ttu-id="ffd40-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ffd40-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffd40-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ffd40-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ffd40-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffd40-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ffd40-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ffd40-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffd40-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffd40-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ffd40-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffd40-112">Application</span></span> | <span data-ttu-id="ffd40-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffd40-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffd40-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffd40-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="ffd40-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ffd40-115">Request headers</span></span>
| <span data-ttu-id="ffd40-116">Name</span><span class="sxs-lookup"><span data-stu-id="ffd40-116">Name</span></span>       | <span data-ttu-id="ffd40-117">Typ</span><span class="sxs-lookup"><span data-stu-id="ffd40-117">Type</span></span> | <span data-ttu-id="ffd40-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffd40-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ffd40-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffd40-119">Authorization</span></span>  | <span data-ttu-id="ffd40-120">string</span><span class="sxs-lookup"><span data-stu-id="ffd40-120">string</span></span>  | <span data-ttu-id="ffd40-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ffd40-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffd40-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ffd40-123">Request body</span></span>
<span data-ttu-id="ffd40-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="ffd40-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ffd40-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ffd40-127">Property</span></span>     | <span data-ttu-id="ffd40-128">Typ</span><span class="sxs-lookup"><span data-stu-id="ffd40-128">Type</span></span>   |<span data-ttu-id="ffd40-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffd40-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffd40-130">attendees</span><span class="sxs-lookup"><span data-stu-id="ffd40-130">attendees</span></span>|[<span data-ttu-id="ffd40-131">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="ffd40-131">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="ffd40-132">Die Sammlung der Teilnehmer für das Ereignis.</span><span class="sxs-lookup"><span data-stu-id="ffd40-132">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="ffd40-133">body</span><span class="sxs-lookup"><span data-stu-id="ffd40-133">body</span></span>|[<span data-ttu-id="ffd40-134">ItemBody</span><span class="sxs-lookup"><span data-stu-id="ffd40-134">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="ffd40-135">Der Text der Nachricht, die mit diesem Ereignis verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="ffd40-135">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="ffd40-136">categories</span><span class="sxs-lookup"><span data-stu-id="ffd40-136">categories</span></span>|<span data-ttu-id="ffd40-137">String</span><span class="sxs-lookup"><span data-stu-id="ffd40-137">String</span></span>|<span data-ttu-id="ffd40-138">Die Kategorien, die mit dem Ereignis verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="ffd40-138">The categories associated with the event.</span></span>|
|<span data-ttu-id="ffd40-139">end</span><span class="sxs-lookup"><span data-stu-id="ffd40-139">end</span></span>|[<span data-ttu-id="ffd40-140">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ffd40-140">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="ffd40-141">Datum und Uhrzeit für das Ende des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="ffd40-141">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="ffd40-p104">Standardmäßig ist die Endzeit in UTC angegeben. Sie können eine optionale Zeitzone in EndTimeZone angeben, die Endzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von EndTimeZone auch ein Wert für StartTimeZone angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="ffd40-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="ffd40-145">In diesem Beispiel wird der 25. Februar 2015 21:34 in PST angegeben: „2015-02-25T21:34:00-08:00“.</span><span class="sxs-lookup"><span data-stu-id="ffd40-145">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="ffd40-146">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="ffd40-146">importance</span></span>|<span data-ttu-id="ffd40-147">String</span><span class="sxs-lookup"><span data-stu-id="ffd40-147">String</span></span>|<span data-ttu-id="ffd40-148">Die Wichtigkeit des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="ffd40-148">The importance of the event.</span></span> <span data-ttu-id="ffd40-149">Mögliche Werte sind: `low`, `normal` und `high`.</span><span class="sxs-lookup"><span data-stu-id="ffd40-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="ffd40-150">isAllDay</span><span class="sxs-lookup"><span data-stu-id="ffd40-150">isAllDay</span></span>|<span data-ttu-id="ffd40-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd40-151">Boolean</span></span>|<span data-ttu-id="ffd40-152">True, wenn das Ereignis den ganzen Tag andauert.</span><span class="sxs-lookup"><span data-stu-id="ffd40-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="ffd40-153">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="ffd40-153">isReminderOn</span></span>|<span data-ttu-id="ffd40-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd40-154">Boolean</span></span>|<span data-ttu-id="ffd40-155">True, wenn eine Benachrichtigung den Benutzer an das Ereignis erinnern soll.</span><span class="sxs-lookup"><span data-stu-id="ffd40-155">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="ffd40-156">location</span><span class="sxs-lookup"><span data-stu-id="ffd40-156">location</span></span>|[<span data-ttu-id="ffd40-157">Ort</span><span class="sxs-lookup"><span data-stu-id="ffd40-157">Location</span></span>](../resources/location.md)|<span data-ttu-id="ffd40-158">Der Ort des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="ffd40-158">The location of the event.</span></span>|
|<span data-ttu-id="ffd40-159">locations</span><span class="sxs-lookup"><span data-stu-id="ffd40-159">locations</span></span>|<span data-ttu-id="ffd40-160">[location](../resources/location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ffd40-160">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="ffd40-161">Die Orte, an denen die Veranstaltung stattfindet.</span><span class="sxs-lookup"><span data-stu-id="ffd40-161">The locations where the event is held or attended from.</span></span> <span data-ttu-id="ffd40-162">Die Eigenschaften **location** und **locations** entsprechen sich immer gegenseitig.</span><span class="sxs-lookup"><span data-stu-id="ffd40-162">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="ffd40-163">Wenn Sie die **location**-Eigenschaft aktualisieren, werden alle früheren Orte in der **locations**-Sammlung entfernt und durch den neuen **location**-Wert ersetzt.</span><span class="sxs-lookup"><span data-stu-id="ffd40-163">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="ffd40-164">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="ffd40-164">onlineMeetingUrl</span></span>|<span data-ttu-id="ffd40-165">String</span><span class="sxs-lookup"><span data-stu-id="ffd40-165">String</span></span>|<span data-ttu-id="ffd40-166">Eine URL für eine Onlinebesprechung.</span><span class="sxs-lookup"><span data-stu-id="ffd40-166">A URL for an online meeting.</span></span>|
|<span data-ttu-id="ffd40-167">recurrence</span><span class="sxs-lookup"><span data-stu-id="ffd40-167">recurrence</span></span>|[<span data-ttu-id="ffd40-168">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="ffd40-168">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="ffd40-169">Das Serienmuster für das Ereignis.</span><span class="sxs-lookup"><span data-stu-id="ffd40-169">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="ffd40-170">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="ffd40-170">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="ffd40-171">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd40-171">Int32</span></span>|<span data-ttu-id="ffd40-172">Festlegung, wie viele Minuten vor Beginn des Ereignisses die Erinnerung angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="ffd40-172">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="ffd40-173">responseRequested</span><span class="sxs-lookup"><span data-stu-id="ffd40-173">responseRequested</span></span>|<span data-ttu-id="ffd40-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd40-174">Boolean</span></span>|<span data-ttu-id="ffd40-175">Legen Sie „True“ fest, wenn der Absender eine Antwort erhalten soll, wenn das Ereignis akzeptiert oder abgelehnt wird.</span><span class="sxs-lookup"><span data-stu-id="ffd40-175">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="ffd40-176">sensitivity</span><span class="sxs-lookup"><span data-stu-id="ffd40-176">sensitivity</span></span>|<span data-ttu-id="ffd40-177">String</span><span class="sxs-lookup"><span data-stu-id="ffd40-177">String</span></span>| <span data-ttu-id="ffd40-178">Mögliche Werte: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="ffd40-178">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="ffd40-179">showAs</span><span class="sxs-lookup"><span data-stu-id="ffd40-179">showAs</span></span>|<span data-ttu-id="ffd40-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffd40-180">String</span></span>|<span data-ttu-id="ffd40-181">Der anzuzeigende Status.</span><span class="sxs-lookup"><span data-stu-id="ffd40-181">The status to show.</span></span> <span data-ttu-id="ffd40-182">Mögliche Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ffd40-182">Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="ffd40-183">start</span><span class="sxs-lookup"><span data-stu-id="ffd40-183">start</span></span>|[<span data-ttu-id="ffd40-184">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ffd40-184">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="ffd40-185">Die Startzeit des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="ffd40-185">The start time of the event.</span></span> <br/><br/><span data-ttu-id="ffd40-p108">Standardmäßig ist die Startzeit in UTC angegeben. Sie können eine optionale Zeitzone in StartTimeZone angeben, die Startzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von StartTimeZone auch ein Wert für EndTimeZone angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="ffd40-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="ffd40-189">In diesem Beispiel wird 25. Februar 2015 19:34 in PST angegeben: „2015-02-25T19:34:00-08:00“.</span><span class="sxs-lookup"><span data-stu-id="ffd40-189">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="ffd40-190">subject</span><span class="sxs-lookup"><span data-stu-id="ffd40-190">subject</span></span>|<span data-ttu-id="ffd40-191">String</span><span class="sxs-lookup"><span data-stu-id="ffd40-191">String</span></span>|<span data-ttu-id="ffd40-192">Der Text der Betreffzeile des Ereignisses</span><span class="sxs-lookup"><span data-stu-id="ffd40-192">The text of the event's subject line.</span></span>|

<span data-ttu-id="ffd40-193">Da die **event**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **event**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="ffd40-193">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

## <a name="response"></a><span data-ttu-id="ffd40-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffd40-194">Response</span></span>

<span data-ttu-id="ffd40-195">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [vent](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffd40-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffd40-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ffd40-196">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ffd40-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffd40-197">Request</span></span>

<span data-ttu-id="ffd40-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ffd40-198">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

##### <a name="response"></a><span data-ttu-id="ffd40-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffd40-199">Response</span></span>

<span data-ttu-id="ffd40-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffd40-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "time": "datetime-value"
  },
  "recurrence": null,  
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

## <a name="see-also"></a><span data-ttu-id="ffd40-203">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="ffd40-203">See also</span></span>

- [<span data-ttu-id="ffd40-204">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ffd40-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="ffd40-205">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ffd40-205">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="ffd40-206">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="ffd40-206">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

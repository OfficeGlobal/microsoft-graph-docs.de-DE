# <a name="update-user-mailbox-settings"></a><span data-ttu-id="99751-101">Postfacheinstellungen des Benutzers aktualisieren</span><span class="sxs-lookup"><span data-stu-id="99751-101">Update user mailbox settings</span></span>

<span data-ttu-id="99751-p101">Aktualisieren Sie eine oder mehrere Einstellungen des Postfachs des Benutzers. Dies umfasst die Einstellungen für [automatische Antworten](../resources/automaticrepliessetting.md) (automatische Benachrichtigung von Personen über den Empfang von E-Mails), [Gebietsschema](../resources/localeinfo.md) (Sprache und Land/Region), Zeitzone und die [Geschäftszeiten](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="99751-p101">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="99751-104">Diese Einstellungen können Sie im Rahmen des [mailboxSettings](../resources/mailboxsettings.md)-Elements aktivieren, konfigurieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="99751-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="99751-105">**Hinweis:** Sie können keine Postfacheinstellungen erstellen oder löschen.</span><span class="sxs-lookup"><span data-stu-id="99751-105">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="99751-106">Wenn Sie die bevorzugte Zeitzone für einen Benutzer aktualisieren, können Sie diese im Windows- oder im [IANA-Format](https://www.iana.org/time-zones) (auch als Olson-Zeitzone bezeichnet) angeben.</span><span class="sxs-lookup"><span data-stu-id="99751-106">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span>

## <a name="permissions"></a><span data-ttu-id="99751-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99751-107">Permissions</span></span>
<span data-ttu-id="99751-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="99751-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="99751-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99751-110">Permission type</span></span>      | <span data-ttu-id="99751-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99751-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99751-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99751-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99751-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99751-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="99751-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99751-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99751-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99751-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="99751-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99751-116">Application</span></span> | <span data-ttu-id="99751-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99751-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99751-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99751-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99751-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="99751-119">Optional query parameters</span></span>
<span data-ttu-id="99751-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="99751-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="99751-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99751-121">Request headers</span></span>
| <span data-ttu-id="99751-122">Name</span><span class="sxs-lookup"><span data-stu-id="99751-122">Name</span></span>       | <span data-ttu-id="99751-123">Typ</span><span class="sxs-lookup"><span data-stu-id="99751-123">Type</span></span> | <span data-ttu-id="99751-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99751-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99751-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="99751-125">Authorization</span></span>  | <span data-ttu-id="99751-126">string</span><span class="sxs-lookup"><span data-stu-id="99751-126">string</span></span>  | <span data-ttu-id="99751-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99751-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99751-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99751-129">Request body</span></span>
<span data-ttu-id="99751-p104">Geben Sie im Anforderungstext die Werte für die relevanten Eigenschaften an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Im Folgenden werden die beschreibbaren/aktualisierbaren Eigenschaften aufgelistet:</span><span class="sxs-lookup"><span data-stu-id="99751-p104">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="99751-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99751-134">Property</span></span>     | <span data-ttu-id="99751-135">Typ</span><span class="sxs-lookup"><span data-stu-id="99751-135">Type</span></span>   |<span data-ttu-id="99751-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99751-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99751-137">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="99751-137">automaticRepliesSetting</span></span>|[<span data-ttu-id="99751-138">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="99751-138">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="99751-139">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="99751-139">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="99751-140">Sie können solche Benachrichtigungen für nur einen zukünftigen Datumsbereich festlegen.</span><span class="sxs-lookup"><span data-stu-id="99751-140">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="99751-141">language</span><span class="sxs-lookup"><span data-stu-id="99751-141">language</span></span>|[<span data-ttu-id="99751-142">localeInfo</span><span class="sxs-lookup"><span data-stu-id="99751-142">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="99751-143">Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.</span><span class="sxs-lookup"><span data-stu-id="99751-143">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="99751-144">timeZone</span><span class="sxs-lookup"><span data-stu-id="99751-144">timeZone</span></span>|<span data-ttu-id="99751-145">string</span><span class="sxs-lookup"><span data-stu-id="99751-145">string</span></span>|<span data-ttu-id="99751-146">Die Standardzeitzone für das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="99751-146">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="99751-147">workingHours</span><span class="sxs-lookup"><span data-stu-id="99751-147">workingHours</span></span>|[<span data-ttu-id="99751-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="99751-148">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="99751-149">Die Stunden, Wochentage und die Zeitzone, an denen bzw. in der der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="99751-149">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="99751-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="99751-150">Response</span></span>

<span data-ttu-id="99751-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [mailboxSettings](../resources/mailboxSettings.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99751-151">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>


## <a name="errors"></a><span data-ttu-id="99751-152">Fehler</span><span class="sxs-lookup"><span data-stu-id="99751-152">Errors</span></span>

<span data-ttu-id="99751-153">Durch Festlegen von Geschäftszeiten mit falschen Werten können möglicherweise die folgenden Fehler zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="99751-153">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="99751-154">Szenario</span><span class="sxs-lookup"><span data-stu-id="99751-154">Scenario</span></span>   | <span data-ttu-id="99751-155">HTTP-Statuscode</span><span class="sxs-lookup"><span data-stu-id="99751-155">HTTP status code</span></span> | <span data-ttu-id="99751-156">Fehlercode</span><span class="sxs-lookup"><span data-stu-id="99751-156">Error code</span></span> | <span data-ttu-id="99751-157">Fehlermeldung</span><span class="sxs-lookup"><span data-stu-id="99751-157">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="99751-158">Ungültige **startTime** oder **endTime**</span><span class="sxs-lookup"><span data-stu-id="99751-158">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="99751-159">400</span><span class="sxs-lookup"><span data-stu-id="99751-159">400</span></span> | <span data-ttu-id="99751-160">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="99751-160">RequestBodyRead</span></span> | <span data-ttu-id="99751-161">Das Literal „08“ kann nicht in den erwarteten Typ „Edm.TimeOfDay“ konvertiert werden.</span><span class="sxs-lookup"><span data-stu-id="99751-161">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="99751-162">Die Startzeit größer als die Endzeit</span><span class="sxs-lookup"><span data-stu-id="99751-162">Start time is greater than end time</span></span> | <span data-ttu-id="99751-163">400</span><span class="sxs-lookup"><span data-stu-id="99751-163">400</span></span> | <span data-ttu-id="99751-164">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="99751-164">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="99751-165">Die Startzeit muss vor der Endzeit liegen.</span><span class="sxs-lookup"><span data-stu-id="99751-165">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="99751-166">Ungültiger Tag in **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="99751-166">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="99751-167">400</span><span class="sxs-lookup"><span data-stu-id="99751-167">400</span></span> | <span data-ttu-id="99751-168">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="99751-168">InvalidArguments</span></span> | <span data-ttu-id="99751-169">Der angeforderte Wert „RandomDay“ wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="99751-169">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="99751-170">Ungültige **timeZone**</span><span class="sxs-lookup"><span data-stu-id="99751-170">Invalid **timeZone**</span></span> | <span data-ttu-id="99751-171">400</span><span class="sxs-lookup"><span data-stu-id="99751-171">400</span></span> | <span data-ttu-id="99751-172">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="99751-172">InvalidTimeZone</span></span> | <span data-ttu-id="99751-173">Die angegebenen Zeitzoneneinstellungen sind ungültig.</span><span class="sxs-lookup"><span data-stu-id="99751-173">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="99751-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99751-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99751-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99751-175">Request</span></span>
<span data-ttu-id="99751-176">Im folgenden Beispiel werden automatische Antworten für einen bestimmten Datumsbereich durch Festlegen der folgenden Eigenschaften der **automaticRepliesSetting**-Eigenschaft aktiviert: **status**, **scheduledStartDateTime** und **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="99751-176">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "scheduledStartDateTime": {
          "dateTime": "2016-03-20T18:00:00.0000000",
          "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
          "dateTime": "2016-03-28T18:00:00.0000000",
          "timeZone": "UTC"
        }
    }
}
```
##### <a name="response"></a><span data-ttu-id="99751-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="99751-177">Response</span></span>
<span data-ttu-id="99751-178">Die Antwort enthält die aktualisierten Einstellungen für automatische Antworten.</span><span class="sxs-lookup"><span data-stu-id="99751-178">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="99751-179">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="99751-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="99751-180">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99751-180">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "all",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-20T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T02:00:00.0000000",
            "timeZone": "UTC"
        },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="99751-181">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="99751-181">Request 2</span></span>
<span data-ttu-id="99751-182">Das zweite Beispiel passt die Zeitzone für die Geschäftszeiten des angemeldeten Benutzers an, indem die **timeZone**-Eigenschaft auf eine [benutzerdefinierte Zeitzone](../resources/customtimezone.md) festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="99751-182">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
  "workingHours": {
      "endTime" : "18:30:00.0000000", 
      "daysOfWeek": [ 
          "Monday", 
          "Tuesday", 
          "Wednesday", 
          "Thursday", 
          "Friday", 
          "Saturday" 
      ], 
      "timeZone" : { 
         "@odata.type": "#microsoft.graph.customTimeZone", 
         "bias":-300, 
         "name": "Customized Time Zone",
         "standardOffset":{   
           "time":"02:00:00.0000000", 
           "dayOccurrence":2, 
           "dayOfWeek":"Sunday", 
           "month":10, 
           "year":0 
         }, 
         "daylightOffset":{   
           "daylightBias":100, 
           "time":"02:00:00.0000000", 
           "dayOccurrence":4, 
           "dayOfWeek":"Sunday", 
           "month":5, 
           "year":0 
         } 
      } 
  }
} 
```
##### <a name="response-2"></a><span data-ttu-id="99751-183">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="99751-183">Response 2</span></span>
<span data-ttu-id="99751-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99751-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday",
            "saturday"
        ],
        "startTime":"09:00:00.0000000",
        "endTime":"18:30:00.0000000",
        "timeZone":{
            "@odata.type":"#microsoft.graph.customTimeZone",
            "bias":-200,
            "name":"Customized Time Zone",
            "standardOffset":{
                "time":"02:00:00.0000000",
                "dayOccurrence":4,
                "dayOfWeek":"sunday",
                "month":5,
                "year":0
            },
            "daylightOffset":{
                "daylightBias":-100,
                "time":"02:00:00.0000000",
                "dayOccurrence":2,
                "dayOfWeek":"sunday",
                "month":10,
                "year":0
            }
        }
    }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
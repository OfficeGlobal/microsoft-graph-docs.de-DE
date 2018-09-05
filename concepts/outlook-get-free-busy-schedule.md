# <a name="get-freebusy-schedule-for-users-and-resources-preview"></a><span data-ttu-id="ecd7d-101">Abrufen von Frei/Gebucht-Informationen für Benutzer und Ressourcen (Preview)</span><span class="sxs-lookup"><span data-stu-id="ecd7d-101">Get free/busy schedule for users and resources (preview)</span></span>

<span data-ttu-id="ecd7d-102">In einer Arbeits- oder Schulumgebung ist es üblich, zu schauen, wann ein Benutzer für eine Besprechung frei ist oder die Verfügbarkeit eines Teams, eines Raums oder einer Ausrüstung für einen bestimmten Zeitraum zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-102">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="ecd7d-103">Mit der Aktion [getSchedule](../api-reference/beta/api/calendar_getschedule.md) erhalten Sie die Verfügbarkeitsinformationen einer oder mehrerer Entitäten - Benutzer, Verteilerlisten oder Ressourcen - für einen bestimmten Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-103">The [getSchedule](../api-reference/beta/api/calendar_getschedule.md) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="ecd7d-104">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ecd7d-104">Example</span></span>

<span data-ttu-id="ecd7d-105">Ein einfaches Beispiel ist der Frei/Gebucht-Zeitplan eines Mitarbeiters, Alex, an einem bestimmten Tag, von 9 bis 18 Uhr, Pacitfic Standard Time:</span><span class="sxs-lookup"><span data-stu-id="ecd7d-105">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "Schedules": ["AlexW@contoso.OnMicrosoft.com"],
    "StartTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "EndTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

<span data-ttu-id="ecd7d-106">**getSchedule** gibt zwei Zeitplaneinträge zurück, die mit den vorhandenen Ereignissen im Standardkalender von Alex übereinstimmen und die Start- und Endzeiten der einzelnen Ereignisse sowie deren Frei/Gebucht-Status anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-106">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="ecd7d-107">Sie können davon ausgehen, dass Alex für die verbleibende Zeit in diesem Datums-/Zeitbereich frei ist.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-107">You can assume Alex is free for the remaining time in that date/time range.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        }
    ]
}

```

<span data-ttu-id="ecd7d-108">Abgesehen von dem Frei/Gebucht-Zeitplan und den Arbeitszeiten von Alex gibt **getSchedule** auch **AvailabilityView** zurück. Dabei handelt es sich um eine zusammengefasste Ansicht der Verfügbarkeit von Alex für diesen Tag.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-108">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="ecd7d-109">Die zusammengeführte Ansicht ist eine Zeichenkette, die aus Zeitfenstern besteht, die diesen Tag abdecken, wobei jedes Zeitfenster die Verfügbarkeit von Alex gemäß der folgenden Konvention anzeigt:</span><span class="sxs-lookup"><span data-stu-id="ecd7d-109">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="ecd7d-110">`0`= Frei</span><span class="sxs-lookup"><span data-stu-id="ecd7d-110">`0`= free</span></span>
- <span data-ttu-id="ecd7d-111">`1`= mit Vorbehalt</span><span class="sxs-lookup"><span data-stu-id="ecd7d-111">`1`= tentative</span></span>
- <span data-ttu-id="ecd7d-112">`2`= Gebucht</span><span class="sxs-lookup"><span data-stu-id="ecd7d-112">`2`= busy</span></span>
- <span data-ttu-id="ecd7d-113">`3`= Abwesend</span><span class="sxs-lookup"><span data-stu-id="ecd7d-113">`3`= out of office</span></span>
- <span data-ttu-id="ecd7d-114">`4`= an anderer Stelle arbeiten.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-114">`4`= working elsewhere.</span></span> 

<span data-ttu-id="ecd7d-115">Standardmäßig beträgt die Länge der einzelnen Zeitfenster 30 Minuten.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-115">Specifies the length of each time slot in minutes. Default is 30 minutes.</span></span> <span data-ttu-id="ecd7d-116">Dieses Beispiel verwendet die Eigenschaft **availabilityViewInterval**, um das Zeitfenster auf 15 Minuten einzustellen.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-116">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="ecd7d-117">Wie unterscheidet sich getSchedule von findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="ecd7d-117">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="ecd7d-118">Die Aktion [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) ähnelt der Aktion **getSchedule**, da sowohl der Frei/Gebucht-Status als auch die Arbeitszeiten der angegebenen Benutzer und Ressourcen ausgelesen werden.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-118">The [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="ecd7d-119">Die beiden Aktionen unterscheiden sich in einigen wesentlichen Punkten.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-119">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="ecd7d-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ecd7d-120">Application</span></span>

<span data-ttu-id="ecd7d-121">**findMeetingTimes** wendet bestimmte Geschäftslogiken an, um Besprechungszeiten und -orte vorzuschlagen, wie zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ecd7d-121">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="ecd7d-122">Optionale oder obligatorische Teilnahme jeder Entität</span><span class="sxs-lookup"><span data-stu-id="ecd7d-122">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="ecd7d-123">Die Art der gewünschten Aktivität zur Tageszeit</span><span class="sxs-lookup"><span data-stu-id="ecd7d-123">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="ecd7d-124">Die für die Beschlussfähigkeit einer Besprechung erforderliche Mindestteilnehmerzahl</span><span class="sxs-lookup"><span data-stu-id="ecd7d-124">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="ecd7d-125">Sie empfiehlt sich für Szenarien, die von der [Optimierung der Terminbuchung](findmeetingtimes_example.md) abhängig sind.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-125">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes_example.md).</span></span>

<span data-ttu-id="ecd7d-126">**getSchedule** gibt lediglich den Frei/Gebucht-Status vorhandener Ereignisse in jedem der angeforderten Kalender für einen bestimmten Zeitraum zurück und nimmt an, dass die restliche Zeit in diesem Zeitraum TP frei ist.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-126">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="ecd7d-127">Um diese Daten zur Vervollständigung Ihres Szenarios zu nutzen, wenden Sie weitere Geschäftslogiken an.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-127">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="ecd7d-128">Nur-App-Support</span><span class="sxs-lookup"><span data-stu-id="ecd7d-128">App-only support</span></span>

<span data-ttu-id="ecd7d-129">**findmeetingtimes** unterstützt nur solche delegierten Szenarien, bei denen ein Benutzer sich in der App angemeldet haben muss.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-129">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="ecd7d-130">Die App kann Ereignisse nur in den Kalendern lesen, auf die der angemeldete Benutzer zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-130">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="ecd7d-131">Dies kann Kalender beinhalten, die andere Benutzer delegiert oder mit dem angemeldeten Benutzer geteilt haben.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-131">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="ecd7d-132">**getSchedule** unterstützt sowohl delegierte als auch Nur-App-Szenarien.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-132">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="ecd7d-133">Im letzteren Fall erteilt ein Administrator der App die Erlaubnis, den Zugriff auf alle Kalender ohne angemeldeten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-133">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="ecd7d-134">Versionsunterstützung</span><span class="sxs-lookup"><span data-stu-id="ecd7d-134">Version support</span></span>

<span data-ttu-id="ecd7d-135">**findmeetingtimes** ist in der Regel für alle Apps verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-135">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="ecd7d-136">**getSchedule** ist derzeit [in der Vorschauversion](versioning_and_support.md#beta-version) verfügbar und daher nicht für den Einsatz in Produktivanwendungen geeignet.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-136">**getSchedule** is currently available [in preview status](versioning_and_support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="ecd7d-137">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ecd7d-137">Permissions</span></span>
<span data-ttu-id="ecd7d-138">Die niedrigste Berechtigung, die Sie benötigen, um Frei/Gebucht-Informationen zu erhalten, ist Calendar.Read.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-138">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="ecd7d-139">Abhängig von Ihrem App-Szenario kann dies vom angemeldeten Benutzer oder Administrator genehmigt werden.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-139">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="ecd7d-140">Abgesehen vom Frei/Gebucht-Status und den Arbeitszeiten der angeforderten Entitäten kann **getSchedule** auch den Inhalt und den Ort eines Ereignisses unter folgenden Bedingungen zurückgeben:</span><span class="sxs-lookup"><span data-stu-id="ecd7d-140">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="ecd7d-141">Wenn das Ereignis mit niedriger Vertraulichkeitsstufe gekennzeichnet ist - `normal` oder `personal` UND eine oder mehrere der folgenden Bedingungen zutrifft/zutreffen:</span><span class="sxs-lookup"><span data-stu-id="ecd7d-141">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="ecd7d-142">Die Kalendereinstellungen des angeforderten Benutzers erlauben es allen Benutzern in der Organisation, Titel und Orte anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="ecd7d-142">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="ecd7d-143">Der Kalender des angeforderten Benutzers wird mit dem angemeldeten Benutzer geteilt</span><span class="sxs-lookup"><span data-stu-id="ecd7d-143">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="ecd7d-144">Der angemeldete Benutzer ist ein Administrator der gleichen Organisation wie der angeforderte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-144">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="ecd7d-145">Zeitzonendarstellung</span><span class="sxs-lookup"><span data-stu-id="ecd7d-145">Time zone representation</span></span>
<span data-ttu-id="ecd7d-146">Standardmäßig werden die Anfangs- und Endzeiten der zurückgegebenen Elemente des Zeitplans in UTC dargestellt.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-146">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="ecd7d-147">Sie können einen `Prefer` Header verwenden, um eine für Ihre App passende Zeitzone anzugeben.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-147">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="ecd7d-148">Dazu folgendes Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ecd7d-148">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="ecd7d-149">Grenzwerte und Fehlerzustände</span><span class="sxs-lookup"><span data-stu-id="ecd7d-149">Limits and error conditions</span></span>
<span data-ttu-id="ecd7d-150">Beachten Sie die folgenden Grenzwerte und Fehlerzustände:</span><span class="sxs-lookup"><span data-stu-id="ecd7d-150">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="ecd7d-151">**getSchedule** unterstützt die Suche nach Frei/Gebucht-Informationen für bis zu 20 Objekte gleichzeitig.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-151">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="ecd7d-152">Diese Begrenzung gilt sowohl für die Anzahl der einzeln oder als Mitglieder einer Verteilerliste identifizierten Benutzer als auch für die Anzahl der Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-152">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="ecd7d-153">Der Suchzeitraum muss weniger als 42 Tage betragen.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-153">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="ecd7d-154">Wenn **getSchedule** einen bestimmten Benutzer oder eine bestimmte Ressource nicht identifizieren kann, wird ein einzelnes Zeitplan-Element zurückgegeben und der Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ecd7d-154">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="ecd7d-155">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ecd7d-155">See also</span></span>
- [<span data-ttu-id="ecd7d-156">Verweis auf Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ecd7d-156">Permissions reference</span></span>](permissions_reference.md#calendars-permissions)
- [<span data-ttu-id="ecd7d-157">Suchen nach möglichen Besprechungszeiten im Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="ecd7d-157">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes_example.md)

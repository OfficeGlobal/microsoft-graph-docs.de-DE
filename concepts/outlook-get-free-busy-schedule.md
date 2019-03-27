---
title: Abrufen des Frei/Gebucht-Zeitplans für Benutzer und Ressourcen,
description: Ein häufiges Szenario in einer Arbeits- oder Schulumgebung besteht darin, anzuzeigen, wann ein Benutzer für eine Besprechung verfügbar ist, oder die Verfügbarkeit eines Teams, Raums oder Geräts für einen Zeitraum zu durchsuchen.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 8ecf31ec74327d4f5fbd9d585eef24fcaec60709
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869197"
---
# <a name="get-freebusy-schedule-of-users-and-resources"></a><span data-ttu-id="c8643-103">Abrufen des Frei/Gebucht-Zeitplans für Benutzer und Ressourcen,</span><span class="sxs-lookup"><span data-stu-id="c8643-103">Get free/busy schedule of users and resources (preview)</span></span>

<span data-ttu-id="c8643-104">Ein häufiges Szenario in einer Arbeits- oder Schulumgebung besteht darin, anzuzeigen, wann ein Benutzer für eine Besprechung verfügbar ist, oder die Verfügbarkeit eines Teams, Raums oder Geräts für einen Zeitraum zu durchsuchen.</span><span class="sxs-lookup"><span data-stu-id="c8643-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="c8643-105">Mit der [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0)-Aktion können Sie die Verfügbarkeitsinformationen einer oder mehrerer Entitäten (Benutzer, Verteilerlisten oder Ressourcen) für einen bestimmten Zeitraum abrufen.</span><span class="sxs-lookup"><span data-stu-id="c8643-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="c8643-106">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8643-106">Example</span></span>

<span data-ttu-id="c8643-107">Ein einfach Beispiel ist das Suchen des Frei/Gebucht-Zeitplans eines Mitarbeiters Alex an einem bestimmten Tag von 9 Uhr bis 18 Uhr, Pacific Standard Time:</span><span class="sxs-lookup"><span data-stu-id="c8643-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacific Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/getschedule 
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

<span data-ttu-id="c8643-108">**getSchedule** gibt zwei Zeitplanelemente zurück, die vorhandenen Ereignissen in dem Standardkalender von Alex entsprechen; es werden die Start- und Endzeiten der einzelnen Ereignisse sowie der Frei/Gebucht-Status angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c8643-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="c8643-109">Sie können davon ausgehen, dass Alex die verbleibende Zeit in diesem Datums-/Uhrzeitbereich verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="c8643-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
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

<span data-ttu-id="c8643-110">Unabhängig vom Frei/Gebucht-Zeitplan und den Arbeitszeiten von Alex gibt **getSchedule** auch **availabilityView** zurück, eine zusammengeführte Ansicht der Verfügbarkeit von Alex an diesem Tag.</span><span class="sxs-lookup"><span data-stu-id="c8643-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="c8643-111">Die zusammengeführte Ansicht ist eine Zeichenfolge, die aus Zeitfenstern für diesen Tag besteht; jedes Zeitfenster gibt dabei die Verfügbarkeit von Alex mithilfe der folgenden Konvention an:</span><span class="sxs-lookup"><span data-stu-id="c8643-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="c8643-112">`0`= frei</span><span class="sxs-lookup"><span data-stu-id="c8643-112">`0`= free</span></span>
- <span data-ttu-id="c8643-113">`1`= mit Vorbehalt</span><span class="sxs-lookup"><span data-stu-id="c8643-113">`1`= tentative</span></span>
- <span data-ttu-id="c8643-114">`2`= gebucht</span><span class="sxs-lookup"><span data-stu-id="c8643-114">`2`= busy</span></span>
- <span data-ttu-id="c8643-115">`3`= abwesend</span><span class="sxs-lookup"><span data-stu-id="c8643-115">`3`= out of office</span></span>
- <span data-ttu-id="c8643-116">`4`= an anderem Ort tätig.</span><span class="sxs-lookup"><span data-stu-id="c8643-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="c8643-117">Standardmäßig beträgt die Länge der einzelnen Zeitfenster 30 Minuten.</span><span class="sxs-lookup"><span data-stu-id="c8643-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="c8643-118">Dieses Beispiel verwendet die **availabilityViewInterval**-Eigenschaft, um das Zeitfenster auf 15 Minuten zu ändern.</span><span class="sxs-lookup"><span data-stu-id="c8643-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a><span data-ttu-id="c8643-119">Worin unterscheiden sich getSchedule und findMeetingTimes?</span><span class="sxs-lookup"><span data-stu-id="c8643-119">How does getSchedule compare with findMeetingTimes</span></span>

<span data-ttu-id="c8643-120">Die [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)-Aktion ist dahingehend vergleichbar mit **getSchedule**, dass beide Aktionen den Frei/Gebucht-Status und die Arbeitszeiten der angegebenen Benutzer und Ressourcen lesen.</span><span class="sxs-lookup"><span data-stu-id="c8643-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="c8643-121">Die beiden Aktionen unterscheiden sich in einigen anderen wichtigen Aspekten.</span><span class="sxs-lookup"><span data-stu-id="c8643-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="c8643-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8643-122">Application</span></span>

<span data-ttu-id="c8643-123">**findMeetingTimes** wendet eine bestimmte Geschäftslogik an, um Besprechungszeiten und Orte vorzuschlagen, z. B.:</span><span class="sxs-lookup"><span data-stu-id="c8643-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="c8643-124">Optionale oder obligatorische Teilnahme der einzelnen Entitäten.</span><span class="sxs-lookup"><span data-stu-id="c8643-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="c8643-125">Die Art der angeforderten Aktivität für die Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="c8643-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="c8643-126">Die Mindestteilnehmeranzahl, die für ein Quorum für eine Besprechung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c8643-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="c8643-127">Dies eignet sich für Szenarien, die von [einer optimierten Terminbuchung](findmeetingtimes-example.md) abhängig sind.</span><span class="sxs-lookup"><span data-stu-id="c8643-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="c8643-128">**getSchedule** gibt einfach der Frei/Gebucht-Status der vorhandenen Ereignisse in jedem der angeforderten Kalender für einen bestimmten Zeitraum zurück und geht davon aus, dass die verbleibende Zeit in diesem Zeitraum frei ist.</span><span class="sxs-lookup"><span data-stu-id="c8643-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="c8643-129">Dann wird weitere Geschäftslogik angewendet, um diese Daten zur Vervollständigung Ihres Szenarios zu nutzen.</span><span class="sxs-lookup"><span data-stu-id="c8643-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="c8643-130">Nur-App-Support</span><span class="sxs-lookup"><span data-stu-id="c8643-130">App-only support</span></span>

<span data-ttu-id="c8643-131">**findmeetingtimes** unterstützt nur delegierte Szenarien, in denen sich ein Benutzer bei der App angemeldet haben muss.</span><span class="sxs-lookup"><span data-stu-id="c8643-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="c8643-132">Die App kann Ereignisse nur in den Kalendern lesen, auf die der angemeldete Benutzer zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="c8643-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="c8643-133">Dazu zählen Kalender, die andere Benutzer delegiert oder für den angemeldeten Benutzer freigegeben haben.</span><span class="sxs-lookup"><span data-stu-id="c8643-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="c8643-134">**getSchedule** unterstützt sowohl delegierte als auch Nur-App-Szenarien.</span><span class="sxs-lookup"><span data-stu-id="c8643-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="c8643-135">Bei letzterem stimmt ein Administrator zu, dass die App auf alle Kalender ohne einen angemeldeten Benutzer zugreift.</span><span class="sxs-lookup"><span data-stu-id="c8643-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>

### <a name="permissions"></a><span data-ttu-id="c8643-136">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8643-136">Permissions</span></span>
<span data-ttu-id="c8643-137">"Calendars.Read.Shared" ist die niedrigste Berechtigung, die von **findmeetingtimes** benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="c8643-137">The least privileged permissions required by **findmeetingtimes** is Calendars.Read.Shared.</span></span>

<span data-ttu-id="c8643-138">"Calendar.Read" ist die niedrigste Berechtigung, die von **getSchedule** benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="c8643-138">The least privileged permission required by **getSchedule** is Calendar.Read.</span></span> 

### <a name="version-support"></a><span data-ttu-id="c8643-139">Versionsunterstützung</span><span class="sxs-lookup"><span data-stu-id="c8643-139">Version support</span></span>

<span data-ttu-id="c8643-140">**findmeetingtimes** und **getSchedule** sind sowohl allgemein verfügbar als auch für den Einsatz in Produktionsanwendungen geeignet.</span><span class="sxs-lookup"><span data-stu-id="c8643-140">**findmeetingtimes** and **getSchedule** are both generally available and appropriate for use in production apps.</span></span>


## <a name="event-data-returned"></a><span data-ttu-id="c8643-141">Zurückgegebene Ereignisdaten</span><span class="sxs-lookup"><span data-stu-id="c8643-141">Event data returned</span></span>
<span data-ttu-id="c8643-142">"Calendar.Read" ist die niedrigste Berechtigung, die von **getSchedule** zum Abrufen von Frei/Gebucht-Informationen durch eine App benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="c8643-142">The least privileged permission required by **getSchedule** for an app to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="c8643-143">Je nach App-Szenario kann der angemeldete Benutzer oder der Administrator zustimmen.</span><span class="sxs-lookup"><span data-stu-id="c8643-143">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>

<span data-ttu-id="c8643-144">Während die genehmigte Berechtigung es einer App erlaubt, **getSchedule** auf den Kalendern der angeforderten Benutzer über Outlook zu verwenden, steuert der angeforderte Benutzer, welche Ereignisdaten, falls vorhanden, von **getSchedule** zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c8643-144">While the consented permission lets an app use **getSchedule** on the requested users' calendars, through Outlook, the requested user controls which event data, if any, that **getSchedule** returns.</span></span> 

<span data-ttu-id="c8643-145">Beispielsweise kann **getSchedule** den Frei/Belegt-Status und die Arbeitszeiten der angeforderten Benutzer oder auch die Eigenschaften **subject**, **location** und **isPrivate** eines Ereignisses zurückgeben, vorausgesetzt, dass:</span><span class="sxs-lookup"><span data-stu-id="c8643-145">For example, **getSchedule** can return the free/busy status and working hours of the requested users, or it can also return the **subject**, **location**, and **isPrivate** properties of an event, provided that:</span></span>

- <span data-ttu-id="c8643-146">Das Ereignis mit geringer Vertraulichkeitsstufe markiert ist (`normal` oder `personal`) UND eine oder mehrere der folgenden Bedingungen zutreffen:</span><span class="sxs-lookup"><span data-stu-id="c8643-146">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

   - <span data-ttu-id="c8643-147">Die Kalendereinstellungen des angeforderten Benutzers erlauben es dem angemeldeten Benutzer, Betreffzeilen und Orte anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="c8643-147">The requested user’s calendar settings allow the signed-in user to view subject lines and locations</span></span>
   - <span data-ttu-id="c8643-148">Der Kalender des angeforderten Benutzers ist für den angemeldeten Benutzer freigegeben.</span><span class="sxs-lookup"><span data-stu-id="c8643-148">The requested user’s calendar is shared with the signed-in user</span></span>

<span data-ttu-id="c8643-149">Diese Bedingungen gelten unabhängig davon, ob der angemeldete Benutzer ein Administrator in der Organisation ist.</span><span class="sxs-lookup"><span data-stu-id="c8643-149">These conditions apply regardless of whether the signed-in user is an administrator in the organization.</span></span> <span data-ttu-id="c8643-150">Der angeforderte Benutzer hat die Kontrolle über die zurückgegebenen Ereignisdaten.</span><span class="sxs-lookup"><span data-stu-id="c8643-150">The requested user has control over the event data returned.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="c8643-151">Zeitzonendarstellung</span><span class="sxs-lookup"><span data-stu-id="c8643-151">Time zone representation</span></span>
<span data-ttu-id="c8643-152">Standardmäßig werden die Start- und Endzeiten der zurückgegebenen Zeitplanelemente in UTC dargestellt.</span><span class="sxs-lookup"><span data-stu-id="c8643-152">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="c8643-153">Sie können eine `Prefer`-Kopfzeile verwenden, um eine für Ihre App geeignete Zeitzone anzugeben.</span><span class="sxs-lookup"><span data-stu-id="c8643-153">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="c8643-154">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c8643-154">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="c8643-155">Beschränkungen und Fehlerursachen</span><span class="sxs-lookup"><span data-stu-id="c8643-155">Limits and error conditions</span></span>
<span data-ttu-id="c8643-156">Beachten Sie die folgenden Beschränkungen und Fehlerbedingungen:</span><span class="sxs-lookup"><span data-stu-id="c8643-156">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="c8643-157">**getSchedule** kann das Nachschlagen von Frei/Gebucht-Informationen für bis zu 20 Entitäten gleichzeitig unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c8643-157">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="c8643-158">Dieser Grenzwert gilt für die Anzahl von Benutzern, die einzeln oder als Mitglieder einer Verteilerliste identifiziert wurden, und auch für die Anzahl von Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="c8643-158">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="c8643-159">Der Zeitraum zum Nachschlagen muss weniger als 42 Tage betragen.</span><span class="sxs-lookup"><span data-stu-id="c8643-159">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="c8643-160">Wenn **getSchedule** keinen angegebenen Benutzer oder keine angegebene Ressource identifizieren kann, wird ein einzelnes Zeitplanelement zurückgegeben und der Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c8643-160">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 


## <a name="see-also"></a><span data-ttu-id="c8643-161">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="c8643-161">See also</span></span>
- [<span data-ttu-id="c8643-162">Berechtigungsreferenz</span><span class="sxs-lookup"><span data-stu-id="c8643-162">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="c8643-163">Suchen nach möglichen Besprechungszeiten im Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="c8643-163">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)

---
title: Abrufen des Frei/Gebucht-Zeitplans für Benutzer und Ressourcen (Vorschau)
description: Ein häufiges Szenario in einer Arbeits- oder Schulumgebung besteht darin, anzuzeigen, wann ein Benutzer für eine Besprechung verfügbar ist, oder die Verfügbarkeit eines Teams, Raums oder Geräts für einen Zeitraum zu durchsuchen.
ms.openlocfilehash: 8a2dd9318bdd806c99d525ee41f46d78d1963b47
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092304"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="ba027-103">Abrufen des Frei/Gebucht-Zeitplans für Benutzer und Ressourcen (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="ba027-103">Get free/busy schedule of users and resources (preview)</span></span>

<span data-ttu-id="ba027-104">Ein häufiges Szenario in einer Arbeits- oder Schulumgebung besteht darin, anzuzeigen, wann ein Benutzer für eine Besprechung verfügbar ist, oder die Verfügbarkeit eines Teams, Raums oder Geräts für einen Zeitraum zu durchsuchen.</span><span class="sxs-lookup"><span data-stu-id="ba027-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="ba027-105">Mit der [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta)-Aktion können Sie die Verfügbarkeitsinformationen einer oder mehrerer Entitäten (Benutzer, Verteilerlisten oder Ressourcen) für einen bestimmten Zeitraum abrufen.</span><span class="sxs-lookup"><span data-stu-id="ba027-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="ba027-106">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba027-106">Example</span></span>

<span data-ttu-id="ba027-107">Ein einfach Beispiel ist das Suchen des Frei/Gebucht-Zeitplans eines Mitarbeiters Alex an einem bestimmten Tag von 9 Uhr bis 18 Uhr, Pacific Standard Time:</span><span class="sxs-lookup"><span data-stu-id="ba027-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

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

<span data-ttu-id="ba027-108">**getSchedule** gibt zwei Zeitplanelemente zurück, die vorhandenen Ereignissen in dem Standardkalender von Alex entsprechen; es werden die Start- und Endzeiten der einzelnen Ereignisse sowie der Frei/Gebucht-Status angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ba027-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="ba027-109">Sie können davon ausgehen, dass Alex die verbleibende Zeit in diesem Datums-/Uhrzeitbereich verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="ba027-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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

<span data-ttu-id="ba027-110">Unabhängig vom Frei/Gebucht-Zeitplan und den Arbeitszeiten von Alex gibt **getSchedule** auch **availabilityView** zurück, eine zusammengeführte Ansicht der Verfügbarkeit von Alex an diesem Tag.</span><span class="sxs-lookup"><span data-stu-id="ba027-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="ba027-111">Die zusammengeführte Ansicht ist eine Zeichenfolge, die aus Zeitfenstern für diesen Tag besteht; jedes Zeitfenster gibt dabei die Verfügbarkeit von Alex mithilfe der folgenden Konvention an:</span><span class="sxs-lookup"><span data-stu-id="ba027-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="ba027-112">`0`= frei</span><span class="sxs-lookup"><span data-stu-id="ba027-112">`0`= free</span></span>
- <span data-ttu-id="ba027-113">`1`= mit Vorbehalt</span><span class="sxs-lookup"><span data-stu-id="ba027-113">`1`= tentative</span></span>
- <span data-ttu-id="ba027-114">`2`= gebucht</span><span class="sxs-lookup"><span data-stu-id="ba027-114">`2`= busy</span></span>
- <span data-ttu-id="ba027-115">`3`= abwesend</span><span class="sxs-lookup"><span data-stu-id="ba027-115">`3`= out of office</span></span>
- <span data-ttu-id="ba027-116">`4`= an anderem Ort tätig.</span><span class="sxs-lookup"><span data-stu-id="ba027-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="ba027-117">Standardmäßig beträgt die Länge der einzelnen Zeitfenster 30 Minuten.</span><span class="sxs-lookup"><span data-stu-id="ba027-117">Specifies the length of each time slot in minutes. Default is 30 minutes.</span></span> <span data-ttu-id="ba027-118">Dieses Beispiel verwendet die **availabilityViewInterval**-Eigenschaft, um das Zeitfenster auf 15 Minuten zu ändern.</span><span class="sxs-lookup"><span data-stu-id="ba027-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="ba027-119">Inwiefern unterscheidet sich getSchedule von FindMeetingTimes?</span><span class="sxs-lookup"><span data-stu-id="ba027-119">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="ba027-120">Die [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)-Aktion ist dahingehend vergleichbar mit **getSchedule**, dass beide Aktionen den Frei/Gebucht-Status und die Arbeitszeiten der angegebenen Benutzer und Ressourcen lesen.</span><span class="sxs-lookup"><span data-stu-id="ba027-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="ba027-121">Die beiden Aktionen unterscheiden sich in einigen anderen wichtigen Aspekten.</span><span class="sxs-lookup"><span data-stu-id="ba027-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="ba027-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba027-122">Application</span></span>

<span data-ttu-id="ba027-123">**findMeetingTimes** wendet eine bestimmte Geschäftslogik an, um Besprechungszeiten und Orte vorzuschlagen, z. B.:</span><span class="sxs-lookup"><span data-stu-id="ba027-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="ba027-124">Optionale oder obligatorische Teilnahme der einzelnen Entitäten.</span><span class="sxs-lookup"><span data-stu-id="ba027-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="ba027-125">Die Art der angeforderten Aktivität für die Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="ba027-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="ba027-126">Die Mindestteilnehmeranzahl, die für ein Quorum für eine Besprechung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ba027-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="ba027-127">Dies eignet sich für Szenarien, die von [einer optimierten Terminbuchung](findmeetingtimes-example.md) abhängig sind.</span><span class="sxs-lookup"><span data-stu-id="ba027-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="ba027-128">**getSchedule** gibt einfach der Frei/Gebucht-Status der vorhandenen Ereignisse in jedem der angeforderten Kalender für einen bestimmten Zeitraum zurück und geht davon aus, dass die verbleibende Zeit in diesem Zeitraum frei ist.</span><span class="sxs-lookup"><span data-stu-id="ba027-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="ba027-129">Dann wird weitere Geschäftslogik angewendet, um diese Daten zur Vervollständigung Ihres Szenarios zu nutzen.</span><span class="sxs-lookup"><span data-stu-id="ba027-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="ba027-130">Nur-App-Support</span><span class="sxs-lookup"><span data-stu-id="ba027-130">App-only support</span></span>

<span data-ttu-id="ba027-131">**findmeetingtimes** unterstützt nur delegierte Szenarien, in denen sich ein Benutzer bei der App angemeldet haben muss.</span><span class="sxs-lookup"><span data-stu-id="ba027-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="ba027-132">Die App kann Ereignisse nur in den Kalendern lesen, auf die der angemeldete Benutzer zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="ba027-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="ba027-133">Dazu zählen Kalender, die andere Benutzer delegiert oder für den angemeldeten Benutzer freigegeben haben.</span><span class="sxs-lookup"><span data-stu-id="ba027-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="ba027-134">**getSchedule** unterstützt sowohl delegierte als auch Nur-App-Szenarien.</span><span class="sxs-lookup"><span data-stu-id="ba027-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="ba027-135">Bei letzterem stimmt ein Administrator zu, dass die App auf alle Kalender ohne einen angemeldeten Benutzer zugreift.</span><span class="sxs-lookup"><span data-stu-id="ba027-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="ba027-136">Versionsunterstützung</span><span class="sxs-lookup"><span data-stu-id="ba027-136">Version support</span></span>

<span data-ttu-id="ba027-137">**findmeetingtimes** ist allgemein für alle Apps verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ba027-137">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="ba027-138">**getSchedule** ist derzeit im [Vorschaustatus](versioning-and-support.md#beta-version) verfügbar und ist daher nicht zur Verwendung in Produktions-Apps geeignet.</span><span class="sxs-lookup"><span data-stu-id="ba027-138">**getSchedule** is currently available [in preview status](versioning-and-support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="ba027-139">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ba027-139">Permissions</span></span>
<span data-ttu-id="ba027-140">Calendar.Read ist die niedrigste Berechtigung, die Sie zum Abrufen von Frei/Gebucht-Informationen benötigen.</span><span class="sxs-lookup"><span data-stu-id="ba027-140">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="ba027-141">Je nach App-Szenario kann der angemeldete Benutzer oder der Administrator zustimmen.</span><span class="sxs-lookup"><span data-stu-id="ba027-141">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="ba027-142">Neben dem Frei/Gebucht-Status und den Arbeitszeiten der angeforderten Entitäten kann **getSchedule** unter den folgenden Voraussetzungen auch den Betreff und den Ort eines Ereignisses zurückgeben:</span><span class="sxs-lookup"><span data-stu-id="ba027-142">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="ba027-143">Wenn das Ereignis mit geringer Vertraulichkeitsstufe markiert ist: `normal` oder `personal`, UND eine oder mehrere der folgenden Bedingungen treffen zu:</span><span class="sxs-lookup"><span data-stu-id="ba027-143">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="ba027-144">Die Kalendereinstellungen des angeforderten Benutzers ermöglichen allen Benutzern in der Organisation, Titel und Orte anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="ba027-144">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="ba027-145">Der Kalender des angeforderten Benutzers ist für den angemeldeten Benutzer freigegeben.</span><span class="sxs-lookup"><span data-stu-id="ba027-145">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="ba027-146">Der angemeldete Benutzer ist ein Administrator derselben Organisation wie der angeforderte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ba027-146">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="ba027-147">Zeitzonendarstellung</span><span class="sxs-lookup"><span data-stu-id="ba027-147">Time zone representation</span></span>
<span data-ttu-id="ba027-148">Standardmäßig werden die Start- und Endzeiten der zurückgegebenen Zeitplanelemente in UTC dargestellt.</span><span class="sxs-lookup"><span data-stu-id="ba027-148">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="ba027-149">Sie können eine `Prefer`-Kopfzeile verwenden, um eine für Ihre App geeignete Zeitzone anzugeben.</span><span class="sxs-lookup"><span data-stu-id="ba027-149">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="ba027-150">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ba027-150">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="ba027-151">Beschränkungen und Fehlerursachen</span><span class="sxs-lookup"><span data-stu-id="ba027-151">Limits and error conditions</span></span>
<span data-ttu-id="ba027-152">Beachten Sie die folgenden Beschränkungen und Fehlerbedingungen:</span><span class="sxs-lookup"><span data-stu-id="ba027-152">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="ba027-153">**getSchedule** kann das Nachschlagen von Frei/Gebucht-Informationen für bis zu 20 Entitäten gleichzeitig unterstützen.</span><span class="sxs-lookup"><span data-stu-id="ba027-153">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="ba027-154">Dieser Grenzwert gilt für die Anzahl von Benutzern, die einzeln oder als Mitglieder einer Verteilerliste identifiziert wurden, und auch für die Anzahl von Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="ba027-154">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="ba027-155">Der Zeitraum zum Nachschlagen muss weniger als 42 Tage betragen.</span><span class="sxs-lookup"><span data-stu-id="ba027-155">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="ba027-156">Wenn **getSchedule** keinen angegebenen Benutzer oder keine angegebene Ressource identifizieren kann, wird ein einzelnes Zeitplanelement zurückgegeben und der Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ba027-156">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="ba027-157">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ba027-157">See also</span></span>
- [<span data-ttu-id="ba027-158">Berechtigungsreferenz</span><span class="sxs-lookup"><span data-stu-id="ba027-158">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="ba027-159">Suchen nach möglichen Besprechungszeiten im Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="ba027-159">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)

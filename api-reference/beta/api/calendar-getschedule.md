---
title: 'Kalender: GetSchedule'
description: Rufen Sie die Frei/Gebucht-Verfügbarkeitsinformationen für eine Auflistung von Benutzern, Verteilerlisten oder Ressourcen für einen angegebenen Zeitraum.
ms.openlocfilehash: 5122cf34530f18f872e80863f259f348193d252e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059680"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="3158c-103">Kalender: GetSchedule</span><span class="sxs-lookup"><span data-stu-id="3158c-103">calendar: getSchedule</span></span>

> <span data-ttu-id="3158c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3158c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3158c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3158c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3158c-106">Rufen Sie die Frei/Gebucht-Verfügbarkeitsinformationen für eine Auflistung von Benutzern, Verteilerlisten oder Ressourcen für einen angegebenen Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="3158c-106">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="3158c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3158c-107">Permissions</span></span>
<span data-ttu-id="3158c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3158c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3158c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3158c-110">Permission type</span></span>      | <span data-ttu-id="3158c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3158c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3158c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3158c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3158c-113">Calendar.Read Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3158c-113">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="3158c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3158c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3158c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3158c-115">Not supported.</span></span> |
|<span data-ttu-id="3158c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3158c-116">Application</span></span> | <span data-ttu-id="3158c-117">Calendar.Read Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3158c-117">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3158c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3158c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="3158c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3158c-119">Request headers</span></span>
| <span data-ttu-id="3158c-120">Name</span><span class="sxs-lookup"><span data-stu-id="3158c-120">Name</span></span>       | <span data-ttu-id="3158c-121">Typ</span><span class="sxs-lookup"><span data-stu-id="3158c-121">Type</span></span> | <span data-ttu-id="3158c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3158c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3158c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3158c-123">Authorization</span></span>  | <span data-ttu-id="3158c-124">string</span><span class="sxs-lookup"><span data-stu-id="3158c-124">string</span></span>  | <span data-ttu-id="3158c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3158c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3158c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3158c-127">Content-Type</span></span>  | <span data-ttu-id="3158c-128">string</span><span class="sxs-lookup"><span data-stu-id="3158c-128">string</span></span> | <span data-ttu-id="3158c-129">Die Art der Daten im Textkörper einer Entität, die Application/Json ist.</span><span class="sxs-lookup"><span data-stu-id="3158c-129">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="3158c-130">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3158c-130">Required.</span></span>  |
| <span data-ttu-id="3158c-131">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="3158c-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="3158c-132">string</span><span class="sxs-lookup"><span data-stu-id="3158c-132">string</span></span> | <span data-ttu-id="3158c-133">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="3158c-133">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="3158c-134">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3158c-134">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="3158c-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="3158c-135">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3158c-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3158c-136">Request body</span></span>
<span data-ttu-id="3158c-137">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="3158c-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3158c-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3158c-138">Property</span></span>     | <span data-ttu-id="3158c-139">Typ</span><span class="sxs-lookup"><span data-stu-id="3158c-139">Type</span></span>   |<span data-ttu-id="3158c-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3158c-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3158c-141">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="3158c-141">availabilityViewInterval</span></span>|<span data-ttu-id="3158c-142">String</span><span class="sxs-lookup"><span data-stu-id="3158c-142">String</span></span>|<span data-ttu-id="3158c-143">Stellt die Dauer der ein Zeitintervall in einer **AvailabilityView** in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3158c-143">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="3158c-144">Der Standardwert ist 30 Minuten, mindestens 6, Maximum liegt bei 1440.</span><span class="sxs-lookup"><span data-stu-id="3158c-144">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="3158c-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="3158c-145">Optional.</span></span>|
|<span data-ttu-id="3158c-146">endTime</span><span class="sxs-lookup"><span data-stu-id="3158c-146">endTime</span></span>|[<span data-ttu-id="3158c-147">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3158c-147">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3158c-148">Das Datum, Uhrzeit und Zeitzone, die die Periode endet.</span><span class="sxs-lookup"><span data-stu-id="3158c-148">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="3158c-149">Zeitpläne</span><span class="sxs-lookup"><span data-stu-id="3158c-149">schedules</span></span>|<span data-ttu-id="3158c-150">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="3158c-150">String collection</span></span>|<span data-ttu-id="3158c-151">Eine Auflistung von SMTP-Adressen von Benutzern, Verteilerlisten oder Ressourcen zum Abrufen von Verfügbarkeitsinformationen für.</span><span class="sxs-lookup"><span data-stu-id="3158c-151">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="3158c-152">startTime</span><span class="sxs-lookup"><span data-stu-id="3158c-152">startTime</span></span>|[<span data-ttu-id="3158c-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3158c-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3158c-154">Das Datum, Uhrzeit und Zeitzone, die der Zeitraum beginnt.</span><span class="sxs-lookup"><span data-stu-id="3158c-154">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="3158c-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="3158c-155">Response</span></span>

<span data-ttu-id="3158c-156">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von [ScheduleInformation](../resources/scheduleinformation.md) -Objekten für jedes Objekt in der `schedules` Parameter.</span><span class="sxs-lookup"><span data-stu-id="3158c-156">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="3158c-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3158c-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3158c-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3158c-158">Request</span></span>
<span data-ttu-id="3158c-159">Das folgende Beispiel ruft die Verfügbarkeitsinformationen für zwei Benutzer für den angegebenen Datum, Uhrzeit und Zeitzone ab.</span><span class="sxs-lookup"><span data-stu-id="3158c-159">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["AdeleV@contoso.onmicrosoft.com", "AlexW@contoso.OnMicrosoft.com"],
    "startTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

##### <a name="response"></a><span data-ttu-id="3158c-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="3158c-160">Response</span></span>
<span data-ttu-id="3158c-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3158c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
            "scheduleId":"AdeleV@contoso.onmicrosoft.com",
            "availabilityView":"222222000022000000000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
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
                    "subject":"Lunch yoga",
                    "location":"Courtyard",
                    "start":{
                        "dateTime":"2018-08-06T11:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T12:00:00.0000000",
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
        },
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
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
                    "subject":"Q4 planning",
                    "location":"Big Bear",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'Kalender: getSchedule'
description: Rufen Sie die Frei/Gebucht-Informationen zur Verfügbarkeit von Benutzern, Verteilerlisten oder Ressourcen für einen angegebenen Zeitraum ab.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0c2f6a54664242831d7fd3f2ddfc6a44984674e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530027"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="3e8e8-103">Kalender: getSchedule</span><span class="sxs-lookup"><span data-stu-id="3e8e8-103">calendar: getSchedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e8e8-104">Rufen Sie die Frei/Gebucht-Informationen zur Verfügbarkeit von Benutzern, Verteilerlisten oder Ressourcen für einen angegebenen Zeitraum ab.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-104">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e8e8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3e8e8-105">Permissions</span></span>
<span data-ttu-id="3e8e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e8e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e8e8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e8e8-108">Permission type</span></span>      | <span data-ttu-id="3e8e8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e8e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e8e8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e8e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e8e8-111">Calendar.Read, Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e8e8-111">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="3e8e8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e8e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e8e8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e8e8-113">Not supported.</span></span> |
|<span data-ttu-id="3e8e8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e8e8-114">Application</span></span> | <span data-ttu-id="3e8e8-115">Calendar.Read, Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e8e8-115">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e8e8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e8e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="3e8e8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e8e8-117">Request headers</span></span>
| <span data-ttu-id="3e8e8-118">Name</span><span class="sxs-lookup"><span data-stu-id="3e8e8-118">Name</span></span>       | <span data-ttu-id="3e8e8-119">Typ</span><span class="sxs-lookup"><span data-stu-id="3e8e8-119">Type</span></span> | <span data-ttu-id="3e8e8-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e8e8-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3e8e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e8e8-121">Authorization</span></span>  | <span data-ttu-id="3e8e8-122">string</span><span class="sxs-lookup"><span data-stu-id="3e8e8-122">string</span></span>  | <span data-ttu-id="3e8e8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e8e8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e8e8-125">Content-Type</span></span>  | <span data-ttu-id="3e8e8-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e8e8-126">string</span></span> | <span data-ttu-id="3e8e8-127">Die Art der Daten im Textkörper einer Entität, die Anwendung/JSON ist.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="3e8e8-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-128">Required.</span></span>  |
| <span data-ttu-id="3e8e8-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="3e8e8-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="3e8e8-130">string</span><span class="sxs-lookup"><span data-stu-id="3e8e8-130">string</span></span> | <span data-ttu-id="3e8e8-131">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="3e8e8-132">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="3e8e8-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e8e8-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e8e8-134">Request body</span></span>
<span data-ttu-id="3e8e8-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e8e8-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e8e8-136">Property</span></span>     | <span data-ttu-id="3e8e8-137">Typ</span><span class="sxs-lookup"><span data-stu-id="3e8e8-137">Type</span></span>   |<span data-ttu-id="3e8e8-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e8e8-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e8e8-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="3e8e8-139">availabilityViewInterval</span></span>|<span data-ttu-id="3e8e8-140">String</span><span class="sxs-lookup"><span data-stu-id="3e8e8-140">String</span></span>|<span data-ttu-id="3e8e8-141">Steht für die Dauer eines Zeitraums in einem **availabilityView**-Objekt in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="3e8e8-142">Die Standardeinstellung beträgt 30 Minuten, minimale Dauer liegt bei 6, maximale Dauer liegt bei 1440 Minuten.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="3e8e8-143">Optional.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-143">Optional.</span></span>|
|<span data-ttu-id="3e8e8-144">endTime</span><span class="sxs-lookup"><span data-stu-id="3e8e8-144">endTime</span></span>|[<span data-ttu-id="3e8e8-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e8e8-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3e8e8-146">Datum, Uhrzeit und Zeitzone für das Ende des Zeitraums.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="3e8e8-147">Terminpläne</span><span class="sxs-lookup"><span data-stu-id="3e8e8-147">schedules</span></span>|<span data-ttu-id="3e8e8-148">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3e8e8-148">String collection</span></span>|<span data-ttu-id="3e8e8-149">Eine Sammlung der SMTP-Adressen von Benutzern, Verteilerlisten oder Ressourcen, für die Verfügbarkeitsinformationen abgerufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="3e8e8-150">startTime</span><span class="sxs-lookup"><span data-stu-id="3e8e8-150">startTime</span></span>|[<span data-ttu-id="3e8e8-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e8e8-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="3e8e8-152">Datum, Uhrzeit und Zeitzone für den Beginn des Zeitraums.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="3e8e8-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e8e8-153">Response</span></span>

<span data-ttu-id="3e8e8-154">Bei erfolgreicher Ausführung gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von [scheduleInformation](../resources/scheduleinformation.md)-Objekten für jedes Objekt im `schedules`-Parameter zurück.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="3e8e8-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e8e8-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e8e8-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e8e8-156">Request</span></span>
<span data-ttu-id="3e8e8-157">Im folgenden Beispiel werden die Verfügbarkeitsinformationen für zwei Benutzer für das angegebene Datum, die angegebene Uhrzeit und Zeitzone abgerufen.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

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

##### <a name="response"></a><span data-ttu-id="3e8e8-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e8e8-158">Response</span></span>
<span data-ttu-id="3e8e8-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e8e8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-getschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

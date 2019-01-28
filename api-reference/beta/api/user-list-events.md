---
title: Ereignisse auflisten
description: 'Abrufen einer Liste von Ereignisobjekten aus dem Standardkalender des Benutzers oder '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef16f9f0db1bc1e489bc7322ff72f58598d8d0a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526662"
---
# <a name="list-events"></a><span data-ttu-id="6f84f-103">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="6f84f-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f84f-104">Abrufen einer Liste von [event](../resources/event.md)-Objekten aus dem Standardkalender des Benutzers oder einem angegebenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="6f84f-104">Get a list of [event](../resources/event.md) objects from the user's default calendar or from a specified calendar.</span></span> <span data-ttu-id="6f84f-105">Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.</span><span class="sxs-lookup"><span data-stu-id="6f84f-105">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="6f84f-106">Um erweiterte Ereignisinstanzen abzurufen, können Sie [die Kalenderansicht abrufen](calendar-list-calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="6f84f-106">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="6f84f-107">Es gibt zwei Szenarien, in denen eine App Ereignisse im Kalender eines anderen Benutzers abrufen kann:</span><span class="sxs-lookup"><span data-stu-id="6f84f-107">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="6f84f-108">Wenn die App Anwendungsberechtigungen besitzt oder</span><span class="sxs-lookup"><span data-stu-id="6f84f-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6f84f-109">Wenn die App die entsprechenden delegierten [Berechtigungen](#permissions) von einem Benutzer besitzt und ein anderer Benutzer einen Kalender für diesen Benutzer freigegeben hat oder diesem Benutzer delegierten Zugriff erteilt hat.</span><span class="sxs-lookup"><span data-stu-id="6f84f-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6f84f-110">Hier finden Sie [weitere Informationen und ein Beispiel](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="6f84f-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="6f84f-111">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="6f84f-111">Support various time zones</span></span>

<span data-ttu-id="6f84f-112">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="6f84f-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="6f84f-113">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6f84f-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="6f84f-p103">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="6f84f-117">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="6f84f-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f84f-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6f84f-118">Permissions</span></span>
<span data-ttu-id="6f84f-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f84f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f84f-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f84f-121">Permission type</span></span>      | <span data-ttu-id="6f84f-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f84f-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f84f-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f84f-123">Delegated (work or school account)</span></span> | <span data-ttu-id="6f84f-124">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f84f-124">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6f84f-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f84f-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f84f-126">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f84f-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6f84f-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f84f-127">Application</span></span> | <span data-ttu-id="6f84f-128">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f84f-128">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f84f-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f84f-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6f84f-130">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6f84f-130">Optional query parameters</span></span>
<span data-ttu-id="6f84f-131">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6f84f-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6f84f-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f84f-132">Request headers</span></span>
| <span data-ttu-id="6f84f-133">Name</span><span class="sxs-lookup"><span data-stu-id="6f84f-133">Name</span></span>       | <span data-ttu-id="6f84f-134">Typ</span><span class="sxs-lookup"><span data-stu-id="6f84f-134">Type</span></span> | <span data-ttu-id="6f84f-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f84f-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6f84f-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f84f-136">Authorization</span></span>  | <span data-ttu-id="6f84f-137">string</span><span class="sxs-lookup"><span data-stu-id="6f84f-137">string</span></span>  | <span data-ttu-id="6f84f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f84f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6f84f-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="6f84f-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="6f84f-141">string</span><span class="sxs-lookup"><span data-stu-id="6f84f-141">string</span></span> | <span data-ttu-id="6f84f-142">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="6f84f-143">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="6f84f-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="6f84f-144">Optional.</span></span> |
| <span data-ttu-id="6f84f-145">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="6f84f-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="6f84f-146">string</span><span class="sxs-lookup"><span data-stu-id="6f84f-146">string</span></span> | <span data-ttu-id="6f84f-147">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="6f84f-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="6f84f-148">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="6f84f-148">Values can be "text" or "html".</span></span> <span data-ttu-id="6f84f-149">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="6f84f-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="6f84f-150">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="6f84f-151">Optional.</span><span class="sxs-lookup"><span data-stu-id="6f84f-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f84f-152">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f84f-152">Request body</span></span>
<span data-ttu-id="6f84f-153">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6f84f-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f84f-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f84f-154">Response</span></span>

<span data-ttu-id="6f84f-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f84f-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f84f-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6f84f-157">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="6f84f-157">Request 1</span></span>
<span data-ttu-id="6f84f-158">Das erste Beispiel ruft alle Ereignisse des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="6f84f-158">The first example gets all the user's events.</span></span> <span data-ttu-id="6f84f-159">Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="6f84f-159">It specifies the following:</span></span>

- <span data-ttu-id="6f84f-160">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="6f84f-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="6f84f-p109">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="6f84f-163">Die Anforderung gibt keinen `Prefer: outlook.body-content-type`-Header an, um ein bestimmtes Format für den zurückgegebenen Ereignistext anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="6f84f-163">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="6f84f-164">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="6f84f-164">Response 1</span></span>
<span data-ttu-id="6f84f-165">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6f84f-165">Here is an example of the response.</span></span> <span data-ttu-id="6f84f-166">Da kein `Prefer: outlook.body-content-type`-Header angegeben wurde, wird die **body**-Eigenschaft im standardmäßigen HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-166">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1932

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"html",
                "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
            },
            "start":{
                "dateTime":"2017-04-21T10:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "end":{
                "dateTime":"2017-04-21T12:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "location": {
                "displayName": "Assembly Hall",
                "locationType": "default",
                "uniqueId": "Assembly Hall",
                "uniqueIdType": "private"
            },
            "locations": [
                {
                    "displayName": "Assembly Hall",
                    "locationType": "default",
                    "uniqueIdType": "unknown"
                }
            ],
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Samantha Booth",
                        "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Dana Swope",
                        "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                }
            }
        }
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="6f84f-167">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="6f84f-167">Request 2</span></span>
<span data-ttu-id="6f84f-168">Das zweite Beispiel veranschaulicht, wie Sie einen `Prefer: outlook.body-content-type="text"`-Header verwenden, um die **body**-Eigenschaft der angegebenen Nachricht im Textformat abzurufen.</span><span class="sxs-lookup"><span data-stu-id="6f84f-168">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>

<span data-ttu-id="6f84f-169">Die Anforderung verwendet auch einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="6f84f-169">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="6f84f-170">Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-170">Without a `$select` parameter, all of the event properties will be returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text" 
```
##### <a name="response-2"></a><span data-ttu-id="6f84f-171">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="6f84f-171">Response 2</span></span>
<span data-ttu-id="6f84f-172">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6f84f-172">Here is an example of the response.</span></span> <span data-ttu-id="6f84f-173">Die **body**-Eigenschaft wird im Textformat zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f84f-173">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 640

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

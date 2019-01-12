---
title: Ereignisse auflisten
description: 'Rufen Sie eine Liste der Ereignisobjekte im Postfach des Benutzers. Die Liste enthält die einzelnen '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b5e23391c434e2ace5a567bb23efe5539ad7aee5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946308"
---
# <a name="list-events"></a><span data-ttu-id="a1244-104">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="a1244-104">List events</span></span>

<span data-ttu-id="a1244-p102">Dient zum Abrufen einer Liste der [event](../resources/event.md)-Objekte im Postfach des Benutzers. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.</span><span class="sxs-lookup"><span data-stu-id="a1244-p102">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="a1244-107">Um erweiterte Ereignisinstanzen abzurufen, können Sie [die Kalenderansicht abrufen](calendar-list-calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="a1244-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="a1244-108">Zurzeit gibt dieser Vorgang Ereignistext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="a1244-108">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="a1244-109">Es gibt zwei Szenarien, in dem eine app Ereignisse im Kalender des Benutzers abzurufen:</span><span class="sxs-lookup"><span data-stu-id="a1244-109">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="a1244-110">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="a1244-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a1244-111">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen Kalender freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="a1244-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a1244-112">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="a1244-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="a1244-113">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="a1244-113">Support various time zones</span></span>

<span data-ttu-id="a1244-114">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="a1244-114">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="a1244-115">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="a1244-115">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="a1244-p104">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1244-p104">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="a1244-119">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="a1244-119">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1244-120">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a1244-120">Permissions</span></span>
<span data-ttu-id="a1244-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1244-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1244-123">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1244-123">Permission type</span></span>      | <span data-ttu-id="a1244-124">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1244-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1244-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1244-125">Delegated (work or school account)</span></span> | <span data-ttu-id="a1244-126">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1244-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a1244-127">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1244-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1244-128">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1244-128">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a1244-129">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1244-129">Application</span></span> | <span data-ttu-id="a1244-130">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1244-130">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1244-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1244-131">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="a1244-132">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a1244-132">Optional query parameters</span></span>
<span data-ttu-id="a1244-133">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a1244-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a1244-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1244-134">Request headers</span></span>
| <span data-ttu-id="a1244-135">Name</span><span class="sxs-lookup"><span data-stu-id="a1244-135">Name</span></span>       | <span data-ttu-id="a1244-136">Typ</span><span class="sxs-lookup"><span data-stu-id="a1244-136">Type</span></span> | <span data-ttu-id="a1244-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1244-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="a1244-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1244-138">Authorization</span></span>  | <span data-ttu-id="a1244-139">string</span><span class="sxs-lookup"><span data-stu-id="a1244-139">string</span></span> | <span data-ttu-id="a1244-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1244-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a1244-142">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a1244-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="a1244-143">string</span><span class="sxs-lookup"><span data-stu-id="a1244-143">string</span></span> | <span data-ttu-id="a1244-144">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="a1244-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="a1244-145">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1244-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="a1244-146">Optional.</span><span class="sxs-lookup"><span data-stu-id="a1244-146">Optional.</span></span> |
| <span data-ttu-id="a1244-147">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a1244-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a1244-148">string</span><span class="sxs-lookup"><span data-stu-id="a1244-148">string</span></span> | <span data-ttu-id="a1244-149">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="a1244-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="a1244-150">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="a1244-150">Values can be "text" or "html".</span></span> <span data-ttu-id="a1244-151">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="a1244-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="a1244-152">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1244-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="a1244-153">Optional.</span><span class="sxs-lookup"><span data-stu-id="a1244-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1244-154">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1244-154">Request body</span></span>
<span data-ttu-id="a1244-155">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a1244-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1244-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1244-156">Response</span></span>

<span data-ttu-id="a1244-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1244-157">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1244-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1244-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1244-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1244-159">Request</span></span>
<span data-ttu-id="a1244-p109">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="a1244-p109">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="a1244-162">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="a1244-162">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="a1244-p110">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1244-p110">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="a1244-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1244-165">Response</span></span>
<span data-ttu-id="a1244-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Die **body**-Eigenschaft wird im HTML-Standardformat zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1244-p111">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Ereignisse auflisten
description: 'Abrufen einer Liste der Ereignisobjekte von Standardkalender des Benutzers oder '
localization_priority: Priority
ms.openlocfilehash: 3d4938d866d4dc2d0f5c5fad65b40085f86b35d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825956"
---
# <a name="list-events"></a><span data-ttu-id="a064d-103">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="a064d-103">List events</span></span>

> <span data-ttu-id="a064d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a064d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a064d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a064d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a064d-106">Rufen Sie eine Liste der [Ereignisobjekte](../resources/event.md) aus Standardkalender des Benutzers oder einen angegebenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="a064d-106">Get a list of [event](../resources/event.md) objects from the user's default calendar or from a specified calendar.</span></span> <span data-ttu-id="a064d-107">Die Liste enthält Einzelinstanz Besprechungen und Series-Master.</span><span class="sxs-lookup"><span data-stu-id="a064d-107">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="a064d-108">Um erweiterte Ereignisinstanzen abzurufen, können Sie [die Kalenderansicht abrufen](calendar-list-calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="a064d-108">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="a064d-109">Es gibt zwei Szenarien, in dem eine app Ereignisse im Kalender des Benutzers abzurufen:</span><span class="sxs-lookup"><span data-stu-id="a064d-109">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="a064d-110">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="a064d-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a064d-111">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen Kalender freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="a064d-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a064d-112">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="a064d-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="a064d-113">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="a064d-113">Support various time zones</span></span>

<span data-ttu-id="a064d-114">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="a064d-114">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="a064d-115">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="a064d-115">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="a064d-p104">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-p104">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="a064d-119">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="a064d-119">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="a064d-120">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a064d-120">Permissions</span></span>
<span data-ttu-id="a064d-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a064d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a064d-123">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a064d-123">Permission type</span></span>      | <span data-ttu-id="a064d-124">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a064d-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a064d-125">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a064d-125">Delegated (work or school account)</span></span> | <span data-ttu-id="a064d-126">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a064d-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a064d-127">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a064d-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a064d-128">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a064d-128">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a064d-129">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a064d-129">Application</span></span> | <span data-ttu-id="a064d-130">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a064d-130">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a064d-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a064d-131">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="a064d-132">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a064d-132">Optional query parameters</span></span>
<span data-ttu-id="a064d-133">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a064d-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a064d-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a064d-134">Request headers</span></span>
| <span data-ttu-id="a064d-135">Name</span><span class="sxs-lookup"><span data-stu-id="a064d-135">Name</span></span>       | <span data-ttu-id="a064d-136">Typ</span><span class="sxs-lookup"><span data-stu-id="a064d-136">Type</span></span> | <span data-ttu-id="a064d-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a064d-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a064d-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="a064d-138">Authorization</span></span>  | <span data-ttu-id="a064d-139">string</span><span class="sxs-lookup"><span data-stu-id="a064d-139">string</span></span>  | <span data-ttu-id="a064d-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a064d-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a064d-142">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a064d-142">Prefer: outlook.timezone</span></span> | <span data-ttu-id="a064d-143">string</span><span class="sxs-lookup"><span data-stu-id="a064d-143">string</span></span> | <span data-ttu-id="a064d-144">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="a064d-145">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="a064d-146">Optional.</span><span class="sxs-lookup"><span data-stu-id="a064d-146">Optional.</span></span> |
| <span data-ttu-id="a064d-147">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a064d-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a064d-148">string</span><span class="sxs-lookup"><span data-stu-id="a064d-148">string</span></span> | <span data-ttu-id="a064d-149">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="a064d-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="a064d-150">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="a064d-150">Values can be "text" or "html".</span></span> <span data-ttu-id="a064d-151">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="a064d-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="a064d-152">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="a064d-153">Optional.</span><span class="sxs-lookup"><span data-stu-id="a064d-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a064d-154">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a064d-154">Request body</span></span>
<span data-ttu-id="a064d-155">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a064d-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a064d-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="a064d-156">Response</span></span>

<span data-ttu-id="a064d-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-157">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a064d-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a064d-158">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a064d-159">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="a064d-159">Request 1</span></span>
<span data-ttu-id="a064d-160">Im erste Beispiel ruft die Ereignisse des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="a064d-160">The first example gets all the user's events.</span></span> <span data-ttu-id="a064d-161">Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="a064d-161">It specifies the following:</span></span>

- <span data-ttu-id="a064d-162">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="a064d-162">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="a064d-p110">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-p110">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="a064d-165">Die Anforderung gibt keine `Prefer: outlook.body-content-type` Kopfzeile an, dass ein bestimmtes Format für den Textkörper zurückgegebene Ereignis.</span><span class="sxs-lookup"><span data-stu-id="a064d-165">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="a064d-166">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="a064d-166">Response 1</span></span>
<span data-ttu-id="a064d-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a064d-167">Here is an example of the response.</span></span> <span data-ttu-id="a064d-168">Da kein `Prefer: outlook.body-content-type` Kopfzeile angegeben wurde, wird die **Body** -Eigenschaft in der Standard-HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-168">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="a064d-169">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="a064d-169">Request 2</span></span>
<span data-ttu-id="a064d-170">Das zweite Beispiel zeigt, wie Sie eine `Prefer: outlook.body-content-type="text"` Header, um die **Body** -Eigenschaft der angegebenen Nachricht im Textformat erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="a064d-170">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>

<span data-ttu-id="a064d-171">Die Anforderung verwendet auch eine `$select` Parameter zum Zurückgeben bestimmter Eigenschaften abzufragen.</span><span class="sxs-lookup"><span data-stu-id="a064d-171">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="a064d-172">Ohne ein `$select` -Parameter aller Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-172">Without a `$select` parameter, all of the event properties will be returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text" 
```
##### <a name="response-2"></a><span data-ttu-id="a064d-173">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="a064d-173">Response 2</span></span>
<span data-ttu-id="a064d-174">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a064d-174">Here is an example of the response.</span></span> <span data-ttu-id="a064d-175">Die **Body** -Eigenschaft wird im Text-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a064d-175">The **body** property is returned in text format.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

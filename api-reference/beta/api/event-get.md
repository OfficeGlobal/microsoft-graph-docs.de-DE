---
title: Ereignis abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen event-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 491bf4c60d8de5f85b8ddff91ebbc0703c7cdd97
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828994"
---
# <a name="get-event"></a><span data-ttu-id="879c3-103">Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="879c3-103">Get event</span></span>

> <span data-ttu-id="879c3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="879c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="879c3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="879c3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="879c3-106">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen [event](../resources/event.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="879c3-106">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="879c3-107">Es gibt zwei Szenarien, in dem eine app ein Ereignis im Kalender des Benutzers abzurufen:</span><span class="sxs-lookup"><span data-stu-id="879c3-107">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="879c3-108">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="879c3-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="879c3-109">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen Kalender freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="879c3-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="879c3-110">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="879c3-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="879c3-111">Da die **event**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **event**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="879c3-111">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="879c3-112">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="879c3-112">Support various time zones</span></span>

<span data-ttu-id="879c3-113">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="879c3-113">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="879c3-114">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="879c3-114">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="879c3-p103">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="879c3-118">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="879c3-118">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="879c3-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="879c3-119">Permissions</span></span>
<span data-ttu-id="879c3-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="879c3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="879c3-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="879c3-122">Permission type</span></span>      | <span data-ttu-id="879c3-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="879c3-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="879c3-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="879c3-124">Delegated (work or school account)</span></span> | <span data-ttu-id="879c3-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="879c3-125">Calendars.Read</span></span>    |
|<span data-ttu-id="879c3-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="879c3-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="879c3-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="879c3-127">Calendars.Read</span></span>    |
|<span data-ttu-id="879c3-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="879c3-128">Application</span></span> | <span data-ttu-id="879c3-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="879c3-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="879c3-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="879c3-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroup/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="879c3-131">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="879c3-131">Optional query parameters</span></span>
<span data-ttu-id="879c3-132">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="879c3-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="879c3-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="879c3-133">Request headers</span></span>
| <span data-ttu-id="879c3-134">Name</span><span class="sxs-lookup"><span data-stu-id="879c3-134">Name</span></span>       | <span data-ttu-id="879c3-135">Typ</span><span class="sxs-lookup"><span data-stu-id="879c3-135">Type</span></span> | <span data-ttu-id="879c3-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="879c3-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="879c3-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="879c3-137">Authorization</span></span>  | <span data-ttu-id="879c3-138">string</span><span class="sxs-lookup"><span data-stu-id="879c3-138">string</span></span>  | <span data-ttu-id="879c3-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="879c3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="879c3-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="879c3-141">Prefer: outlook.timezone</span></span> | <span data-ttu-id="879c3-142">string</span><span class="sxs-lookup"><span data-stu-id="879c3-142">string</span></span> | <span data-ttu-id="879c3-143">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="879c3-144">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="879c3-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="879c3-145">Optional.</span></span> |
| <span data-ttu-id="879c3-146">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="879c3-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="879c3-147">string</span><span class="sxs-lookup"><span data-stu-id="879c3-147">string</span></span> | <span data-ttu-id="879c3-148">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="879c3-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="879c3-149">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="879c3-149">Values can be "text" or "html".</span></span> <span data-ttu-id="879c3-150">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="879c3-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="879c3-151">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="879c3-152">Optional.</span><span class="sxs-lookup"><span data-stu-id="879c3-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="879c3-153">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="879c3-153">Request body</span></span>
<span data-ttu-id="879c3-154">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="879c3-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="879c3-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="879c3-155">Response</span></span>

<span data-ttu-id="879c3-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-156">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="879c3-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="879c3-157">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="879c3-158">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="879c3-158">Request 1</span></span>
<span data-ttu-id="879c3-p108">Im erste Beispiel wird das angegebene Ereignis abgerufen. Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="879c3-p108">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="879c3-161">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="879c3-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="879c3-p109">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="879c3-164">Die Anforderung gibt keine `Prefer: outlook.body-content-type` Kopfzeile an, dass ein bestimmtes Format für den Textkörper zurückgegebene Ereignis.</span><span class="sxs-lookup"><span data-stu-id="879c3-164">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="879c3-165">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="879c3-165">Response 1</span></span>
<span data-ttu-id="879c3-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="879c3-166">Here is an example of the response.</span></span> <span data-ttu-id="879c3-167">Da kein `Prefer: outlook.body-content-type` Kopfzeile angegeben wurde, wird die **Body** -Eigenschaft in der Standard-HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-167">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1928

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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
```

##### <a name="request-2"></a><span data-ttu-id="879c3-168">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="879c3-168">Request 2</span></span>
<span data-ttu-id="879c3-169">Das zweite Beispiel zeigt, wie Sie eine `Prefer: outlook.body-content-type="text"` Header, um die **Body** -Eigenschaft des angegebenen Ereignisses im Textformat erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="879c3-169">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="879c3-170">Die Anforderung verwendet auch eine `$select` Parameter zum Zurückgeben bestimmter Eigenschaften abzufragen.</span><span class="sxs-lookup"><span data-stu-id="879c3-170">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="879c3-171">Ohne ein `$select` -Parameter aller Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-171">Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAoZDOFAAA=')?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
##### <a name="response-2"></a><span data-ttu-id="879c3-172">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="879c3-172">Response 2</span></span>
<span data-ttu-id="879c3-173">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="879c3-173">Here is an example of the response.</span></span> <span data-ttu-id="879c3-174">Die **Body** -Eigenschaft wird im Text-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="879c3-174">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "name": "get_event_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 636

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGI1AAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
    }
}
```


##### <a name="request-3"></a><span data-ttu-id="879c3-175">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="879c3-175">Request 3</span></span>

<span data-ttu-id="879c3-176">Im dritte Beispiel zeigt ein Ereignis, das mehr als einem Standort gibt abrufen.</span><span class="sxs-lookup"><span data-stu-id="879c3-176">The third example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="879c3-177">Die Anforderung gibt einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="879c3-177">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkADAGAADDdm4NAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-3"></a><span data-ttu-id="879c3-178">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="879c3-178">Response 3</span></span>
<span data-ttu-id="879c3-179">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="879c3-179">Here is an example of the response.</span></span> <span data-ttu-id="879c3-180">Die **locations**-Eigenschaft umfasst Details für die drei Orte, für die das Ereignis organisiert wird.</span><span class="sxs-lookup"><span data-stu-id="879c3-180">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="879c3-181">Da die Anforderung keine festlegt `Prefer: outlook.timezone` oder `Prefer: outlook.body-content-type` Header, den **start** und **End** -Eigenschaften werden in der Standardeinstellung UTC-Zeitzone angezeigt, und der Textkörper weist das Standard-HTML-Format.</span><span class="sxs-lookup"><span data-stu-id="879c3-181">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

<!-- {
  "blockType": "response",
  "name": "get_event_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"UTC"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"UTC"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
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
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="879c3-182">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="879c3-182">See also</span></span>

- [<span data-ttu-id="879c3-183">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="879c3-183">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="879c3-184">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="879c3-184">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="879c3-185">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="879c3-185">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

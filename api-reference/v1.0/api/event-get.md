---
title: Ereignis abrufen
description: Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen event-Objekts.
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: fa525081bf785267edd79823d2ddcba44a9db50a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821469"
---
# <a name="get-event"></a><span data-ttu-id="9ec8b-103">Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="9ec8b-103">Get event</span></span>

<span data-ttu-id="9ec8b-104">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen [event](../resources/event.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-104">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="9ec8b-105">Zurzeit gibt dieser Vorgang Ereignistext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-105">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="9ec8b-106">Es gibt zwei Szenarien, in dem eine app ein Ereignis im Kalender des Benutzers abzurufen:</span><span class="sxs-lookup"><span data-stu-id="9ec8b-106">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="9ec8b-107">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="9ec8b-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="9ec8b-108">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen Kalender freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="9ec8b-109">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="9ec8b-109">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="9ec8b-110">Da die **event**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **event**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-110">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="9ec8b-111">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="9ec8b-111">Support various time zones</span></span>

<span data-ttu-id="9ec8b-112">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="9ec8b-113">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="9ec8b-p102">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="9ec8b-117">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="9ec8b-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9ec8b-118">Permissions</span></span>
<span data-ttu-id="9ec8b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ec8b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec8b-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ec8b-121">Permission type</span></span>      | <span data-ttu-id="9ec8b-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ec8b-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ec8b-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ec8b-123">Delegated (work or school account)</span></span> | <span data-ttu-id="9ec8b-124">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9ec8b-124">Calendars.Read</span></span>    |
|<span data-ttu-id="9ec8b-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ec8b-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ec8b-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9ec8b-126">Calendars.Read</span></span>    |
|<span data-ttu-id="9ec8b-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ec8b-127">Application</span></span> | <span data-ttu-id="9ec8b-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9ec8b-128">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ec8b-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ec8b-129">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="9ec8b-130">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9ec8b-130">Optional query parameters</span></span>
<span data-ttu-id="9ec8b-131">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9ec8b-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ec8b-132">Request headers</span></span>
| <span data-ttu-id="9ec8b-133">Name</span><span class="sxs-lookup"><span data-stu-id="9ec8b-133">Name</span></span>       | <span data-ttu-id="9ec8b-134">Typ</span><span class="sxs-lookup"><span data-stu-id="9ec8b-134">Type</span></span> | <span data-ttu-id="9ec8b-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ec8b-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="9ec8b-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ec8b-136">Authorization</span></span>  | <span data-ttu-id="9ec8b-137">string</span><span class="sxs-lookup"><span data-stu-id="9ec8b-137">string</span></span> | <span data-ttu-id="9ec8b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ec8b-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9ec8b-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="9ec8b-141">string</span><span class="sxs-lookup"><span data-stu-id="9ec8b-141">string</span></span> | <span data-ttu-id="9ec8b-142">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="9ec8b-143">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="9ec8b-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-144">Optional.</span></span> |
| <span data-ttu-id="9ec8b-145">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="9ec8b-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="9ec8b-146">string</span><span class="sxs-lookup"><span data-stu-id="9ec8b-146">string</span></span> | <span data-ttu-id="9ec8b-147">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="9ec8b-148">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-148">Values can be "text" or "html".</span></span> <span data-ttu-id="9ec8b-149">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="9ec8b-150">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="9ec8b-151">Optional.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ec8b-152">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ec8b-152">Request body</span></span>
<span data-ttu-id="9ec8b-153">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ec8b-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ec8b-154">Response</span></span>

<span data-ttu-id="9ec8b-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-155">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ec8b-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ec8b-156">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9ec8b-157">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="9ec8b-157">Request 1</span></span>
<span data-ttu-id="9ec8b-p107">Im erste Beispiel wird das angegebene Ereignis abgerufen. Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="9ec8b-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="9ec8b-160">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-160">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="9ec8b-p108">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGIAAAoZDOFAAA="],
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGIAAAoZDOFAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response-1"></a><span data-ttu-id="9ec8b-163">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="9ec8b-163">Response 1</span></span>

<span data-ttu-id="9ec8b-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Die **body**-Eigenschaft wird im HTML-Standardformat zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-p109">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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


##### <a name="request-2"></a><span data-ttu-id="9ec8b-166">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="9ec8b-166">Request 2</span></span>

<span data-ttu-id="9ec8b-167">Im zweiten Beispiel wird das Abrufen eines Ereignisses dargestellt, das mehr als einen Ort angibt.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-167">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="9ec8b-168">Die Anforderung gibt einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-168">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADAGAADDdm4NAAA="],
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGAADDdm4NAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-2"></a><span data-ttu-id="9ec8b-169">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="9ec8b-169">Response 2</span></span>
<span data-ttu-id="9ec8b-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-170">Here is an example of the response.</span></span> <span data-ttu-id="9ec8b-171">Die **locations**-Eigenschaft umfasst Details für die drei Orte, für die das Ereignis organisiert wird.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-171">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="9ec8b-172">Da die Anforderung keinen `Prefer: outlook.timezone`-Header angibt, werden die Eigenschaften **start** und **end** in der standardmäßigen UTC-Zeitzone angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-172">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="9ec8b-173">Der Ereignistext weist das standardmäßige HTML-Format auf.</span><span class="sxs-lookup"><span data-stu-id="9ec8b-173">The event body is in the default HTML format.</span></span>  

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
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



## <a name="see-also"></a><span data-ttu-id="9ec8b-174">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="9ec8b-174">See also</span></span>

- [<span data-ttu-id="9ec8b-175">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="9ec8b-175">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9ec8b-176">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="9ec8b-176">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9ec8b-177">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="9ec8b-177">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

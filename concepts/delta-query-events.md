---
title: 'Abrufen inkrementeller Änderungen an Ereignissen in einer Kalenderansicht '
description: 'Eine Kalenderansicht ist eine Sammlung von Ereignissen in einem Datums-/Uhrzeitbereich aus dem Standardkalender (../me/calendarview) '
ms.openlocfilehash: 68e4053c29fd95f04ff0b031bf519301e63dc08a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092245"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a><span data-ttu-id="86d9b-103">Abrufen inkrementeller Änderungen an Ereignissen in einer Kalenderansicht</span><span class="sxs-lookup"><span data-stu-id="86d9b-103">Get incremental changes to events in a calendar view</span></span> 

<span data-ttu-id="86d9b-p101">Eine Kalenderansicht ist eine Sammlung von Ereignissen in einen Datums-/Uhrzeitbereich aus dem Standardkalender (../me/calendarview) oder aus einem anderen Kalender des Benutzers. Durch Verwendung einer Delta-Abfrage können Sie neue, aktualisierte oder gelöschte Ereignisse in einer Kalenderansicht abrufen. Die zurückgegebenen Ereignisse können Vorkommen und Ausnahmen einer Serie und einzelne Instanzen enthalten. Mit Delta-Daten können Sie einen lokalen Speicher für Ereignisse eines Benutzers pflegen und synchronisieren, ohne dass Sie jedes Mal den gesamten Ereignissatz vom Server abrufen müssen.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p101">A calendar view is a collection of events in a date/time range from the default calendar (../me/calendarview) or some other calendar of the user's. By using delta query, you can get new, updated, or deleted events in a calendar view. The returned events may include occurrences and exceptions of a recurring series, and single instances. The delta data enables you to maintain and synchronize a local store of a user's events, without having to fetch the entire set of the user's events from the server every time.</span></span>

<span data-ttu-id="86d9b-p102">Die Delta-Abfrage unterstützt die vollständige Synchronisierung, die alle Ereignisse in der angegebenen Kalenderansicht abruft, und die inkrementelle Synchronisierung, die nur die Ereignisse abruft, die seit der letzten Synchronisierung in der Kalenderansicht geändert wurden. In der Regel führen Sie zunächst eine vollständige Synchronisierung durch und rufen anschließend regelmäßig inkrementelle Änderungen an dieser Kalenderansicht ab.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p102">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization. Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span> 

## <a name="track-event-changes-in-a-calendar-view"></a><span data-ttu-id="86d9b-110">Nachverfolgen von Ereignisänderungen in einer Kalenderansicht</span><span class="sxs-lookup"><span data-stu-id="86d9b-110">Track event changes in a calendar view</span></span>

<span data-ttu-id="86d9b-p103">Delta-Abfragen für Ereignisse sind spezifisch für einen Kalender und Datums-/Uhrzeitbereich, den Sie angeben (d. h. eine Kalenderansicht). Um die Änderungen in mehreren Kalendern nachzuverfolgen, müssen Sie jeden Kalender einzeln verfolgen.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p103">Delta query for events is specific to a calendar and date/time range that you specify (i.e., a calendar view). To track the changes in multiple calendars, you need to track each calendar individually.</span></span> 

<span data-ttu-id="86d9b-p104">Das Nachverfolgen von Ereignisänderungen in einer Kalenderansicht ist in der Regel eine Runde aus einer oder mehreren GET-Anforderungen mit der [Delta](/graph/api/event-delta?view=graph-rest-1.0)-Funktion. Die ursprüngliche GET-Anforderung wird ähnlich wie das [Auflisten einer Kalenderansicht](/graph/api/calendar-list-calendarview?view=graph-rest-1.0) durchgeführt, außer dass die folgende **delta**-Funktion eingeschlossen wird:</span><span class="sxs-lookup"><span data-stu-id="86d9b-p104">Tracking event changes in a calendar view typically is a round of one or more GET requests with the [delta](/graph/api/event-delta?view=graph-rest-1.0) function. The initial GET request is very much like the way you [list a calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), except that you include the **delta** function:</span></span>

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="86d9b-115">Eine GET-Anforderung mit der **delta**-Funktion gibt Folgendes zurück:</span><span class="sxs-lookup"><span data-stu-id="86d9b-115">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="86d9b-116">`nextLink` (mit einer URL mit einem **delta**-Funktionsaufruf und einem _skipToken_) oder</span><span class="sxs-lookup"><span data-stu-id="86d9b-116">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="86d9b-117">`deltaLink` (mit einer URL mit einem **delta**-Funktionsaufruf und einem _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="86d9b-117">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="86d9b-118">Diese Token sind [Statustoken](delta-query-overview.md#state-tokens), die die refs/remotes/microsoftgraph/master-Parameter _startDateTime_ und _endDateTime_ sowie alle anderen Abfrageparameter in der GET-Anforderung der ursprünglichen Delta-Abfrage codieren.</span><span class="sxs-lookup"><span data-stu-id="86d9b-118">These tokens are [state tokens](delta-query-overview.md#state-tokens) which encode the refs/remotes/microsoftgraph/master _startDateTime_ and _endDateTime_ parameters, and any other query parameter in your initial delta query GET request.</span></span> 

<span data-ttu-id="86d9b-p105">Zustandstoken sind für den Client nicht transparent. Um mit einer Änderungsnachverfolgung fortzufahren, kopieren Sie die von der letzten GET-Anforderung zurückgegebene `nextLink`- oder `deltaLink`-URL einfach und wenden sie auf den nächsten **delta**-Funktionsaufruf für dieselbe Kalenderansicht an. `deltaLink` (in einer Antwort zurückgegeben), bedeutet, dass die aktuelle Runde der Änderungsnachverfolgung abgeschlossen ist. Sie können die `deltaLink`-URL für die nächste Runde speichern und verwenden.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p105">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next **delta** function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="86d9b-123">Im [Beispiel](#example-to-synchronize-events-in-a-calendar-view) unten finden Sie Informationen zur Verwendung der `nextLink`- und `deltaLink`-URLs.</span><span class="sxs-lookup"><span data-stu-id="86d9b-123">See the [example](#example-to-synchronize-events-in-a-calendar-view) below to learn how to use these `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a><span data-ttu-id="86d9b-124">Verwenden von Abfrageparametern in einer Delta-Abfrage für eine Kalenderansicht</span><span class="sxs-lookup"><span data-stu-id="86d9b-124">Use query parameters in a delta query for calendar view</span></span>

- <span data-ttu-id="86d9b-125">Schließen Sie die Parameter _startDateTime_ und _endDateTime_ ein, um einen Datums-/Uhrzeitbereich für Ihre Kalenderansicht zu definieren.</span><span class="sxs-lookup"><span data-stu-id="86d9b-125">Include the _startDateTime_ and _endDateTime_ parameters to define a date/time range for your calendar view.</span></span>
- <span data-ttu-id="86d9b-126">`$select` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86d9b-126">`$select` is not supported.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="86d9b-127">Optionaler Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86d9b-127">Optional request header</span></span>

<span data-ttu-id="86d9b-128">Jede GET-Anforderung der Delta-Abfrage gibt eine Sammlung aus einem oder mehreren Ereignissen in der Antwort zurück.</span><span class="sxs-lookup"><span data-stu-id="86d9b-128">Each delta query GET request returns a collection of one or more events in the response.</span></span> <span data-ttu-id="86d9b-129">Sie können optional den Anforderungsheader, `Prefer: odata.maxpagesize={x}`, angeben, um die maximale Anzahl an Ereignissen in einer Antwort festzulegen.</span><span class="sxs-lookup"><span data-stu-id="86d9b-129">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of events in a response.</span></span>


## <a name="example-to-synchronize-events-in-a-calendar-view"></a><span data-ttu-id="86d9b-130">Beispiel für die Synchronisierung von Ereignissen in einer Kalenderansicht</span><span class="sxs-lookup"><span data-stu-id="86d9b-130">Example to synchronize events in a calendar view</span></span>

<span data-ttu-id="86d9b-p107">Das folgende Beispiel zeigt eine Reihe von 3 Anforderungen zum Synchronisieren des Standardkalenders eines Benutzers in einem bestimmten Zeitbereich. Es gibt 5 Ereignisse in dieser Kalenderansicht.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p107">The following example shows a series of 3 requests to synchronize the user's default calendar in a specific time range. There are 5 events in that calendar view.</span></span>

- <span data-ttu-id="86d9b-133">[Schritt 1: Beispiel für ursprüngliche Anforderung](#step-1-sample-initial-request) und [Antwort](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="86d9b-133">[Step 1: sample initial request](#step-1-sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="86d9b-134">[Schritt 2: Beispiel für zweite Anforderung](#step-2-sample-second-request) und [Antwort](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="86d9b-134">[Step 2: sample second request](#step-2-sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="86d9b-135">[Schritt 3: Beispiel für dritte Anforderung](#step-3-sample-third-request) und [letzte Antwort](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="86d9b-135">[Step 3: sample third request](#step-3-sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="86d9b-p108">Aus Platzgründen wird in den Beispielantworten nur eine Untergruppe der Eigenschaften eines Ereignisses angezeigt. In einem tatsächlichen Aufruf werden die meiste Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p108">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span> 

<span data-ttu-id="86d9b-138">Sehen Sie sich auch an, was Sie in der [nächsten Runde](#the-next-round-sample-first-response) tun werden.</span><span class="sxs-lookup"><span data-stu-id="86d9b-138">See also what you'll do in the [next round](#the-next-round-sample-first-response).</span></span>


### <a name="step-1-sample-initial-request"></a><span data-ttu-id="86d9b-139">Schritt 1: Beispiel für ursprüngliche Anforderung</span><span class="sxs-lookup"><span data-stu-id="86d9b-139">Step 1: sample initial request</span></span>

<span data-ttu-id="86d9b-p109">In diesem Beispiel wird die angegebene Kalenderansicht zum ersten Mal synchronisiert, sodass die ursprüngliche Synchronisierungsanforderung kein Statustoken enthält. In dieser Runde werden alle Ereignisse in dieser Kalenderansicht zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p109">In this example, the specified calendar view is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="86d9b-142">Die erste Anforderung gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="86d9b-142">The first request specifies the following:</span></span>

- <span data-ttu-id="86d9b-143">Datum-/Uhrzeitwerte für die Parameter _startDateTime_ und _endDateTime_.</span><span class="sxs-lookup"><span data-stu-id="86d9b-143">Date/time values for the _startDateTime_ and _endDateTime_ parameters.</span></span>
- <span data-ttu-id="86d9b-144">Den [optionalen Anforderungsheader](#optional-request-header), _odata.maxpagesize_, der gleichzeitig 2 Ereignisse zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="86d9b-144">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 events at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a><span data-ttu-id="86d9b-145">Beispiel für ursprüngliche Antwort</span><span class="sxs-lookup"><span data-stu-id="86d9b-145">Sample initial response</span></span>

<span data-ttu-id="86d9b-p110">Die Antwort enthält zwei Ereignisse und einen `@odata.nextLink`-Antwortheader mit einem `skipToken`. Die `nextLink`-URL gibt an, dass in der Kalenderansicht weitere Ereignisse abgerufen werden können.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p110">The response includes two events and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more events in the calendar view to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIQ==\"",
            "subject":"Plan shopping list",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-09T20:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-09T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },      
            "id":"AAMkADNVxRAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIg==\"",
            "subject":"Pick up car",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T01:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxSAAA="
        }
    ]
}
```

### <a name="step-2-sample-second-request"></a><span data-ttu-id="86d9b-148">Schritt 2: Beispiel für zweite Anforderung</span><span class="sxs-lookup"><span data-stu-id="86d9b-148">Step 2: sample second request</span></span>

<span data-ttu-id="86d9b-p111">Die zweite Anforderung gibt die aus der vorherigen Antwort zurückgegebene `nextLink`-URL an. Beachten Sie, dass sie nicht dieselben Parameter _startDateTime_ und _endDateTime_ wie in der ursprünglichen Anforderung angeben muss, da das `skipToken` in der `nextLink`-URL diese codiert und einschließt.</span><span class="sxs-lookup"><span data-stu-id="86d9b-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same _startDateTime_ and _endDateTime_ parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="86d9b-151">Beispiel für zweite Antwort</span><span class="sxs-lookup"><span data-stu-id="86d9b-151">Sample second response</span></span> 

<span data-ttu-id="86d9b-152">Die zweite Antwort gibt die nächsten 2 Ereignisse in der Kalenderansicht und ein weiteres `nextLink`, was bedeutet, dass weitere abzurufende Ereignisse in der Kalenderansicht vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="86d9b-152">The second response returns the next 2 events in the calendar view and another `nextLink`, indicating there are more events to get from the calendar view.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIw==\"",
            "subject":"Get food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T19:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T21:30:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxTAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvJA==\"",
            "subject":"Prepare food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-11T00:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxUAAA="
        }
    ]
}
```


### <a name="step-3-sample-third-request"></a><span data-ttu-id="86d9b-153">Schritt 3: Beispiel für dritte Anforderung</span><span class="sxs-lookup"><span data-stu-id="86d9b-153">Step 3: sample third request</span></span>

<span data-ttu-id="86d9b-154">Die dritte Anforderung verwendet weiterhin das neueste aus der letzten Synchronisierungsanforderung zurückgegebene `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="86d9b-154">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span> 
 

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="86d9b-155">Beispiel für dritte und letzte Antwort</span><span class="sxs-lookup"><span data-stu-id="86d9b-155">Sample third and final response</span></span>

<span data-ttu-id="86d9b-p112">Die dritte Antwort gibt das einzige in dem Ordner verbleibende Ereignis in der Kalenderansicht sowie eine `deltaLink`-URL zurück, was bedeutet, dass die Synchronisierung für diese Kalenderansicht momentan abgeschlossen ist. Speichern und verwenden Sie die `deltaLink`-URL, um [diese Kalenderansicht in der nächsten Runde zu synchronisieren](#the-next-round-sample-first-request).</span><span class="sxs-lookup"><span data-stu-id="86d9b-p112">The third response returns the only remaining event in the calendar view, and a `deltaLink` URL which indicates synchronization is complete for this calendar view. Save and use the `deltaLink` URL to [synchronize that calendar view in the next round](#the-next-round-sample-first-request).</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97g==\"",
            "subject":"Rest!",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-12T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-12T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Home"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HuAAA="
        }
    ]
}
```


### <a name="the-next-round-sample-first-request"></a><span data-ttu-id="86d9b-158">Die nächste Runde: Beispiel für erste Anforderung</span><span class="sxs-lookup"><span data-stu-id="86d9b-158">The next round: sample first request</span></span>

<span data-ttu-id="86d9b-p113">Mit dem `deltaLink` aus der [letzten Anforderung](#step-3-sample-third-request) in der letzten Runde können Sie nur die Ereignisse abrufen, die sich seitdem in dieser Kalenderansicht geändert haben (durch Hinzufügung, Löschung oder Aktualisierung). Ihre erste Anforderung in der nächsten Runde sieht folgendermaßen aus, sofern Sie die gleiche maximale Seitengröße in der Antwort beibehalten möchten:</span><span class="sxs-lookup"><span data-stu-id="86d9b-p113">Using the `deltaLink` from the [last request](#step-3-sample-third-request) in the last round, you will be able to get only those events that have changed (by being added, deleted, or updated) in that calendar view since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="the-next-round-sample-first-response"></a><span data-ttu-id="86d9b-161">Die nächste Runde: Beispiel für erste Antwort</span><span class="sxs-lookup"><span data-stu-id="86d9b-161">The next round: sample first response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcFuQtZdtpk4",
    "value":[
        {
            "@odata.type": "#microsoft.graph.event",
            "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS04OGQLkRkXbBznTvAADb6ytyAAA=",
            "@removed": {
                "reason": "deleted"
            }
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97w==\"",
            "subject":"Attend service",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-25T06:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-25T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Chapel of Saint Ignatius",
                "address":{
                    "street":"900 Broadway",
                    "city":"Seattle",
                    "state":"WA",
                    "countryOrRegion":"United States",
                    "postalCode":""
                },
                "coordinates":{
                    "latitude":47.6105,
                    "longitude":-122.321
                }
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HvAAA="
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="86d9b-162">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="86d9b-162">See also</span></span>

- [<span data-ttu-id="86d9b-163">Microsoft Graph-Delta-Abfrage</span><span class="sxs-lookup"><span data-stu-id="86d9b-163">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="86d9b-164">Inkrementelle Änderungen an Nachrichten abrufen</span><span class="sxs-lookup"><span data-stu-id="86d9b-164">Get incremental changes to messages</span></span>](delta-query-messages.md)
- [<span data-ttu-id="86d9b-165">Inkrementelle Änderungen an Gruppen abrufen</span><span class="sxs-lookup"><span data-stu-id="86d9b-165">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="86d9b-166">Inkrementelle Änderungen an Benutzern abrufen</span><span class="sxs-lookup"><span data-stu-id="86d9b-166">Get incremental changes to users</span></span>](delta-query-users.md)

# <a name="list-calendarview"></a><span data-ttu-id="28ce8-101">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="28ce8-101">List calendarView</span></span>

<span data-ttu-id="28ce8-102">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender des Benutzers oder aus einem seiner anderen Kalender abrufen.</span><span class="sxs-lookup"><span data-stu-id="28ce8-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28ce8-103">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="28ce8-103">Prerequisites</span></span>
<span data-ttu-id="28ce8-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Calendars.Read; Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="28ce8-104">One of the following scopes is required to execute this API: Calendars.Read; Calendars.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="28ce8-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28ce8-105">HTTP request</span></span>

<span data-ttu-id="28ce8-106">Der standardmäßige [Kalender](../resources/calendar.md) eines Benutzers:</span><span class="sxs-lookup"><span data-stu-id="28ce8-106">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="28ce8-107">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="28ce8-107">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="28ce8-108">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="28ce8-108">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="28ce8-109">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="28ce8-109">Query parameters</span></span>

<span data-ttu-id="28ce8-110">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="28ce8-110">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="28ce8-111">Parameter</span><span class="sxs-lookup"><span data-stu-id="28ce8-111">Parameter</span></span>    | <span data-ttu-id="28ce8-112">Typ</span><span class="sxs-lookup"><span data-stu-id="28ce8-112">Type</span></span>   |<span data-ttu-id="28ce8-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28ce8-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28ce8-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="28ce8-114">startDateTime</span></span>|<span data-ttu-id="28ce8-115">String</span><span class="sxs-lookup"><span data-stu-id="28ce8-115">String</span></span>|<span data-ttu-id="28ce8-p101">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="28ce8-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="28ce8-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="28ce8-118">endDateTime</span></span>|<span data-ttu-id="28ce8-119">String</span><span class="sxs-lookup"><span data-stu-id="28ce8-119">String</span></span>|<span data-ttu-id="28ce8-p102">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="28ce8-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="28ce8-122">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="28ce8-122">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="28ce8-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28ce8-123">Request headers</span></span>
| <span data-ttu-id="28ce8-124">Name</span><span class="sxs-lookup"><span data-stu-id="28ce8-124">Name</span></span>       | <span data-ttu-id="28ce8-125">Typ</span><span class="sxs-lookup"><span data-stu-id="28ce8-125">Type</span></span> | <span data-ttu-id="28ce8-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28ce8-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="28ce8-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="28ce8-127">Authorization</span></span>  | <span data-ttu-id="28ce8-128">string</span><span class="sxs-lookup"><span data-stu-id="28ce8-128">string</span></span>  | <span data-ttu-id="28ce8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28ce8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28ce8-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28ce8-131">Content-Type</span></span>   | <span data-ttu-id="28ce8-132">string</span><span class="sxs-lookup"><span data-stu-id="28ce8-132">string</span></span>  | <span data-ttu-id="28ce8-133">application/json</span><span class="sxs-lookup"><span data-stu-id="28ce8-133">application/json</span></span> | 
| <span data-ttu-id="28ce8-134">Prefer</span><span class="sxs-lookup"><span data-stu-id="28ce8-134">Prefer</span></span> | <span data-ttu-id="28ce8-135">string</span><span class="sxs-lookup"><span data-stu-id="28ce8-135">string</span></span> | <span data-ttu-id="28ce8-p104">outlook.timezone="Eastern Standard Time". Optional.  Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, wird die Antwort in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28ce8-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28ce8-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28ce8-140">Request body</span></span>
<span data-ttu-id="28ce8-141">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="28ce8-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28ce8-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="28ce8-142">Response</span></span>

<span data-ttu-id="28ce8-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28ce8-143">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28ce8-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28ce8-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28ce8-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28ce8-145">Request</span></span>
<span data-ttu-id="28ce8-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28ce8-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="28ce8-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="28ce8-147">Response</span></span>
<span data-ttu-id="28ce8-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28ce8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

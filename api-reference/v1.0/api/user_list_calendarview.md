# <a name="list-calendarview"></a><span data-ttu-id="14a05-101">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="14a05-101">List calendarView</span></span>

<span data-ttu-id="14a05-102">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender des Benutzers oder aus einem seiner anderen Kalender abrufen.</span><span class="sxs-lookup"><span data-stu-id="14a05-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="14a05-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="14a05-103">Permissions</span></span>
<span data-ttu-id="14a05-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="14a05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="14a05-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14a05-106">Permission type</span></span>      | <span data-ttu-id="14a05-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14a05-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="14a05-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14a05-108">Delegated (work or school account)</span></span> | <span data-ttu-id="14a05-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14a05-109">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="14a05-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14a05-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14a05-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14a05-111">Calendars.Read, Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="14a05-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14a05-112">Application</span></span> | <span data-ttu-id="14a05-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14a05-113">Calendars.Read, Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="14a05-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14a05-114">HTTP request</span></span>

<span data-ttu-id="14a05-115">Der standardmäßige [Kalender](../resources/calendar.md) eines Benutzers:</span><span class="sxs-lookup"><span data-stu-id="14a05-115">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="14a05-116">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="14a05-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="14a05-117">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="14a05-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="14a05-118">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="14a05-118">Query parameters</span></span>

<span data-ttu-id="14a05-119">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="14a05-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="14a05-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="14a05-120">Parameter</span></span>    | <span data-ttu-id="14a05-121">Typ</span><span class="sxs-lookup"><span data-stu-id="14a05-121">Type</span></span>   |<span data-ttu-id="14a05-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14a05-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14a05-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="14a05-123">startDateTime</span></span>|<span data-ttu-id="14a05-124">String</span><span class="sxs-lookup"><span data-stu-id="14a05-124">String</span></span>|<span data-ttu-id="14a05-p102">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="14a05-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="14a05-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="14a05-127">endDateTime</span></span>|<span data-ttu-id="14a05-128">String</span><span class="sxs-lookup"><span data-stu-id="14a05-128">String</span></span>|<span data-ttu-id="14a05-p103">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="14a05-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="14a05-131">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="14a05-131">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="14a05-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14a05-132">Request headers</span></span>
| <span data-ttu-id="14a05-133">Name</span><span class="sxs-lookup"><span data-stu-id="14a05-133">Name</span></span>       | <span data-ttu-id="14a05-134">Typ</span><span class="sxs-lookup"><span data-stu-id="14a05-134">Type</span></span> | <span data-ttu-id="14a05-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14a05-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14a05-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="14a05-136">Authorization</span></span>  | <span data-ttu-id="14a05-137">string</span><span class="sxs-lookup"><span data-stu-id="14a05-137">string</span></span>  | <span data-ttu-id="14a05-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="14a05-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14a05-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14a05-140">Content-Type</span></span>   | <span data-ttu-id="14a05-141">string</span><span class="sxs-lookup"><span data-stu-id="14a05-141">string</span></span>  | <span data-ttu-id="14a05-142">application/json</span><span class="sxs-lookup"><span data-stu-id="14a05-142">application/json</span></span> | 
| <span data-ttu-id="14a05-143">Prefer</span><span class="sxs-lookup"><span data-stu-id="14a05-143">Prefer</span></span> | <span data-ttu-id="14a05-144">string</span><span class="sxs-lookup"><span data-stu-id="14a05-144">string</span></span> | <span data-ttu-id="14a05-p105">outlook.timezone="Eastern Standard Time". Optional.  Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, wird die Antwort in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14a05-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14a05-149">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14a05-149">Request body</span></span>
<span data-ttu-id="14a05-150">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="14a05-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14a05-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="14a05-151">Response</span></span>

<span data-ttu-id="14a05-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14a05-152">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14a05-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14a05-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14a05-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="14a05-154">Request</span></span>
<span data-ttu-id="14a05-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="14a05-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="14a05-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="14a05-156">Response</span></span>
<span data-ttu-id="14a05-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14a05-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

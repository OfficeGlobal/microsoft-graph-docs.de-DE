# <a name="list-calendarview"></a><span data-ttu-id="ea1f6-101">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="ea1f6-101">List calendarView</span></span>

<span data-ttu-id="ea1f6-102">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender `(../me/calendarview)` eines Benutzers oder einer Gruppe oder aus einem anderen Kalender des Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea1f6-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea1f6-103">Prerequisites</span></span>
<span data-ttu-id="ea1f6-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="ea1f6-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="ea1f6-105">Ereignisse im Kalender eines Benutzers: _Calendars.Read_ oder _Calendars.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="ea1f6-105">Events in a user's calendar: _Calendars.Read_ or _Calendars.ReadWrite_</span></span>
* <span data-ttu-id="ea1f6-106">Ereignisse in einem Gruppenkalender: _Group.Read.All_ oder _Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="ea1f6-106">Events in a group calendar: _Group.Read.All_ or _Group.ReadWrite.All_</span></span>

## <a name="http-request"></a><span data-ttu-id="ea1f6-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea1f6-107">HTTP request</span></span>

<span data-ttu-id="ea1f6-108">Der Standard[kalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-108">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="ea1f6-109">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="ea1f6-109">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="ea1f6-110">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="ea1f6-110">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="ea1f6-111">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ea1f6-111">Query parameters</span></span>

<span data-ttu-id="ea1f6-112">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-112">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ea1f6-113">Parameter</span><span class="sxs-lookup"><span data-stu-id="ea1f6-113">Parameter</span></span>    | <span data-ttu-id="ea1f6-114">Typ</span><span class="sxs-lookup"><span data-stu-id="ea1f6-114">Type</span></span>   |<span data-ttu-id="ea1f6-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea1f6-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea1f6-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ea1f6-116">startDateTime</span></span>|<span data-ttu-id="ea1f6-117">String</span><span class="sxs-lookup"><span data-stu-id="ea1f6-117">String</span></span>|<span data-ttu-id="ea1f6-p101">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ea1f6-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ea1f6-120">endDateTime</span></span>|<span data-ttu-id="ea1f6-121">String</span><span class="sxs-lookup"><span data-stu-id="ea1f6-121">String</span></span>|<span data-ttu-id="ea1f6-p102">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="ea1f6-124">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-124">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ea1f6-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea1f6-125">Request headers</span></span>
| <span data-ttu-id="ea1f6-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ea1f6-126">Header</span></span>       | <span data-ttu-id="ea1f6-127">Wert</span><span class="sxs-lookup"><span data-stu-id="ea1f6-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea1f6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea1f6-128">Authorization</span></span>  | <span data-ttu-id="ea1f6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ea1f6-131">Prefer</span><span class="sxs-lookup"><span data-stu-id="ea1f6-131">Prefer</span></span>  | <span data-ttu-id="ea1f6-p104">outlook.timezone="Eastern Standard Time". Optional.  Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, wird die Antwort in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea1f6-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea1f6-136">Request body</span></span>
<span data-ttu-id="ea1f6-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea1f6-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea1f6-138">Response</span></span>

<span data-ttu-id="ea1f6-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-139">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea1f6-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea1f6-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea1f6-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea1f6-141">Request</span></span>
<span data-ttu-id="ea1f6-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="ea1f6-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea1f6-143">Response</span></span>
<span data-ttu-id="ea1f6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea1f6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "response-value",
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

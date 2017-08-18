# <a name="list-instances"></a><span data-ttu-id="f799a-101">Instanzen auflisten</span><span class="sxs-lookup"><span data-stu-id="f799a-101">List instances</span></span>

<span data-ttu-id="f799a-p101">Dient zum Abrufen der Instanzen (Vorkommen) eines Ereignisses für einen angegebenen Zeitraum. Wenn das Ereignis vom Typ `SeriesMaster` ist, werden hierdurch die Vorkommen und Ausnahmen des Ereignisses im des angegebenen Zeitraum zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f799a-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f799a-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="f799a-104">Prerequisites</span></span>
<span data-ttu-id="f799a-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Calendars.Read*</span><span class="sxs-lookup"><span data-stu-id="f799a-105">One of the following **scopes** is required to execute this API: *Calendars.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="f799a-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f799a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="f799a-107">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f799a-107">Query parameters</span></span>

<span data-ttu-id="f799a-108">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="f799a-108">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="f799a-109">Parameter</span><span class="sxs-lookup"><span data-stu-id="f799a-109">Parameter</span></span>    | <span data-ttu-id="f799a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f799a-110">Type</span></span>   |<span data-ttu-id="f799a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f799a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f799a-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f799a-112">startDateTime</span></span>|<span data-ttu-id="f799a-113">String</span><span class="sxs-lookup"><span data-stu-id="f799a-113">String</span></span>|<span data-ttu-id="f799a-p102">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="f799a-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="f799a-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f799a-116">endDateTime</span></span>|<span data-ttu-id="f799a-117">String</span><span class="sxs-lookup"><span data-stu-id="f799a-117">String</span></span>|<span data-ttu-id="f799a-p103">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="f799a-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="f799a-120">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f799a-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f799a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f799a-121">Request headers</span></span>
| <span data-ttu-id="f799a-122">Name</span><span class="sxs-lookup"><span data-stu-id="f799a-122">Name</span></span>       | <span data-ttu-id="f799a-123">Typ</span><span class="sxs-lookup"><span data-stu-id="f799a-123">Type</span></span> | <span data-ttu-id="f799a-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f799a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f799a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f799a-125">Authorization</span></span>  | <span data-ttu-id="f799a-126">string</span><span class="sxs-lookup"><span data-stu-id="f799a-126">string</span></span>  | <span data-ttu-id="f799a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f799a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f799a-129">Prefer</span><span class="sxs-lookup"><span data-stu-id="f799a-129">Prefer</span></span> | <span data-ttu-id="f799a-130">string</span><span class="sxs-lookup"><span data-stu-id="f799a-130">string</span></span> | <span data-ttu-id="f799a-p105">outlook.timezone="Eastern Standard Time". Optional.  Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, wird die Antwort in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f799a-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f799a-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f799a-135">Request body</span></span>
<span data-ttu-id="f799a-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f799a-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f799a-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f799a-137">Response</span></span>

<span data-ttu-id="f799a-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f799a-138">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f799a-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f799a-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f799a-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f799a-140">Request</span></span>
<span data-ttu-id="f799a-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f799a-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="f799a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f799a-142">Response</span></span>
<span data-ttu-id="f799a-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f799a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="list-events"></a><span data-ttu-id="2509b-101">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="2509b-101">List events</span></span>

<span data-ttu-id="2509b-p101">Dient zum Abrufen einer Liste von Ereignissen in einem Kalender.  Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.</span><span class="sxs-lookup"><span data-stu-id="2509b-p101">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="2509b-104">Wenn Sie erweiterte Ereignisinstanzen abrufen möchten, können Sie [die Kalenderansicht abrufen](calendar_list_calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="2509b-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2509b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2509b-105">Permissions</span></span>
<span data-ttu-id="2509b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2509b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2509b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2509b-108">Permission type</span></span>      | <span data-ttu-id="2509b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2509b-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2509b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2509b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2509b-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2509b-111">Calendars.Read</span></span>    | 
|<span data-ttu-id="2509b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2509b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2509b-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2509b-113">Calendars.Read</span></span>    | 
|<span data-ttu-id="2509b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2509b-114">Application</span></span> | <span data-ttu-id="2509b-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2509b-115">Calendars.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2509b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2509b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2509b-117">Der Standard[kalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="2509b-117">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="2509b-118">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="2509b-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="2509b-119">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="2509b-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2509b-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2509b-120">Optional query parameters</span></span>
<span data-ttu-id="2509b-121">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2509b-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2509b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2509b-122">Request headers</span></span>
| <span data-ttu-id="2509b-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2509b-123">Header</span></span>       | <span data-ttu-id="2509b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="2509b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2509b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2509b-125">Authorization</span></span>  | <span data-ttu-id="2509b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2509b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2509b-128">Prefer</span><span class="sxs-lookup"><span data-stu-id="2509b-128">Prefer</span></span>  | <span data-ttu-id="2509b-p104">outlook.timezone="Eastern Standard Time". Optional.  Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, wird die Antwort in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2509b-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2509b-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2509b-133">Request body</span></span>
<span data-ttu-id="2509b-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2509b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2509b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2509b-135">Response</span></span>

<span data-ttu-id="2509b-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2509b-136">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2509b-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2509b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2509b-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2509b-138">Request</span></span>
<span data-ttu-id="2509b-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2509b-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="2509b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="2509b-140">Response</span></span>
<span data-ttu-id="2509b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2509b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

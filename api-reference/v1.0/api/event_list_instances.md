# <a name="list-instances"></a><span data-ttu-id="03f64-101">Instanzen auflisten</span><span class="sxs-lookup"><span data-stu-id="03f64-101">List instances</span></span>

<span data-ttu-id="03f64-p101">Dient zum Abrufen der Instanzen (Vorkommen) eines Ereignisses für einen angegebenen Zeitraum. Wenn das Ereignis vom Typ `SeriesMaster` ist, werden hierdurch die Vorkommen und Ausnahmen des Ereignisses im des angegebenen Zeitraum zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03f64-p101">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="03f64-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="03f64-104">Permissions</span></span>
<span data-ttu-id="03f64-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="03f64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03f64-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="03f64-107">Permission type</span></span>      | <span data-ttu-id="03f64-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="03f64-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03f64-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="03f64-109">Delegated (work or school account)</span></span> | <span data-ttu-id="03f64-110">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="03f64-110">Calendars.Read</span></span>    |
|<span data-ttu-id="03f64-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="03f64-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03f64-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="03f64-112">Calendars.Read</span></span>    |
|<span data-ttu-id="03f64-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="03f64-113">Application</span></span> | <span data-ttu-id="03f64-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="03f64-114">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="03f64-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="03f64-115">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="03f64-116">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="03f64-116">Query parameters</span></span>

<span data-ttu-id="03f64-117">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="03f64-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="03f64-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="03f64-118">Parameter</span></span>    | <span data-ttu-id="03f64-119">Typ</span><span class="sxs-lookup"><span data-stu-id="03f64-119">Type</span></span>   |<span data-ttu-id="03f64-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03f64-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03f64-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="03f64-121">startDateTime</span></span>|<span data-ttu-id="03f64-122">String</span><span class="sxs-lookup"><span data-stu-id="03f64-122">String</span></span>|<span data-ttu-id="03f64-p103">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="03f64-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="03f64-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="03f64-125">endDateTime</span></span>|<span data-ttu-id="03f64-126">String</span><span class="sxs-lookup"><span data-stu-id="03f64-126">String</span></span>|<span data-ttu-id="03f64-p104">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="03f64-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="03f64-129">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="03f64-129">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="03f64-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="03f64-130">Request headers</span></span>
| <span data-ttu-id="03f64-131">Name</span><span class="sxs-lookup"><span data-stu-id="03f64-131">Name</span></span>       | <span data-ttu-id="03f64-132">Typ</span><span class="sxs-lookup"><span data-stu-id="03f64-132">Type</span></span> | <span data-ttu-id="03f64-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03f64-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="03f64-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="03f64-134">Authorization</span></span>  | <span data-ttu-id="03f64-135">string</span><span class="sxs-lookup"><span data-stu-id="03f64-135">string</span></span>  | <span data-ttu-id="03f64-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="03f64-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03f64-138">Prefer</span><span class="sxs-lookup"><span data-stu-id="03f64-138">Prefer</span></span> | <span data-ttu-id="03f64-139">string</span><span class="sxs-lookup"><span data-stu-id="03f64-139">string</span></span> | <span data-ttu-id="03f64-p106">outlook.timezone="Eastern Standard Time". Optional.  Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, wird die Antwort in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03f64-p106">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03f64-144">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="03f64-144">Request body</span></span>
<span data-ttu-id="03f64-145">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="03f64-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03f64-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="03f64-146">Response</span></span>

<span data-ttu-id="03f64-147">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03f64-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03f64-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="03f64-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03f64-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="03f64-149">Request</span></span>
<span data-ttu-id="03f64-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="03f64-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="03f64-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="03f64-151">Response</span></span>
<span data-ttu-id="03f64-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03f64-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

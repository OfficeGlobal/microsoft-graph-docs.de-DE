# <a name="list-calendarview"></a><span data-ttu-id="42cfe-101">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="42cfe-101">List calendarView</span></span>

<span data-ttu-id="42cfe-102">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender einer Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="42cfe-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="42cfe-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="42cfe-103">Prerequisites</span></span>
<span data-ttu-id="42cfe-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.Read.All* oder *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="42cfe-104">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="42cfe-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42cfe-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="42cfe-106">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="42cfe-106">Query parameters</span></span>

<span data-ttu-id="42cfe-107">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="42cfe-107">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="42cfe-108">Parameter</span><span class="sxs-lookup"><span data-stu-id="42cfe-108">Parameter</span></span>    | <span data-ttu-id="42cfe-109">Typ</span><span class="sxs-lookup"><span data-stu-id="42cfe-109">Type</span></span>   |<span data-ttu-id="42cfe-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42cfe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42cfe-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="42cfe-111">startDateTime</span></span>|<span data-ttu-id="42cfe-112">String</span><span class="sxs-lookup"><span data-stu-id="42cfe-112">String</span></span>|<span data-ttu-id="42cfe-p101">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="42cfe-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="42cfe-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="42cfe-115">endDateTime</span></span>|<span data-ttu-id="42cfe-116">String</span><span class="sxs-lookup"><span data-stu-id="42cfe-116">String</span></span>|<span data-ttu-id="42cfe-p102">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="42cfe-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="42cfe-119">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="42cfe-119">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="42cfe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42cfe-120">Request headers</span></span>
| <span data-ttu-id="42cfe-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="42cfe-121">Header</span></span>       | <span data-ttu-id="42cfe-122">Wert</span><span class="sxs-lookup"><span data-stu-id="42cfe-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42cfe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42cfe-123">Authorization</span></span>  | <span data-ttu-id="42cfe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42cfe-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="42cfe-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="42cfe-126">Prefer</span></span> | <span data-ttu-id="42cfe-127">string</span><span class="sxs-lookup"><span data-stu-id="42cfe-127">string</span></span> | <span data-ttu-id="42cfe-p104">outlook.timezone="Eastern Standard Time". Optional.  Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, wird die Antwort in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42cfe-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42cfe-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42cfe-132">Request body</span></span>
<span data-ttu-id="42cfe-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="42cfe-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42cfe-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="42cfe-134">Response</span></span>

<span data-ttu-id="42cfe-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42cfe-135">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42cfe-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42cfe-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42cfe-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42cfe-137">Request</span></span>
<span data-ttu-id="42cfe-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42cfe-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```
##### <a name="response"></a><span data-ttu-id="42cfe-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="42cfe-139">Response</span></span>
<span data-ttu-id="42cfe-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42cfe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

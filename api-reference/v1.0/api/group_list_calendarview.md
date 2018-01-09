# <a name="list-calendarview"></a><span data-ttu-id="75b60-101">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="75b60-101">List calendarView</span></span>
<span data-ttu-id="75b60-102">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender einer Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="75b60-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="75b60-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="75b60-103">Permissions</span></span>
<span data-ttu-id="75b60-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75b60-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75b60-106">Permission type</span></span>      | <span data-ttu-id="75b60-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75b60-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75b60-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75b60-108">Delegated (work or school account)</span></span> | <span data-ttu-id="75b60-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75b60-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="75b60-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75b60-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75b60-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75b60-111">Not supported.</span></span>    |
|<span data-ttu-id="75b60-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75b60-112">Application</span></span> | <span data-ttu-id="75b60-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75b60-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75b60-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75b60-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="75b60-115">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="75b60-115">Query parameters</span></span>
<span data-ttu-id="75b60-116">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="75b60-116">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="75b60-117">Parameter</span><span class="sxs-lookup"><span data-stu-id="75b60-117">Parameter</span></span>    | <span data-ttu-id="75b60-118">Typ</span><span class="sxs-lookup"><span data-stu-id="75b60-118">Type</span></span>   |<span data-ttu-id="75b60-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75b60-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75b60-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="75b60-120">startDateTime</span></span>|<span data-ttu-id="75b60-121">String</span><span class="sxs-lookup"><span data-stu-id="75b60-121">String</span></span>|<span data-ttu-id="75b60-p102">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="75b60-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="75b60-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="75b60-124">endDateTime</span></span>|<span data-ttu-id="75b60-125">String</span><span class="sxs-lookup"><span data-stu-id="75b60-125">String</span></span>|<span data-ttu-id="75b60-p103">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="75b60-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="75b60-128">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="75b60-128">This method also supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75b60-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75b60-129">Request headers</span></span>
| <span data-ttu-id="75b60-130">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="75b60-130">Header</span></span>       | <span data-ttu-id="75b60-131">Wert</span><span class="sxs-lookup"><span data-stu-id="75b60-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75b60-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="75b60-132">Authorization</span></span>  | <span data-ttu-id="75b60-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="75b60-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="75b60-135">Prefer</span><span class="sxs-lookup"><span data-stu-id="75b60-135">Prefer</span></span> | <span data-ttu-id="75b60-136">string</span><span class="sxs-lookup"><span data-stu-id="75b60-136">string</span></span> | <span data-ttu-id="75b60-p105">outlook.timezone="Eastern Standard Time". Optional.  Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, wird die Antwort in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75b60-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75b60-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75b60-141">Request body</span></span>
<span data-ttu-id="75b60-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="75b60-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75b60-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="75b60-143">Response</span></span>
<span data-ttu-id="75b60-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75b60-144">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75b60-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75b60-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="75b60-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75b60-146">Request</span></span>
<span data-ttu-id="75b60-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75b60-147">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/calendarView
```

#### <a name="response"></a><span data-ttu-id="75b60-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="75b60-148">Response</span></span>
<span data-ttu-id="75b60-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="75b60-149">Here is an example of the response.</span></span>
><span data-ttu-id="75b60-150">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="75b60-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="75b60-151">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="75b60-151">All the properties will be returned from an actual call.</span></span>
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

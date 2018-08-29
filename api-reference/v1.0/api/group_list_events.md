# <a name="list-events"></a><span data-ttu-id="fb288-101">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="fb288-101">List events</span></span>
<span data-ttu-id="fb288-102">Mit dieser API können Sie eine Liste von Objekten des Typs [event](../resources/event.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="fb288-102">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb288-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fb288-103">Permissions</span></span>
<span data-ttu-id="fb288-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb288-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fb288-106">Permission type</span></span>      | <span data-ttu-id="fb288-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fb288-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb288-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fb288-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fb288-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb288-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb288-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fb288-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb288-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb288-111">Not supported.</span></span>    |
|<span data-ttu-id="fb288-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fb288-112">Application</span></span> | <span data-ttu-id="fb288-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb288-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb288-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb288-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb288-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fb288-115">Optional query parameters</span></span>
<span data-ttu-id="fb288-116">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fb288-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb288-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fb288-117">Request headers</span></span>
| <span data-ttu-id="fb288-118">Name</span><span class="sxs-lookup"><span data-stu-id="fb288-118">Name</span></span>       | <span data-ttu-id="fb288-119">Typ</span><span class="sxs-lookup"><span data-stu-id="fb288-119">Type</span></span> | <span data-ttu-id="fb288-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fb288-120">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="fb288-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fb288-121">Authorization</span></span>  | <span data-ttu-id="fb288-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fb288-122">string</span></span> | <span data-ttu-id="fb288-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fb288-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fb288-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="fb288-125">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="fb288-126">string</span><span class="sxs-lookup"><span data-stu-id="fb288-126">string</span></span> | <span data-ttu-id="fb288-127">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="fb288-127">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="fb288-128">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb288-128">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="fb288-129">Optional.</span><span class="sxs-lookup"><span data-stu-id="fb288-129">Optional.</span></span> |
| <span data-ttu-id="fb288-130">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="fb288-130">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="fb288-131">string</span><span class="sxs-lookup"><span data-stu-id="fb288-131">string</span></span> | <span data-ttu-id="fb288-132">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="fb288-132">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="fb288-133">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="fb288-133">Values can be "text" or "html".</span></span> <span data-ttu-id="fb288-134">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="fb288-134">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="fb288-135">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb288-135">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="fb288-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="fb288-136">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb288-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fb288-137">Request body</span></span>
<span data-ttu-id="fb288-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fb288-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb288-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb288-139">Response</span></span>
<span data-ttu-id="fb288-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb288-140">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb288-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fb288-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fb288-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb288-142">Request</span></span>
<span data-ttu-id="fb288-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fb288-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```

#### <a name="response"></a><span data-ttu-id="fb288-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb288-144">Response</span></span>
<span data-ttu-id="fb288-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fb288-145">The following is an example of the response.</span></span>
><span data-ttu-id="fb288-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fb288-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
              "endDate": "0001-01-01",
              "recurrenceTimeZone": "Eastern Standard Time",
              "numberOfOccurrences": 0
          }
      },
      "attendees": [
          {
              "type": "required",
              "status": {
                  "response": "accepted",
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "HR Taskforce",
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Megan Bowen",
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
          }
      }
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

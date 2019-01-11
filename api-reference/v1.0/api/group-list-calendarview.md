---
title: calendarView auflisten
description: Möchten Sie die vorkommen, Ausnahmen und einzelne Instanzen von Ereignissen in einer Kalenderansicht von einem Zeitbereich definierten erhalten,
localization_priority: Normal
ms.openlocfilehash: 38240df7348d2d1de3576d9b2bb850c5128d8a0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817080"
---
# <a name="list-calendarview"></a><span data-ttu-id="e3ea5-103">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="e3ea5-103">List calendarView</span></span>
<span data-ttu-id="e3ea5-104">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender einer Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3ea5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3ea5-105">Permissions</span></span>
<span data-ttu-id="e3ea5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3ea5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3ea5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3ea5-108">Permission type</span></span>      | <span data-ttu-id="e3ea5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3ea5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3ea5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3ea5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e3ea5-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3ea5-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3ea5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3ea5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3ea5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3ea5-113">Not supported.</span></span>    |
|<span data-ttu-id="e3ea5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3ea5-114">Application</span></span> | <span data-ttu-id="e3ea5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3ea5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3ea5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3ea5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="e3ea5-117">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e3ea5-117">Query parameters</span></span>
<span data-ttu-id="e3ea5-118">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-118">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="e3ea5-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="e3ea5-119">Parameter</span></span>    | <span data-ttu-id="e3ea5-120">Typ</span><span class="sxs-lookup"><span data-stu-id="e3ea5-120">Type</span></span>   |<span data-ttu-id="e3ea5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3ea5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3ea5-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e3ea5-122">startDateTime</span></span>|<span data-ttu-id="e3ea5-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3ea5-123">String</span></span>|<span data-ttu-id="e3ea5-p102">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="e3ea5-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e3ea5-126">endDateTime</span></span>|<span data-ttu-id="e3ea5-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3ea5-127">String</span></span>|<span data-ttu-id="e3ea5-p103">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="e3ea5-130">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-130">This method also supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3ea5-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3ea5-131">Request headers</span></span>
| <span data-ttu-id="e3ea5-132">Name</span><span class="sxs-lookup"><span data-stu-id="e3ea5-132">Name</span></span>       | <span data-ttu-id="e3ea5-133">Typ</span><span class="sxs-lookup"><span data-stu-id="e3ea5-133">Type</span></span> | <span data-ttu-id="e3ea5-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3ea5-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="e3ea5-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3ea5-135">Authorization</span></span>  | <span data-ttu-id="e3ea5-136">string</span><span class="sxs-lookup"><span data-stu-id="e3ea5-136">string</span></span> | <span data-ttu-id="e3ea5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e3ea5-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e3ea5-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="e3ea5-140">string</span><span class="sxs-lookup"><span data-stu-id="e3ea5-140">string</span></span> | <span data-ttu-id="e3ea5-141">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e3ea5-142">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e3ea5-143">Optional.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-143">Optional.</span></span> |
| <span data-ttu-id="e3ea5-144">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="e3ea5-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="e3ea5-145">string</span><span class="sxs-lookup"><span data-stu-id="e3ea5-145">string</span></span> | <span data-ttu-id="e3ea5-146">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="e3ea5-147">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-147">Values can be "text" or "html".</span></span> <span data-ttu-id="e3ea5-148">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="e3ea5-149">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="e3ea5-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3ea5-151">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3ea5-151">Request body</span></span>
<span data-ttu-id="e3ea5-152">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3ea5-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3ea5-153">Response</span></span>
<span data-ttu-id="e3ea5-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3ea5-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3ea5-155">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e3ea5-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3ea5-156">Request</span></span>
<span data-ttu-id="e3ea5-157">Im folgenden Beispiel müssen Ereignisnachrichtentexte im Textformat zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-157">The following example requests event bodies to be returned in text format.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```

#### <a name="response"></a><span data-ttu-id="e3ea5-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3ea5-158">Response</span></span>
<span data-ttu-id="e3ea5-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-159">The following is an example of the response.</span></span>
><span data-ttu-id="e3ea5-160">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e3ea5-161">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e3ea5-161">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1354
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
    "value":[
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-14T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-14T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                 {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
             ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Follow-up meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-16T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-16T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
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
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

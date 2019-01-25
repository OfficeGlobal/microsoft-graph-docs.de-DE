---
title: calendarView auflisten
description: Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender einer Gruppe abrufen.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6abdb25e84787cd7a6430e9a00ef24a997c61e92
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522133"
---
# <a name="list-calendarview"></a><span data-ttu-id="5bbe4-103">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="5bbe4-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bbe4-104">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender einer Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bbe4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5bbe4-105">Permissions</span></span>
<span data-ttu-id="5bbe4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bbe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bbe4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5bbe4-108">Permission type</span></span>      | <span data-ttu-id="5bbe4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5bbe4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bbe4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5bbe4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5bbe4-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bbe4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5bbe4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5bbe4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bbe4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bbe4-113">Not supported.</span></span>    |
|<span data-ttu-id="5bbe4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5bbe4-114">Application</span></span> | <span data-ttu-id="5bbe4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bbe4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bbe4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bbe4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="5bbe4-117">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5bbe4-117">Query parameters</span></span>
<span data-ttu-id="5bbe4-118">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-118">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="5bbe4-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="5bbe4-119">Parameter</span></span>    | <span data-ttu-id="5bbe4-120">Typ</span><span class="sxs-lookup"><span data-stu-id="5bbe4-120">Type</span></span>   |<span data-ttu-id="5bbe4-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5bbe4-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bbe4-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5bbe4-122">startDateTime</span></span>|<span data-ttu-id="5bbe4-123">String</span><span class="sxs-lookup"><span data-stu-id="5bbe4-123">String</span></span>|<span data-ttu-id="5bbe4-p102">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="5bbe4-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5bbe4-126">endDateTime</span></span>|<span data-ttu-id="5bbe4-127">String</span><span class="sxs-lookup"><span data-stu-id="5bbe4-127">String</span></span>|<span data-ttu-id="5bbe4-p103">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="5bbe4-130">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-130">This method also supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bbe4-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5bbe4-131">Request headers</span></span>
| <span data-ttu-id="5bbe4-132">Name</span><span class="sxs-lookup"><span data-stu-id="5bbe4-132">Name</span></span>       | <span data-ttu-id="5bbe4-133">Typ</span><span class="sxs-lookup"><span data-stu-id="5bbe4-133">Type</span></span> | <span data-ttu-id="5bbe4-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5bbe4-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="5bbe4-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bbe4-135">Authorization</span></span>  | <span data-ttu-id="5bbe4-136">String</span><span class="sxs-lookup"><span data-stu-id="5bbe4-136">string</span></span> | <span data-ttu-id="5bbe4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5bbe4-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5bbe4-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="5bbe4-140">string</span><span class="sxs-lookup"><span data-stu-id="5bbe4-140">string</span></span> | <span data-ttu-id="5bbe4-141">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="5bbe4-142">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="5bbe4-143">Optional.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-143">Optional.</span></span> |
| <span data-ttu-id="5bbe4-144">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="5bbe4-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="5bbe4-145">string</span><span class="sxs-lookup"><span data-stu-id="5bbe4-145">string</span></span> | <span data-ttu-id="5bbe4-146">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="5bbe4-147">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-147">Values can be "text" or "html".</span></span> <span data-ttu-id="5bbe4-148">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="5bbe4-149">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="5bbe4-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bbe4-151">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5bbe4-151">Request body</span></span>
<span data-ttu-id="5bbe4-152">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bbe4-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bbe4-153">Response</span></span>
<span data-ttu-id="5bbe4-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bbe4-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5bbe4-155">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5bbe4-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bbe4-156">Request</span></span>
<span data-ttu-id="5bbe4-157">Im folgenden Beispiel müssen Ereignisnachrichtentexte im Textformat zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-157">The following example requests event bodies to be returned in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarviews"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```

#### <a name="response"></a><span data-ttu-id="5bbe4-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bbe4-158">Response</span></span>
<span data-ttu-id="5bbe4-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-159">The following is an example of the response.</span></span>
><span data-ttu-id="5bbe4-160">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5bbe4-161">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5bbe4-161">All the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
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
            "uid":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
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
            "uid":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-calendarview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

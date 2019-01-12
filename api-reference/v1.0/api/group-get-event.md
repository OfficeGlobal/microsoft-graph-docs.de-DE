---
title: Ereignis abrufen
description: Abrufen eines event-Objekts.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6ab5248fb7747238157f24845a244d9f4a6c2e73
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986726"
---
# <a name="get-event"></a><span data-ttu-id="f2e13-103">Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="f2e13-103">Get event</span></span>
<span data-ttu-id="f2e13-104">Abrufen eines [event](../resources/event.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f2e13-104">Get an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2e13-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f2e13-105">Permissions</span></span>
<span data-ttu-id="f2e13-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2e13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2e13-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f2e13-108">Permission type</span></span>      | <span data-ttu-id="f2e13-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f2e13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2e13-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f2e13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f2e13-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e13-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2e13-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f2e13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2e13-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2e13-113">Not supported.</span></span>    |
|<span data-ttu-id="f2e13-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f2e13-114">Application</span></span> | <span data-ttu-id="f2e13-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f2e13-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2e13-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2e13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2e13-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f2e13-117">Optional query parameters</span></span>
<span data-ttu-id="f2e13-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f2e13-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2e13-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f2e13-119">Request headers</span></span>
| <span data-ttu-id="f2e13-120">Name</span><span class="sxs-lookup"><span data-stu-id="f2e13-120">Name</span></span>       | <span data-ttu-id="f2e13-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f2e13-121">Type</span></span> | <span data-ttu-id="f2e13-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2e13-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="f2e13-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e13-123">Authorization</span></span>  | <span data-ttu-id="f2e13-124">string</span><span class="sxs-lookup"><span data-stu-id="f2e13-124">string</span></span> | <span data-ttu-id="f2e13-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2e13-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f2e13-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f2e13-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="f2e13-128">string</span><span class="sxs-lookup"><span data-stu-id="f2e13-128">string</span></span> | <span data-ttu-id="f2e13-129">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="f2e13-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f2e13-130">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2e13-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f2e13-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="f2e13-131">Optional.</span></span> |
| <span data-ttu-id="f2e13-132">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f2e13-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f2e13-133">string</span><span class="sxs-lookup"><span data-stu-id="f2e13-133">string</span></span> | <span data-ttu-id="f2e13-134">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="f2e13-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="f2e13-135">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="f2e13-135">Values can be "text" or "html".</span></span> <span data-ttu-id="f2e13-136">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="f2e13-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="f2e13-137">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2e13-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="f2e13-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="f2e13-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2e13-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f2e13-139">Request body</span></span>
<span data-ttu-id="f2e13-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f2e13-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2e13-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2e13-141">Response</span></span>
<span data-ttu-id="f2e13-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f2e13-142">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e13-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f2e13-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f2e13-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f2e13-144">Request</span></span>
<span data-ttu-id="f2e13-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f2e13-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "get_group_event"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="f2e13-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="f2e13-146">Response</span></span>
<span data-ttu-id="f2e13-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f2e13-147">The following is an example of the response.</span></span>
><span data-ttu-id="f2e13-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f2e13-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
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
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
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
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
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
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

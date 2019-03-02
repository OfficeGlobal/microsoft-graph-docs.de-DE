---
title: Ereignis erstellen
description: Mit dieser API können Sie neue Ereignisse im Standardkalender oder dem jeweils angegebenen Kalender erstellen.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e974bd17b4fe1b1f43e743cbcacbb2104a3888fc
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342296"
---
# <a name="create-event"></a><span data-ttu-id="bea1a-103">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="bea1a-103">Create event</span></span>

<span data-ttu-id="bea1a-104">Mit dieser API können Sie neue Ereignisse im Standardkalender oder dem jeweils angegebenen Kalender erstellen.</span><span class="sxs-lookup"><span data-stu-id="bea1a-104">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="bea1a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bea1a-105">Permissions</span></span>
<span data-ttu-id="bea1a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bea1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bea1a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bea1a-108">Permission type</span></span>      | <span data-ttu-id="bea1a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bea1a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bea1a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bea1a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bea1a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bea1a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bea1a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bea1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bea1a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bea1a-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bea1a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bea1a-114">Application</span></span> | <span data-ttu-id="bea1a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bea1a-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bea1a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bea1a-116">HTTP request</span></span>
<span data-ttu-id="bea1a-117"><!-- { "blockType": "ignored" } --> Der [Standardkalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="bea1a-117">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="bea1a-118">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="bea1a-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="bea1a-119">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="bea1a-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="bea1a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bea1a-120">Request headers</span></span>
| <span data-ttu-id="bea1a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bea1a-121">Header</span></span>       | <span data-ttu-id="bea1a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bea1a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bea1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bea1a-123">Authorization</span></span>  | <span data-ttu-id="bea1a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bea1a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bea1a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bea1a-126">Content-Type</span></span>  | <span data-ttu-id="bea1a-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="bea1a-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bea1a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bea1a-129">Request body</span></span>
<span data-ttu-id="bea1a-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bea1a-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bea1a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="bea1a-131">Response</span></span>

<span data-ttu-id="bea1a-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bea1a-132">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bea1a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bea1a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bea1a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bea1a-134">Request</span></span>
<span data-ttu-id="bea1a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bea1a-135">Here is an example of the request.</span></span>
<span data-ttu-id="bea1a-136">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bea1a-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does mid month work for you?"
  },
  "start": {
      "dateTime": "2019-03-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="bea1a-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="bea1a-137">Response</span></span>
<span data-ttu-id="bea1a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bea1a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA=",
    "createdDateTime": "2019-02-28T21:17:57.56197Z",
    "lastModifiedDateTime": "2019-02-28T21:17:59.044919Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E641B4C",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does mid month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes mid month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-15T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Megan Bowen",
            "address": "MeganB@contoso.OnMicrosoft.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

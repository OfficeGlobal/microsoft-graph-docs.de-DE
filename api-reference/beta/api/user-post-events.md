---
title: Ereignis erstellen
description: Erstellen eines Ereignisses im Standardkalender des Benutzers oder in einem angegebenen Kalender.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b9d18d4674bbce68d9e7bcadbad0a2400e6d287f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947552"
---
# <a name="create-event"></a><span data-ttu-id="4537e-103">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="4537e-103">Create Event</span></span>

> <span data-ttu-id="4537e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4537e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4537e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4537e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4537e-106">Erstellen eines [Ereignisses](../resources/event.md) im Standardkalender des Benutzers oder in einem angegebenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="4537e-106">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="4537e-107">Sie können die Zeitzone für alle Start- und Endzeiten des Ereignisses als Teil dieser Werte angeben, da die **start**- und **end**-Eigenschaft vom Typ [dateTimeTimeZone](../resources/datetimetimezone.md) sind.</span><span class="sxs-lookup"><span data-stu-id="4537e-107">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span>

<span data-ttu-id="4537e-108">Wenn ein Ereignis gesendet wird, sendet der Server Einladungen an alle Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="4537e-108">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="4537e-109">**Festlegen des Ortes in einer Einladung**</span><span class="sxs-lookup"><span data-stu-id="4537e-109">**Setting the location in an event**</span></span>

<span data-ttu-id="4537e-110">Ein Exchange-Administrator kann ein Postfach und eine E-Mail-Adresse für eine Ressource, z. B. einen Besprechungsraum, oder Geräte, z B. einen Projektor, einrichten.</span><span class="sxs-lookup"><span data-stu-id="4537e-110">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="4537e-111">Benutzer können die Ressource als Teilnehmer zu einer Besprechung einladen.</span><span class="sxs-lookup"><span data-stu-id="4537e-111">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="4537e-112">Der Server akzeptiert im Auftrag der Ressource die Besprechungsanfrage basierend auf dem Frei/Gebucht-Zeitplan der Ressource oder lehnt diese ab.</span><span class="sxs-lookup"><span data-stu-id="4537e-112">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span>
<span data-ttu-id="4537e-113">Wenn der Server eine Besprechung für die Ressource akzeptiert, wird ein Ereignis für die Besprechung im Kalender der Ressource erstellt.</span><span class="sxs-lookup"><span data-stu-id="4537e-113">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="4537e-114">Wenn die Besprechung neu geplant wird, aktualisiert der Server das Ereignis im Kalender der Ressource automatisch.</span><span class="sxs-lookup"><span data-stu-id="4537e-114">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="4537e-115">Ein weiterer Vorteil beim Einrichten eines Postfachs für eine Ressource ist das Steuern des Zeitplans der Ressource derart, dass z. B. nur Führungskräfte oder deren Stellvertretungen einen privaten Besprechungsraum buchen können.</span><span class="sxs-lookup"><span data-stu-id="4537e-115">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="4537e-116">Gehen Sie folgendermaßen vor, wenn Sie ein Ereignis organisieren, bei dem ein Besprechungsort vorhanden ist:</span><span class="sxs-lookup"><span data-stu-id="4537e-116">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="4537e-117">Legen Sie die **location**-Eigenschaft des **Ereignisses** entsprechend fest.</span><span class="sxs-lookup"><span data-stu-id="4537e-117">Set the **location** property of the **event** accordingly.</span></span>
2. <span data-ttu-id="4537e-118">Legen Sie die optionale **locationEmailAddress**-Eigenschaft fest, wenn der Besprechungsort eine E-Mail-Adresse aufweist.</span><span class="sxs-lookup"><span data-stu-id="4537e-118">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="4537e-119">Führen Sie die folgenden zusätzlichen Schritte aus, wenn der Besprechungsort als Ressource eingerichtet wurde oder wenn das Ereignis Geräte umfasst, die als Ressource eingerichtet wurden:</span><span class="sxs-lookup"><span data-stu-id="4537e-119">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="4537e-120">Laden Sie die Ressource als [Teilnehmer](../resources/attendee.md) ein.</span><span class="sxs-lookup"><span data-stu-id="4537e-120">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="4537e-121">Legen Sie die **type**-Eigenschaft des Teilnehmers auf `resource` fest.</span><span class="sxs-lookup"><span data-stu-id="4537e-121">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="4537e-122">Legen Sie die **emailAddress** des Teilnehmers als E-Mail-Adresse der Ressource fest.</span><span class="sxs-lookup"><span data-stu-id="4537e-122">Set the attendee **emailAddress** as the resource email address.</span></span>


## <a name="permissions"></a><span data-ttu-id="4537e-123">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4537e-123">Permissions</span></span>
<span data-ttu-id="4537e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4537e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4537e-126">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4537e-126">Permission type</span></span>      | <span data-ttu-id="4537e-127">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4537e-127">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4537e-128">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4537e-128">Delegated (work or school account)</span></span> | <span data-ttu-id="4537e-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4537e-129">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4537e-130">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4537e-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4537e-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4537e-131">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4537e-132">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4537e-132">Application</span></span> | <span data-ttu-id="4537e-133">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4537e-133">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4537e-134">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4537e-134">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="4537e-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4537e-135">Request headers</span></span>
| <span data-ttu-id="4537e-136">Header</span><span class="sxs-lookup"><span data-stu-id="4537e-136">Header</span></span>       | <span data-ttu-id="4537e-137">Wert</span><span class="sxs-lookup"><span data-stu-id="4537e-137">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="4537e-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="4537e-138">Authorization</span></span>  | <span data-ttu-id="4537e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4537e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4537e-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4537e-141">Content-Type</span></span>  | <span data-ttu-id="4537e-p105">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="4537e-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4537e-144">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4537e-144">Request body</span></span>
<span data-ttu-id="4537e-145">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4537e-145">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="4537e-146">Da die **event**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie den `POST`-Vorgang verwenden und während der Erstellung des Ereignisses benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="4537e-146">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="4537e-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="4537e-147">Response</span></span>

<span data-ttu-id="4537e-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4537e-148">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4537e-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4537e-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="4537e-150">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="4537e-150">Request 1</span></span>
<span data-ttu-id="4537e-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4537e-151">Here is an example of the request.</span></span> <span data-ttu-id="4537e-152">Es verwendet den `Prefer: outlook.timezone`-Anforderungsheader, um die **Start**- und **End**zeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="4537e-152">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="4537e-153">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4537e-153">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="4537e-154">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="4537e-154">Response 1</span></span>
<span data-ttu-id="4537e-155">Nachfolgend finden Sie ein Beispiel der Antwort, in der die Eigenschaften **start** und **end** die im `Prefer: outlook.timezone`-Header angegebene Zeitzone verwenden.</span><span class="sxs-lookup"><span data-stu-id="4537e-155">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span>
<span data-ttu-id="4537e-156">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="4537e-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4537e-157">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4537e-157">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "uid":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
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
            "uniqueIdType": "unknown"
        }
    ],
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="4537e-158">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="4537e-158">Request 2</span></span>
<span data-ttu-id="4537e-159">In der nächsten Beispielanforderung werden drei Orte angegeben, an denen der Organisator und Teilnehmer an der Besprechung teilnehmen können.</span><span class="sxs-lookup"><span data-stu-id="4537e-159">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="4537e-160">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4537e-160">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_multiple_locations"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 1390

{
  "subject": "Plan summer company picnic",
  "body": {
    "contentType": "HTML",
    "content": "Let's kick-start this event planning!"
  },
  "start": {
      "dateTime": "2017-08-30T11:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-08-30T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "DanaS@contoso.onmicrosoft.com",
        "name": "Dana Swope"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "AlexW@contoso.onmicrosoft.com",
        "name": "Alex Wilber"
      },
      "type": "Required"
    }
  ],
  "location": {
    "displayName": "Conf Room 3; Fourth Coffee; Home Office",
    "locationType": "Default"
  },
  "locations": [
    {
      "displayName": "Conf Room 3"
    },
    {
      "displayName": "Fourth Coffee",
      "address": {
        "street": "4567 Main St",
        "city": "Redmond",
        "state": "WA",
        "countryOrRegion": "US",
        "postalCode": "32008"
      },
      "coordinates": {
        "latitude": 47.672,
        "longitude": -102.103
      }
    },
    {
      "displayName": "Home Office"
    }
  ]

}
```

##### <a name="response-2"></a><span data-ttu-id="4537e-161">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="4537e-161">Response 2</span></span>
<span data-ttu-id="4537e-162">Im folgenden Antwortbeispiel ist das erstellte Ereignis dargestellt, das Informationen für die drei Standorte für die Besprechung angibt.</span><span class="sxs-lookup"><span data-stu-id="4537e-162">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="4537e-163">Aufgrund des `Prefer: outlook.timezone="Pacific Standard Time"`-Anforderungsheaders werden die Eigenschaften **start** und **end** in PST ausgedrückt.</span><span class="sxs-lookup"><span data-stu-id="4537e-163">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="4537e-164">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="4537e-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4537e-165">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4537e-165">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2985

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "createdDateTime":"2017-08-30T07:06:33.8673345Z",
  "lastModifiedDateTime":"2017-08-30T07:06:34.5079772Z",
  "changeKey":"y53lbKh6jkaxHzFwGhgyxgAAz3IKMA==",
  "categories":[

  ],
  "originalStartTimeZone":"Pacific Standard Time",
  "originalEndTimeZone":"Pacific Standard Time",
  "uid":"04000000820089190544",
  "reminderMinutesBeforeStart":15,
  "isReminderOn":true,
  "hasAttachments":false,
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "importance":"normal",
  "sensitivity":"normal",
  "isAllDay":false,
  "isCancelled":false,
  "isOrganizer":true,
  "responseRequested":true,
  "seriesMasterId":null,
  "showAs":"busy",
  "type":"singleInstance",
  "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADAGAADDdm4NAAA%3D&exvsurl=1&path=/calendar/item",
  "onlineMeetingUrl":null,
  "responseStatus":{
    "response":"organizer",
    "time":"0001-01-01T00:00:00Z"
  },
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
    }
  ],
  "recurrence":null,
  "attendees":[
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```


##### <a name="request-3"></a><span data-ttu-id="4537e-166">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="4537e-166">Request 3</span></span>
<span data-ttu-id="4537e-167">Das dritte Beispiel zeigt, wie ein wiederkehrendes Ereignis erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="4537e-167">The third example shows how to create a recurring event.</span></span> <span data-ttu-id="4537e-168">Das Ereignis findet jeden Montag von 12:00 Uhr bis 2:00 Uhr beginnend am 4. September 2017 bis zum Jahresende statt.</span><span class="sxs-lookup"><span data-stu-id="4537e-168">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon time work for you?"
  },
  "start": {
      "dateTime": "2017-09-04T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-09-04T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "recurrence": {
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Monday" ]
    },
    "range": {
      "type": "endDate",
      "startDate": "2017-09-04",
      "endDate": "2017-12-31"
    }
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="4537e-169">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4537e-169">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="4537e-170">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="4537e-170">Response 3</span></span>
<span data-ttu-id="4537e-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4537e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==\"",
    "id":"AAMkADQwMD",
    "createdDateTime":"2017-10-07T04:59:12.9698856Z",
    "lastModifiedDateTime":"2017-10-07T04:59:13.8136423Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "uid":"040000008200E00074C5B7101A82E0080000000028CEBE04293FD3010000000000000000100000009F85AB8AF8ED4D4FAC777FA89954BDB7",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go for lunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMD&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start":{
        "dateTime":"2017-09-04T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-09-04T14:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar",
        "locationType":"default",
        "uniqueId":"Harry's Bar",
        "uniqueIdType":"private"
    },
    "locations":[
        {
            "displayName":"Harry's Bar",
            "locationType":"default",
            "uniqueIdType":"unknown"
        }
    ],
    "recurrence":{
        "pattern":{
            "type":"weekly",
            "interval":1,
            "month":0,
            "dayOfMonth":0,
            "daysOfWeek":[
                "monday"
            ],
            "firstDayOfWeek":"sunday",
            "index":"first"
        },
        "range":{
            "type":"endDate",
            "startDate":"2017-09-04",
            "endDate":"2017-12-31",
            "recurrenceTimeZone":"Pacific Standard Time",
            "numberOfOccurrences":0
        }
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
        }
    },
    "OnlineMeeting":null
}
```




## <a name="see-also"></a><span data-ttu-id="4537e-174">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="4537e-174">See also</span></span>

- [<span data-ttu-id="4537e-175">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="4537e-175">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4537e-176">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="4537e-176">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4537e-177">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="4537e-177">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

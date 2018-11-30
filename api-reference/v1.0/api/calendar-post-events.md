---
title: Ereignis erstellen
description: Mit dieser API können Sie neue Ereignisse im Standardkalender oder dem jeweils angegebenen Kalender erstellen.
ms.openlocfilehash: da06df89ab4a62a1b767635e3daa928f84f29d9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018363"
---
# <a name="create-event"></a><span data-ttu-id="b6665-103">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="b6665-103">Create Event</span></span>

<span data-ttu-id="b6665-104">Mit dieser API können Sie neue Ereignisse im Standardkalender oder dem jeweils angegebenen Kalender erstellen.</span><span class="sxs-lookup"><span data-stu-id="b6665-104">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6665-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b6665-105">Permissions</span></span>
<span data-ttu-id="b6665-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6665-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6665-108">Permission type</span></span>      | <span data-ttu-id="b6665-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6665-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6665-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6665-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6665-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6665-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b6665-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6665-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6665-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6665-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b6665-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6665-114">Application</span></span> | <span data-ttu-id="b6665-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6665-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6665-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6665-116">HTTP request</span></span>
<span data-ttu-id="b6665-117"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="b6665-117"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="b6665-118">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b6665-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="b6665-119">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b6665-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="b6665-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6665-120">Request headers</span></span>
| <span data-ttu-id="b6665-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b6665-121">Header</span></span>       | <span data-ttu-id="b6665-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b6665-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b6665-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6665-123">Authorization</span></span>  | <span data-ttu-id="b6665-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b6665-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b6665-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6665-126">Content-Type</span></span>  | <span data-ttu-id="b6665-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="b6665-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6665-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6665-129">Request body</span></span>
<span data-ttu-id="b6665-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [Event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b6665-130">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b6665-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6665-131">Response</span></span>

<span data-ttu-id="b6665-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6665-132">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6665-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6665-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6665-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6665-134">Request</span></span>
<span data-ttu-id="b6665-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6665-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="b6665-136">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b6665-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b6665-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6665-137">Response</span></span>
<span data-ttu-id="b6665-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6665-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
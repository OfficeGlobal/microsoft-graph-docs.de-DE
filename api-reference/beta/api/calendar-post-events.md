---
title: Ereignis erstellen
description: Mit dieser API können Sie neue Ereignisse im Standardkalender oder dem jeweils angegebenen Kalender erstellen.
ms.openlocfilehash: df94be6e6d007d52d36b5256e149431e16cb0a2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061632"
---
# <a name="create-event"></a><span data-ttu-id="06de7-103">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="06de7-103">Create Event</span></span>

> <span data-ttu-id="06de7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06de7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06de7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06de7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06de7-106">Mit dieser API können Sie neue Ereignisse im Standardkalender oder dem jeweils angegebenen Kalender erstellen.</span><span class="sxs-lookup"><span data-stu-id="06de7-106">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="06de7-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06de7-107">Permissions</span></span>
<span data-ttu-id="06de7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06de7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06de7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06de7-110">Permission type</span></span>      | <span data-ttu-id="06de7-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06de7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06de7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06de7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06de7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06de7-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="06de7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06de7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06de7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06de7-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="06de7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06de7-116">Application</span></span> | <span data-ttu-id="06de7-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06de7-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="06de7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06de7-118">HTTP request</span></span>
<span data-ttu-id="06de7-119"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="06de7-119"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="06de7-120">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="06de7-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="06de7-121">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="06de7-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="06de7-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06de7-122">Request headers</span></span>
| <span data-ttu-id="06de7-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="06de7-123">Header</span></span>       | <span data-ttu-id="06de7-124">Wert</span><span class="sxs-lookup"><span data-stu-id="06de7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06de7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="06de7-125">Authorization</span></span>  | <span data-ttu-id="06de7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06de7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="06de7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06de7-128">Content-Type</span></span>  | <span data-ttu-id="06de7-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="06de7-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06de7-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06de7-131">Request body</span></span>
<span data-ttu-id="06de7-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [Event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="06de7-132">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="06de7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="06de7-133">Response</span></span>

<span data-ttu-id="06de7-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06de7-134">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06de7-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06de7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06de7-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06de7-136">Request</span></span>
<span data-ttu-id="06de7-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06de7-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="06de7-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="06de7-138">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="06de7-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="06de7-139">Response</span></span>
<span data-ttu-id="06de7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06de7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
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

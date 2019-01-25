---
title: Ereignis erstellen
description: Mit dieser API können Sie neue Ereignisse im Standardkalender oder dem jeweils angegebenen Kalender erstellen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7cd5c6ddf9834163bdd3b03dd2ab2aa36cd3b48b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516329"
---
# <a name="create-event"></a><span data-ttu-id="b7ce7-103">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="b7ce7-103">Create Event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7ce7-104">Mit dieser API können Sie neue Ereignisse im Standardkalender oder dem jeweils angegebenen Kalender erstellen.</span><span class="sxs-lookup"><span data-stu-id="b7ce7-104">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7ce7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b7ce7-105">Permissions</span></span>
<span data-ttu-id="b7ce7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7ce7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7ce7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7ce7-108">Permission type</span></span>      | <span data-ttu-id="b7ce7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7ce7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7ce7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7ce7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7ce7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7ce7-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b7ce7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7ce7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7ce7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7ce7-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b7ce7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7ce7-114">Application</span></span> | <span data-ttu-id="b7ce7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7ce7-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7ce7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7ce7-116">HTTP request</span></span>
<span data-ttu-id="b7ce7-117"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="b7ce7-117"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="b7ce7-118">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b7ce7-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="b7ce7-119">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b7ce7-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="b7ce7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7ce7-120">Request headers</span></span>
| <span data-ttu-id="b7ce7-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b7ce7-121">Header</span></span>       | <span data-ttu-id="b7ce7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b7ce7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7ce7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7ce7-123">Authorization</span></span>  | <span data-ttu-id="b7ce7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b7ce7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b7ce7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7ce7-126">Content-Type</span></span>  | <span data-ttu-id="b7ce7-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="b7ce7-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7ce7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b7ce7-129">Request body</span></span>
<span data-ttu-id="b7ce7-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [Event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b7ce7-130">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b7ce7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7ce7-131">Response</span></span>

<span data-ttu-id="b7ce7-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7ce7-132">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7ce7-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7ce7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7ce7-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7ce7-134">Request</span></span>
<span data-ttu-id="b7ce7-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7ce7-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="b7ce7-136">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b7ce7-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b7ce7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7ce7-137">Response</span></span>
<span data-ttu-id="b7ce7-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7ce7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-post-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

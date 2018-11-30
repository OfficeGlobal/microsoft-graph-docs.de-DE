---
title: calendarView auflisten
description: Möchten Sie die vorkommen, Ausnahmen und einzelne Instanzen von Ereignissen in einer Kalenderansicht von einem Zeitbereich definierten erhalten,
ms.openlocfilehash: dab33fe00029e00aac38d11a9142966dbab4d487
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058071"
---
# <a name="list-calendarview"></a><span data-ttu-id="f185c-103">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="f185c-103">List calendarView</span></span>

> <span data-ttu-id="f185c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f185c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f185c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f185c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f185c-106">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender `(../me/calendarview)` eines Benutzers oder einer Gruppe oder aus einem anderen Kalender des Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="f185c-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="f185c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f185c-107">Permissions</span></span>
<span data-ttu-id="f185c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f185c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f185c-110">Ereignisse im Kalender eines Benutzers: Calendars.Read or Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f185c-110">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="f185c-111">Ereignisse in einem Gruppenkalender: Group.Read.All or Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f185c-111">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f185c-112">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f185c-112">HTTP request</span></span>
<span data-ttu-id="f185c-113"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="f185c-113"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="f185c-114">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="f185c-114">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="f185c-115">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="f185c-115">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="f185c-116">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f185c-116">Query parameters</span></span>

<span data-ttu-id="f185c-117">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="f185c-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="f185c-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="f185c-118">Parameter</span></span>    | <span data-ttu-id="f185c-119">Typ</span><span class="sxs-lookup"><span data-stu-id="f185c-119">Type</span></span>   |<span data-ttu-id="f185c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f185c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f185c-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f185c-121">startDateTime</span></span>|<span data-ttu-id="f185c-122">String</span><span class="sxs-lookup"><span data-stu-id="f185c-122">String</span></span>|<span data-ttu-id="f185c-p103">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="f185c-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="f185c-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f185c-125">endDateTime</span></span>|<span data-ttu-id="f185c-126">String</span><span class="sxs-lookup"><span data-stu-id="f185c-126">String</span></span>|<span data-ttu-id="f185c-p104">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="f185c-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="f185c-129">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f185c-129">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f185c-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f185c-130">Request headers</span></span>
| <span data-ttu-id="f185c-131">Name</span><span class="sxs-lookup"><span data-stu-id="f185c-131">Name</span></span>       | <span data-ttu-id="f185c-132">Typ</span><span class="sxs-lookup"><span data-stu-id="f185c-132">Type</span></span> | <span data-ttu-id="f185c-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f185c-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="f185c-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f185c-134">Authorization</span></span>  | <span data-ttu-id="f185c-135">string</span><span class="sxs-lookup"><span data-stu-id="f185c-135">string</span></span> | <span data-ttu-id="f185c-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f185c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f185c-138">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f185c-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="f185c-139">string</span><span class="sxs-lookup"><span data-stu-id="f185c-139">string</span></span> | <span data-ttu-id="f185c-140">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="f185c-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f185c-141">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f185c-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f185c-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="f185c-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f185c-143">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f185c-143">Request body</span></span>
<span data-ttu-id="f185c-144">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f185c-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f185c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="f185c-145">Response</span></span>

<span data-ttu-id="f185c-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f185c-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f185c-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f185c-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f185c-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f185c-148">Request</span></span>
<span data-ttu-id="f185c-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f185c-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="f185c-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="f185c-150">Response</span></span>
<span data-ttu-id="f185c-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f185c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "response-value",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
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

---
title: calendarView auflisten
description: Möchten Sie die vorkommen, Ausnahmen und einzelne Instanzen von Ereignissen in einer Kalenderansicht von einem Zeitbereich definierten erhalten,
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dfc0d378a48716f70753b38d1970f0d4017a13a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986334"
---
# <a name="list-calendarview"></a><span data-ttu-id="17b1c-103">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="17b1c-103">List calendarView</span></span>

<span data-ttu-id="17b1c-104">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender `(../me/calendarview)` eines Benutzers oder einer Gruppe oder aus einem anderen Kalender des Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="17b1c-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="17b1c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="17b1c-105">Permissions</span></span>
<span data-ttu-id="17b1c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17b1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="17b1c-108">Ereignisse im Kalender eines Benutzers: Calendars.Read or Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17b1c-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="17b1c-109">Ereignisse in einem Gruppenkalender: Group.Read.All or Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b1c-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="17b1c-110">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17b1c-110">HTTP request</span></span>

<span data-ttu-id="17b1c-111">Der Standard[kalender](../resources/calendar.md) eines Benutzers oder einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="17b1c-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="17b1c-112">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="17b1c-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="17b1c-113">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="17b1c-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="17b1c-114">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="17b1c-114">Query parameters</span></span>

<span data-ttu-id="17b1c-115">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="17b1c-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="17b1c-116">Parameter</span><span class="sxs-lookup"><span data-stu-id="17b1c-116">Parameter</span></span>    | <span data-ttu-id="17b1c-117">Typ</span><span class="sxs-lookup"><span data-stu-id="17b1c-117">Type</span></span>   |<span data-ttu-id="17b1c-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17b1c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17b1c-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="17b1c-119">startDateTime</span></span>|<span data-ttu-id="17b1c-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17b1c-120">String</span></span>|<span data-ttu-id="17b1c-p102">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="17b1c-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="17b1c-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="17b1c-123">endDateTime</span></span>|<span data-ttu-id="17b1c-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17b1c-124">String</span></span>|<span data-ttu-id="17b1c-p103">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="17b1c-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="17b1c-127">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="17b1c-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="17b1c-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17b1c-128">Request headers</span></span>
| <span data-ttu-id="17b1c-129">Name</span><span class="sxs-lookup"><span data-stu-id="17b1c-129">Name</span></span>       | <span data-ttu-id="17b1c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="17b1c-130">Type</span></span> | <span data-ttu-id="17b1c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17b1c-131">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="17b1c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="17b1c-132">Authorization</span></span>  | <span data-ttu-id="17b1c-133">string</span><span class="sxs-lookup"><span data-stu-id="17b1c-133">string</span></span> | <span data-ttu-id="17b1c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="17b1c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="17b1c-136">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="17b1c-136">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="17b1c-137">string</span><span class="sxs-lookup"><span data-stu-id="17b1c-137">string</span></span> | <span data-ttu-id="17b1c-138">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="17b1c-138">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="17b1c-139">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17b1c-139">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="17b1c-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="17b1c-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17b1c-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17b1c-141">Request body</span></span>
<span data-ttu-id="17b1c-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="17b1c-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17b1c-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="17b1c-143">Response</span></span>

<span data-ttu-id="17b1c-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17b1c-144">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17b1c-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17b1c-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17b1c-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17b1c-146">Request</span></span>
<span data-ttu-id="17b1c-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17b1c-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="17b1c-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="17b1c-148">Response</span></span>
<span data-ttu-id="17b1c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17b1c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
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

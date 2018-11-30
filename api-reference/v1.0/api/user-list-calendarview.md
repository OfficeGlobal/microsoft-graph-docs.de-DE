---
title: calendarView auflisten
description: 'Abrufen der vorkommen, Ausnahmen und einzelne Instanzen von Ereignissen in einer Kalenderansicht durch ein Zeitbereich, von dem Benutzer Standardkalender definiert, '
ms.openlocfilehash: db2c0b4d5fe2b3929aab7c30e00aff0f30dff5b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016886"
---
# <a name="list-calendarview"></a><span data-ttu-id="5c3aa-103">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="5c3aa-103">List calendarView</span></span>

<span data-ttu-id="5c3aa-104">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender des Benutzers oder aus einem seiner anderen Kalender abrufen.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c3aa-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5c3aa-105">Permissions</span></span>
<span data-ttu-id="5c3aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c3aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c3aa-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c3aa-108">Permission type</span></span>      | <span data-ttu-id="5c3aa-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c3aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c3aa-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c3aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c3aa-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c3aa-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5c3aa-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c3aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c3aa-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c3aa-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5c3aa-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c3aa-114">Application</span></span> | <span data-ttu-id="5c3aa-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c3aa-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c3aa-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c3aa-116">HTTP request</span></span>

<span data-ttu-id="5c3aa-117">Der standardmäßige [Kalender](../resources/calendar.md) eines Benutzers:</span><span class="sxs-lookup"><span data-stu-id="5c3aa-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="5c3aa-118">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="5c3aa-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="5c3aa-119">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="5c3aa-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="5c3aa-120">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5c3aa-120">Query parameters</span></span>

<span data-ttu-id="5c3aa-121">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="5c3aa-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="5c3aa-122">Parameter</span></span>    | <span data-ttu-id="5c3aa-123">Typ</span><span class="sxs-lookup"><span data-stu-id="5c3aa-123">Type</span></span>   |<span data-ttu-id="5c3aa-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c3aa-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c3aa-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5c3aa-125">startDateTime</span></span>|<span data-ttu-id="5c3aa-126">String</span><span class="sxs-lookup"><span data-stu-id="5c3aa-126">String</span></span>|<span data-ttu-id="5c3aa-p102">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="5c3aa-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5c3aa-129">endDateTime</span></span>|<span data-ttu-id="5c3aa-130">String</span><span class="sxs-lookup"><span data-stu-id="5c3aa-130">String</span></span>|<span data-ttu-id="5c3aa-p103">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="5c3aa-133">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5c3aa-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c3aa-134">Request headers</span></span>
| <span data-ttu-id="5c3aa-135">Name</span><span class="sxs-lookup"><span data-stu-id="5c3aa-135">Name</span></span>       | <span data-ttu-id="5c3aa-136">Typ</span><span class="sxs-lookup"><span data-stu-id="5c3aa-136">Type</span></span> | <span data-ttu-id="5c3aa-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c3aa-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="5c3aa-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c3aa-138">Authorization</span></span>  | <span data-ttu-id="5c3aa-139">string</span><span class="sxs-lookup"><span data-stu-id="5c3aa-139">string</span></span> | <span data-ttu-id="5c3aa-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5c3aa-142">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5c3aa-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="5c3aa-143">string</span><span class="sxs-lookup"><span data-stu-id="5c3aa-143">string</span></span> | <span data-ttu-id="5c3aa-144">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="5c3aa-145">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="5c3aa-146">Optional.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-146">Optional.</span></span> |
| <span data-ttu-id="5c3aa-147">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="5c3aa-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="5c3aa-148">string</span><span class="sxs-lookup"><span data-stu-id="5c3aa-148">string</span></span> | <span data-ttu-id="5c3aa-149">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="5c3aa-150">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-150">Values can be "text" or "html".</span></span> <span data-ttu-id="5c3aa-151">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="5c3aa-152">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="5c3aa-153">Optional.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c3aa-154">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c3aa-154">Request body</span></span>
<span data-ttu-id="5c3aa-155">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c3aa-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c3aa-156">Response</span></span>

<span data-ttu-id="5c3aa-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-157">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c3aa-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c3aa-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c3aa-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c3aa-159">Request</span></span>
<span data-ttu-id="5c3aa-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="5c3aa-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c3aa-161">Response</span></span>
<span data-ttu-id="5c3aa-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c3aa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "",
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

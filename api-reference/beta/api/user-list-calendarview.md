---
title: calendarView auflisten
description: Abrufen der vorkommen, Ausnahmen und einzelne Instanzen von Ereignissen in einer Kalenderansicht durch ein Zeitbereich, von dem Benutzer Standardkalender definiert,
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 57c3f184b89db2c0aa983c84db42f7bef1fc5269
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934961"
---
# <a name="list-calendarview"></a><span data-ttu-id="4afa2-103">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="4afa2-103">List calendarView</span></span>

> <span data-ttu-id="4afa2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4afa2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4afa2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4afa2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4afa2-106">Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender des Benutzers oder aus einem seiner anderen Kalender abrufen.</span><span class="sxs-lookup"><span data-stu-id="4afa2-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="4afa2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4afa2-107">Permissions</span></span>
<span data-ttu-id="4afa2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4afa2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4afa2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4afa2-110">Permission type</span></span>      | <span data-ttu-id="4afa2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4afa2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4afa2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4afa2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4afa2-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4afa2-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4afa2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4afa2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4afa2-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4afa2-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4afa2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4afa2-116">Application</span></span> | <span data-ttu-id="4afa2-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4afa2-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4afa2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4afa2-118">HTTP request</span></span>
<span data-ttu-id="4afa2-119">Der standardmäßige [Kalender](../resources/calendar.md) eines Benutzers:</span><span class="sxs-lookup"><span data-stu-id="4afa2-119">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="4afa2-120">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="4afa2-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="4afa2-121">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="4afa2-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="4afa2-122">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4afa2-122">Query parameters</span></span>

<span data-ttu-id="4afa2-123">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="4afa2-123">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="4afa2-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="4afa2-124">Parameter</span></span>    | <span data-ttu-id="4afa2-125">Typ</span><span class="sxs-lookup"><span data-stu-id="4afa2-125">Type</span></span>   |<span data-ttu-id="4afa2-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4afa2-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4afa2-127">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4afa2-127">startDateTime</span></span>|<span data-ttu-id="4afa2-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4afa2-128">String</span></span>|<span data-ttu-id="4afa2-p103">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="4afa2-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="4afa2-131">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4afa2-131">endDateTime</span></span>|<span data-ttu-id="4afa2-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4afa2-132">String</span></span>|<span data-ttu-id="4afa2-p104">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="4afa2-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="4afa2-135">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4afa2-135">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4afa2-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4afa2-136">Request headers</span></span>
| <span data-ttu-id="4afa2-137">Name</span><span class="sxs-lookup"><span data-stu-id="4afa2-137">Name</span></span>       | <span data-ttu-id="4afa2-138">Typ</span><span class="sxs-lookup"><span data-stu-id="4afa2-138">Type</span></span> | <span data-ttu-id="4afa2-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4afa2-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="4afa2-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="4afa2-140">Authorization</span></span>  | <span data-ttu-id="4afa2-141">string</span><span class="sxs-lookup"><span data-stu-id="4afa2-141">string</span></span> | <span data-ttu-id="4afa2-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4afa2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4afa2-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="4afa2-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="4afa2-145">string</span><span class="sxs-lookup"><span data-stu-id="4afa2-145">string</span></span> | <span data-ttu-id="4afa2-146">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="4afa2-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="4afa2-147">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4afa2-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="4afa2-148">Optional.</span><span class="sxs-lookup"><span data-stu-id="4afa2-148">Optional.</span></span> |
| <span data-ttu-id="4afa2-149">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="4afa2-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="4afa2-150">string</span><span class="sxs-lookup"><span data-stu-id="4afa2-150">string</span></span> | <span data-ttu-id="4afa2-151">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="4afa2-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="4afa2-152">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="4afa2-152">Values can be "text" or "html".</span></span> <span data-ttu-id="4afa2-153">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="4afa2-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="4afa2-154">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4afa2-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="4afa2-155">Optional.</span><span class="sxs-lookup"><span data-stu-id="4afa2-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4afa2-156">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4afa2-156">Request body</span></span>
<span data-ttu-id="4afa2-157">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4afa2-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4afa2-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="4afa2-158">Response</span></span>

<span data-ttu-id="4afa2-159">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4afa2-159">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4afa2-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4afa2-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4afa2-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4afa2-161">Request</span></span>
<span data-ttu-id="4afa2-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4afa2-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="4afa2-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="4afa2-163">Response</span></span>
<span data-ttu-id="4afa2-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4afa2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": ""
}-->

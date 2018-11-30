---
title: Ereignisse auflisten
description: Dient zum Abrufen einer Liste von Ereignissen in einem Kalender.  Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.
ms.openlocfilehash: 826f3247c9fbd1a30492368b736805075560a159
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020122"
---
# <a name="list-events"></a><span data-ttu-id="1bcb0-104">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="1bcb0-104">List events</span></span>

<span data-ttu-id="1bcb0-p102">Dient zum Abrufen einer Liste von Ereignissen in einem Kalender.  Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="1bcb0-107">Wenn Sie erweiterte Ereignisinstanzen abrufen möchten, können Sie [die Kalenderansicht abrufen](calendar-list-calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="1bcb0-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bcb0-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1bcb0-108">Permissions</span></span>
<span data-ttu-id="1bcb0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bcb0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bcb0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1bcb0-111">Permission type</span></span>      | <span data-ttu-id="1bcb0-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1bcb0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bcb0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1bcb0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1bcb0-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1bcb0-114">Calendars.Read</span></span>    |
|<span data-ttu-id="1bcb0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1bcb0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bcb0-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1bcb0-116">Calendars.Read</span></span>    |
|<span data-ttu-id="1bcb0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1bcb0-117">Application</span></span> | <span data-ttu-id="1bcb0-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1bcb0-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bcb0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bcb0-119">HTTP request</span></span>
<span data-ttu-id="1bcb0-120"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="1bcb0-120"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="1bcb0-121">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="1bcb0-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="1bcb0-122">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="1bcb0-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1bcb0-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1bcb0-123">Optional query parameters</span></span>
<span data-ttu-id="1bcb0-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1bcb0-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1bcb0-125">Request headers</span></span>
| <span data-ttu-id="1bcb0-126">Name</span><span class="sxs-lookup"><span data-stu-id="1bcb0-126">Name</span></span>       | <span data-ttu-id="1bcb0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1bcb0-127">Type</span></span> | <span data-ttu-id="1bcb0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1bcb0-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="1bcb0-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bcb0-129">Authorization</span></span>  | <span data-ttu-id="1bcb0-130">string</span><span class="sxs-lookup"><span data-stu-id="1bcb0-130">string</span></span> | <span data-ttu-id="1bcb0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1bcb0-133">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1bcb0-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="1bcb0-134">string</span><span class="sxs-lookup"><span data-stu-id="1bcb0-134">string</span></span> | <span data-ttu-id="1bcb0-135">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="1bcb0-136">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="1bcb0-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bcb0-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1bcb0-138">Request body</span></span>
<span data-ttu-id="1bcb0-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bcb0-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bcb0-140">Response</span></span>

<span data-ttu-id="1bcb0-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bcb0-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1bcb0-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bcb0-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bcb0-143">Request</span></span>
<span data-ttu-id="1bcb0-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="1bcb0-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bcb0-145">Response</span></span>
<span data-ttu-id="1bcb0-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bcb0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: Instanzen auflisten
description: Rufen Sie die Instanzen (vorkommen) eines Ereignisses für einen angegebenen Zeitraum. Wenn das Ereignis gehört zu einer `SeriesMaster` eingeben, gibt die
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7a40e6f468c8541748adbc7d8dd588541318c30c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980930"
---
# <a name="list-instances"></a><span data-ttu-id="0f734-104">Listeninstanzen</span><span class="sxs-lookup"><span data-stu-id="0f734-104">List instances</span></span>

> <span data-ttu-id="0f734-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f734-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f734-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f734-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f734-p103">Dient zum Abrufen der Instanzen (Vorkommen) eines Ereignisses für einen angegebenen Zeitraum. Wenn das Ereignis vom Typ `SeriesMaster` ist, werden hierdurch die Vorkommen und Ausnahmen des Ereignisses im des angegebenen Zeitraum zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f734-p103">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f734-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f734-109">Permissions</span></span>
<span data-ttu-id="0f734-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f734-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f734-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f734-112">Permission type</span></span>      | <span data-ttu-id="0f734-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f734-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f734-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f734-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0f734-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0f734-115">Calendars.Read</span></span>    |
|<span data-ttu-id="0f734-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f734-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f734-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0f734-117">Calendars.Read</span></span>    |
|<span data-ttu-id="0f734-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f734-118">Application</span></span> | <span data-ttu-id="0f734-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0f734-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f734-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f734-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="0f734-121">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0f734-121">Query parameters</span></span>

<span data-ttu-id="0f734-122">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="0f734-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="0f734-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="0f734-123">Parameter</span></span>    | <span data-ttu-id="0f734-124">Typ</span><span class="sxs-lookup"><span data-stu-id="0f734-124">Type</span></span>   |<span data-ttu-id="0f734-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f734-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f734-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0f734-126">startDateTime</span></span>|<span data-ttu-id="0f734-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f734-127">String</span></span>|<span data-ttu-id="0f734-p105">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="0f734-p105">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="0f734-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0f734-130">endDateTime</span></span>|<span data-ttu-id="0f734-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f734-131">String</span></span>|<span data-ttu-id="0f734-p106">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="0f734-p106">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="0f734-134">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f734-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0f734-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f734-135">Request headers</span></span>
| <span data-ttu-id="0f734-136">Name</span><span class="sxs-lookup"><span data-stu-id="0f734-136">Name</span></span>       | <span data-ttu-id="0f734-137">Typ</span><span class="sxs-lookup"><span data-stu-id="0f734-137">Type</span></span> | <span data-ttu-id="0f734-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f734-138">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="0f734-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f734-139">Authorization</span></span>  | <span data-ttu-id="0f734-140">string</span><span class="sxs-lookup"><span data-stu-id="0f734-140">string</span></span> | <span data-ttu-id="0f734-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f734-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f734-143">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0f734-143">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="0f734-144">string</span><span class="sxs-lookup"><span data-stu-id="0f734-144">string</span></span> | <span data-ttu-id="0f734-145">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="0f734-145">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="0f734-146">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f734-146">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="0f734-147">Optional.</span><span class="sxs-lookup"><span data-stu-id="0f734-147">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f734-148">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f734-148">Request body</span></span>
<span data-ttu-id="0f734-149">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0f734-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f734-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f734-150">Response</span></span>

<span data-ttu-id="0f734-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f734-151">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f734-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f734-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f734-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f734-153">Request</span></span>
<span data-ttu-id="0f734-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f734-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="0f734-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f734-155">Response</span></span>
<span data-ttu-id="0f734-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f734-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

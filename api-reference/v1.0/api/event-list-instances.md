---
title: Instanzen auflisten
description: 'Rufen Sie die Instanzen (vorkommen) eines Ereignisses für einen angegebenen Zeitraum. Wenn das Ereignis gehört zu einer `SeriesMaster` eingeben, gibt die '
ms.openlocfilehash: 6a423efb2ff969e66ba54807c506a3b431b7ee32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016201"
---
# <a name="list-instances"></a><span data-ttu-id="d1b7d-104">Instanzen auflisten</span><span class="sxs-lookup"><span data-stu-id="d1b7d-104">List instances</span></span>

<span data-ttu-id="d1b7d-p102">Dient zum Abrufen der Instanzen (Vorkommen) eines Ereignisses für einen angegebenen Zeitraum. Wenn das Ereignis vom Typ `SeriesMaster` ist, werden hierdurch die Vorkommen und Ausnahmen des Ereignisses im des angegebenen Zeitraum zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1b7d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d1b7d-107">Permissions</span></span>
<span data-ttu-id="d1b7d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1b7d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1b7d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d1b7d-110">Permission type</span></span>      | <span data-ttu-id="d1b7d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d1b7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1b7d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d1b7d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d1b7d-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d1b7d-113">Calendars.Read</span></span>    |
|<span data-ttu-id="d1b7d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d1b7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1b7d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d1b7d-115">Calendars.Read</span></span>    |
|<span data-ttu-id="d1b7d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d1b7d-116">Application</span></span> | <span data-ttu-id="d1b7d-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d1b7d-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1b7d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1b7d-118">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="d1b7d-119">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d1b7d-119">Query parameters</span></span>

<span data-ttu-id="d1b7d-120">Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="d1b7d-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="d1b7d-121">Parameter</span></span>    | <span data-ttu-id="d1b7d-122">Typ</span><span class="sxs-lookup"><span data-stu-id="d1b7d-122">Type</span></span>   |<span data-ttu-id="d1b7d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1b7d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1b7d-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d1b7d-124">startDateTime</span></span>|<span data-ttu-id="d1b7d-125">String</span><span class="sxs-lookup"><span data-stu-id="d1b7d-125">String</span></span>|<span data-ttu-id="d1b7d-p104">Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d1b7d-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d1b7d-128">endDateTime</span></span>|<span data-ttu-id="d1b7d-129">String</span><span class="sxs-lookup"><span data-stu-id="d1b7d-129">String</span></span>|<span data-ttu-id="d1b7d-p105">Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="d1b7d-132">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d1b7d-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d1b7d-133">Request headers</span></span>
| <span data-ttu-id="d1b7d-134">Name</span><span class="sxs-lookup"><span data-stu-id="d1b7d-134">Name</span></span>       | <span data-ttu-id="d1b7d-135">Typ</span><span class="sxs-lookup"><span data-stu-id="d1b7d-135">Type</span></span> | <span data-ttu-id="d1b7d-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1b7d-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d1b7d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1b7d-137">Authorization</span></span>  | <span data-ttu-id="d1b7d-138">string</span><span class="sxs-lookup"><span data-stu-id="d1b7d-138">string</span></span> | <span data-ttu-id="d1b7d-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d1b7d-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d1b7d-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d1b7d-142">string</span><span class="sxs-lookup"><span data-stu-id="d1b7d-142">string</span></span> | <span data-ttu-id="d1b7d-143">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d1b7d-144">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d1b7d-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1b7d-146">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d1b7d-146">Request body</span></span>
<span data-ttu-id="d1b7d-147">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1b7d-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1b7d-148">Response</span></span>

<span data-ttu-id="d1b7d-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-149">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1b7d-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d1b7d-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1b7d-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1b7d-151">Request</span></span>
<span data-ttu-id="d1b7d-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="d1b7d-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1b7d-153">Response</span></span>
<span data-ttu-id="d1b7d-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1b7d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'event: snoozeReminder'
description: Verschieben Sie eine Erinnerung für ein Ereignis in einem Benutzerkalender bis zu einer neuen Uhrzeit.
ms.openlocfilehash: 8b7cb8f2ada513aac0fd048bb49a69198bc630d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063656"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="15119-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="15119-103">event: snoozeReminder</span></span>

> <span data-ttu-id="15119-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15119-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15119-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15119-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15119-106">Verschieben Sie eine Erinnerung für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) des Benutzers bis zu einem neuen Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="15119-106">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="15119-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15119-107">Permissions</span></span>
<span data-ttu-id="15119-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15119-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15119-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15119-110">Permission type</span></span>      | <span data-ttu-id="15119-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15119-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15119-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15119-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15119-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15119-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="15119-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15119-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15119-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15119-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="15119-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15119-116">Application</span></span> | <span data-ttu-id="15119-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15119-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="15119-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15119-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="15119-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15119-119">Request headers</span></span>
| <span data-ttu-id="15119-120">Name</span><span class="sxs-lookup"><span data-stu-id="15119-120">Name</span></span>       | <span data-ttu-id="15119-121">Typ</span><span class="sxs-lookup"><span data-stu-id="15119-121">Type</span></span> | <span data-ttu-id="15119-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15119-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15119-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15119-123">Authorization</span></span>  | <span data-ttu-id="15119-124">string</span><span class="sxs-lookup"><span data-stu-id="15119-124">string</span></span>  | <span data-ttu-id="15119-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15119-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15119-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15119-127">Content-Type</span></span> | <span data-ttu-id="15119-128">string</span><span class="sxs-lookup"><span data-stu-id="15119-128">string</span></span>  | <span data-ttu-id="15119-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15119-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15119-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15119-131">Request body</span></span>
<span data-ttu-id="15119-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="15119-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="15119-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="15119-133">Parameter</span></span>    | <span data-ttu-id="15119-134">Typ</span><span class="sxs-lookup"><span data-stu-id="15119-134">Type</span></span>   |<span data-ttu-id="15119-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15119-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15119-136">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="15119-136">newReminderTime</span></span>|<span data-ttu-id="15119-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="15119-137">DateTimeTimeZone</span></span>|<span data-ttu-id="15119-138">Das neue Datum und die neue Uhrzeit für die Auslösung der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="15119-138">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="15119-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="15119-139">Response</span></span>

<span data-ttu-id="15119-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15119-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15119-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15119-142">Example</span></span>
<span data-ttu-id="15119-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="15119-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="15119-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15119-144">Request</span></span>
<span data-ttu-id="15119-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15119-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "2016-10-19T10:37:00Z",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="15119-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="15119-146">Response</span></span>
<span data-ttu-id="15119-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="15119-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

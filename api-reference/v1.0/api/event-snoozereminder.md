---
title: 'event: snoozeReminder'
description: Verschieben Sie eine Erinnerung für ein Ereignis in einem Benutzerkalender bis zu einer neuen Uhrzeit.
ms.openlocfilehash: 9e47a128afd8caa9c771011c98e3c6c98c4ee612
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016275"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="b60dc-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="b60dc-103">event: snoozeReminder</span></span>

<span data-ttu-id="b60dc-104">Verschieben Sie eine Erinnerung für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) des Benutzers bis zu einem neuen Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="b60dc-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="b60dc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b60dc-105">Permissions</span></span>
<span data-ttu-id="b60dc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b60dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b60dc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b60dc-108">Permission type</span></span>      | <span data-ttu-id="b60dc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b60dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b60dc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b60dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b60dc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b60dc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b60dc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b60dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b60dc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b60dc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b60dc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b60dc-114">Application</span></span> | <span data-ttu-id="b60dc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b60dc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b60dc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b60dc-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="b60dc-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b60dc-117">Request headers</span></span>
| <span data-ttu-id="b60dc-118">Name</span><span class="sxs-lookup"><span data-stu-id="b60dc-118">Name</span></span>       | <span data-ttu-id="b60dc-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b60dc-119">Type</span></span> | <span data-ttu-id="b60dc-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b60dc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b60dc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b60dc-121">Authorization</span></span>  | <span data-ttu-id="b60dc-122">string</span><span class="sxs-lookup"><span data-stu-id="b60dc-122">string</span></span>  | <span data-ttu-id="b60dc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b60dc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b60dc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b60dc-125">Content-Type</span></span> | <span data-ttu-id="b60dc-126">string</span><span class="sxs-lookup"><span data-stu-id="b60dc-126">string</span></span>  | <span data-ttu-id="b60dc-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b60dc-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b60dc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b60dc-129">Request body</span></span>
<span data-ttu-id="b60dc-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b60dc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b60dc-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="b60dc-131">Parameter</span></span>    | <span data-ttu-id="b60dc-132">Typ</span><span class="sxs-lookup"><span data-stu-id="b60dc-132">Type</span></span>   |<span data-ttu-id="b60dc-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b60dc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b60dc-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="b60dc-134">newReminderTime</span></span>|<span data-ttu-id="b60dc-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b60dc-135">DateTimeTimeZone</span></span>|<span data-ttu-id="b60dc-136">Das neue Datum und die neue Uhrzeit für die Auslösung der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="b60dc-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="b60dc-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b60dc-137">Response</span></span>

<span data-ttu-id="b60dc-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b60dc-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b60dc-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b60dc-140">Example</span></span>
<span data-ttu-id="b60dc-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b60dc-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b60dc-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b60dc-142">Request</span></span>
<span data-ttu-id="b60dc-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b60dc-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="b60dc-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b60dc-144">Response</span></span>
<span data-ttu-id="b60dc-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b60dc-145">Here is an example of the response.</span></span>
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

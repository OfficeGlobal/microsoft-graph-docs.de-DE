---
title: 'event: snoozeReminder'
description: Verschieben Sie eine Erinnerung für ein Ereignis in einem Benutzerkalender bis zu einer neuen Uhrzeit.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d3f8ffab576182f5e67dad49e34c67d886fe0bde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932413"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="66685-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="66685-103">event: snoozeReminder</span></span>

<span data-ttu-id="66685-104">Verschieben Sie eine Erinnerung für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) des Benutzers bis zu einem neuen Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="66685-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="66685-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="66685-105">Permissions</span></span>
<span data-ttu-id="66685-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66685-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66685-108">Permission type</span></span>      | <span data-ttu-id="66685-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66685-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66685-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66685-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66685-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66685-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="66685-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66685-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66685-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66685-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="66685-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66685-114">Application</span></span> | <span data-ttu-id="66685-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66685-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="66685-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66685-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="66685-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66685-117">Request headers</span></span>
| <span data-ttu-id="66685-118">Name</span><span class="sxs-lookup"><span data-stu-id="66685-118">Name</span></span>       | <span data-ttu-id="66685-119">Typ</span><span class="sxs-lookup"><span data-stu-id="66685-119">Type</span></span> | <span data-ttu-id="66685-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66685-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66685-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66685-121">Authorization</span></span>  | <span data-ttu-id="66685-122">string</span><span class="sxs-lookup"><span data-stu-id="66685-122">string</span></span>  | <span data-ttu-id="66685-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="66685-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66685-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66685-125">Content-Type</span></span> | <span data-ttu-id="66685-126">string</span><span class="sxs-lookup"><span data-stu-id="66685-126">string</span></span>  | <span data-ttu-id="66685-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="66685-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66685-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66685-129">Request body</span></span>
<span data-ttu-id="66685-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="66685-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66685-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="66685-131">Parameter</span></span>    | <span data-ttu-id="66685-132">Typ</span><span class="sxs-lookup"><span data-stu-id="66685-132">Type</span></span>   |<span data-ttu-id="66685-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66685-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66685-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="66685-134">newReminderTime</span></span>|<span data-ttu-id="66685-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="66685-135">DateTimeTimeZone</span></span>|<span data-ttu-id="66685-136">Das neue Datum und die neue Uhrzeit für die Auslösung der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="66685-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="66685-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="66685-137">Response</span></span>

<span data-ttu-id="66685-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66685-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66685-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66685-140">Example</span></span>
<span data-ttu-id="66685-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="66685-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="66685-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66685-142">Request</span></span>
<span data-ttu-id="66685-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66685-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="66685-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="66685-144">Response</span></span>
<span data-ttu-id="66685-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="66685-145">Here is an example of the response.</span></span>
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

---
title: 'event: dismissReminder'
description: Schließen Sie eine Erinnerung, die in einem Benutzerkalender für ein Ereignis ausgelöst wurde.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 570a9b34031afe6d53b6e577127180ebdbe7a163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864939"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="dcdd5-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="dcdd5-103">event: dismissReminder</span></span>

> <span data-ttu-id="dcdd5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dcdd5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcdd5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dcdd5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dcdd5-106">Schließen Sie eine Erinnerung, die für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md)des Benutzers ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="dcdd5-106">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcdd5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dcdd5-107">Permissions</span></span>
<span data-ttu-id="dcdd5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcdd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcdd5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dcdd5-110">Permission type</span></span>      | <span data-ttu-id="dcdd5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dcdd5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcdd5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dcdd5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dcdd5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcdd5-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dcdd5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dcdd5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcdd5-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcdd5-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dcdd5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dcdd5-116">Application</span></span> | <span data-ttu-id="dcdd5-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcdd5-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcdd5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcdd5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

## <a name="request-headers"></a><span data-ttu-id="dcdd5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dcdd5-119">Request headers</span></span>

| <span data-ttu-id="dcdd5-120">Name</span><span class="sxs-lookup"><span data-stu-id="dcdd5-120">Name</span></span>       | <span data-ttu-id="dcdd5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="dcdd5-121">Type</span></span> | <span data-ttu-id="dcdd5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dcdd5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dcdd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcdd5-123">Authorization</span></span>  | <span data-ttu-id="dcdd5-124">string</span><span class="sxs-lookup"><span data-stu-id="dcdd5-124">string</span></span>  | <span data-ttu-id="dcdd5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcdd5-p103">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="dcdd5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcdd5-127">Response</span></span>

<span data-ttu-id="dcdd5-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dcdd5-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcdd5-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dcdd5-130">Example</span></span>

<span data-ttu-id="dcdd5-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="dcdd5-131">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dcdd5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcdd5-132">Request</span></span>
<span data-ttu-id="dcdd5-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dcdd5-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="dcdd5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcdd5-134">Response</span></span>
<span data-ttu-id="dcdd5-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dcdd5-135">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

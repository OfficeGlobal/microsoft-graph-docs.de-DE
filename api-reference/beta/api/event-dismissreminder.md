---
title: 'event: dismissReminder'
description: Schließen Sie eine Erinnerung, die in einem Benutzerkalender für ein Ereignis ausgelöst wurde.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 43ba18ae5a2e0859ed033ca89615c4116f0908b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916439"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="a0ee9-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="a0ee9-103">event: dismissReminder</span></span>

> <span data-ttu-id="a0ee9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a0ee9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0ee9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a0ee9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0ee9-106">Schließen Sie eine Erinnerung, die für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md)des Benutzers ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="a0ee9-106">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0ee9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a0ee9-107">Permissions</span></span>
<span data-ttu-id="a0ee9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0ee9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0ee9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0ee9-110">Permission type</span></span>      | <span data-ttu-id="a0ee9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0ee9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0ee9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0ee9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0ee9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0ee9-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a0ee9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0ee9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0ee9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0ee9-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a0ee9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0ee9-116">Application</span></span> | <span data-ttu-id="a0ee9-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0ee9-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0ee9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0ee9-118">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a0ee9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0ee9-119">Request headers</span></span>

| <span data-ttu-id="a0ee9-120">Name</span><span class="sxs-lookup"><span data-stu-id="a0ee9-120">Name</span></span>       | <span data-ttu-id="a0ee9-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a0ee9-121">Type</span></span> | <span data-ttu-id="a0ee9-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0ee9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0ee9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0ee9-123">Authorization</span></span>  | <span data-ttu-id="a0ee9-124">string</span><span class="sxs-lookup"><span data-stu-id="a0ee9-124">string</span></span>  | <span data-ttu-id="a0ee9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a0ee9-p103">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="a0ee9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0ee9-127">Response</span></span>

<span data-ttu-id="a0ee9-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0ee9-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0ee9-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0ee9-130">Example</span></span>

<span data-ttu-id="a0ee9-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a0ee9-131">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a0ee9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0ee9-132">Request</span></span>
<span data-ttu-id="a0ee9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a0ee9-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="a0ee9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0ee9-134">Response</span></span>
<span data-ttu-id="a0ee9-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0ee9-135">Here is an example of the response.</span></span>

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

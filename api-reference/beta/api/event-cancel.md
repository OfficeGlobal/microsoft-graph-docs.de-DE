---
title: 'Ereignis: Abbrechen'
description: 'Dieser Aktion kann den Organisator einer Besprechung senden eine Absage und das Ereignis abzubrechen. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7fe7841ae1f0a7a4d3128177203becbb363073f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951196"
---
# <a name="event-cancel"></a><span data-ttu-id="aadc6-103">Ereignis: Abbrechen</span><span class="sxs-lookup"><span data-stu-id="aadc6-103">event: cancel</span></span>

> <span data-ttu-id="aadc6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aadc6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aadc6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aadc6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aadc6-106">Dieser Aktion kann den Organisator einer Besprechung senden eine Absage und das Ereignis abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="aadc6-106">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="aadc6-107">Die Aktion wird das Ereignis in den Ordner Gelöschte Objekte verschoben.</span><span class="sxs-lookup"><span data-stu-id="aadc6-107">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="aadc6-108">Der Organisator kann auch ein Vorkommen einer Besprechungsserie abzubrechen, durch die Bereitstellung der Vorkommen-Ereignis-ID</span><span class="sxs-lookup"><span data-stu-id="aadc6-108">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="aadc6-109">Diese Aktion aufrufen Teilnehmerin Ruft einen Fehler (HTTP 400 Ungültige Anforderung), wobei die folgende Fehlermeldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="aadc6-109">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="aadc6-110">"Die Anforderung konnte nicht abgeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="aadc6-110">"Your request can't be completed.</span></span> <span data-ttu-id="aadc6-111">Sie müssen ein Organisator eine Besprechung abgebrochen werden."</span><span class="sxs-lookup"><span data-stu-id="aadc6-111">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="aadc6-112">Diese Aktion unterscheidet sich von [Löschen](event-delete.md) , **Abbrechen** nur den Organisator steht und den Organisator eine benutzerdefinierte Meldung an die Teilnehmer über den Abbruch senden können.</span><span class="sxs-lookup"><span data-stu-id="aadc6-112">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="aadc6-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aadc6-113">Permissions</span></span>
<span data-ttu-id="aadc6-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aadc6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aadc6-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aadc6-116">Permission type</span></span>      | <span data-ttu-id="aadc6-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aadc6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aadc6-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aadc6-118">Delegated (work or school account)</span></span> | <span data-ttu-id="aadc6-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aadc6-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="aadc6-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aadc6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aadc6-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aadc6-121">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="aadc6-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aadc6-122">Application</span></span> | <span data-ttu-id="aadc6-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aadc6-123">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aadc6-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aadc6-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/cancel
POST /users/{id | userPrincipalName}/events/{id}/cancel
POST /groups/{id}/events/{id}/cancel

POST /me/calendar/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendar/events/{id}/cancel
POST /groups/{id}/calendar/events/{id}/cancel

POST /me/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/cancel

POST /me/calendargroup/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/cancel

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="aadc6-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aadc6-125">Request headers</span></span>
| <span data-ttu-id="aadc6-126">Name</span><span class="sxs-lookup"><span data-stu-id="aadc6-126">Name</span></span>       | <span data-ttu-id="aadc6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="aadc6-127">Type</span></span> | <span data-ttu-id="aadc6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aadc6-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aadc6-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="aadc6-129">Authorization</span></span>  | <span data-ttu-id="aadc6-130">string</span><span class="sxs-lookup"><span data-stu-id="aadc6-130">string</span></span>  | <span data-ttu-id="aadc6-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aadc6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aadc6-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aadc6-133">Content-Type</span></span> | <span data-ttu-id="aadc6-134">string</span><span class="sxs-lookup"><span data-stu-id="aadc6-134">string</span></span>  | <span data-ttu-id="aadc6-p106">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aadc6-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aadc6-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aadc6-137">Request body</span></span>
<span data-ttu-id="aadc6-138">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="aadc6-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aadc6-139">Parameter</span><span class="sxs-lookup"><span data-stu-id="aadc6-139">Parameter</span></span>    | <span data-ttu-id="aadc6-140">Typ</span><span class="sxs-lookup"><span data-stu-id="aadc6-140">Type</span></span>   |<span data-ttu-id="aadc6-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aadc6-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aadc6-142">comment</span><span class="sxs-lookup"><span data-stu-id="aadc6-142">comment</span></span>|<span data-ttu-id="aadc6-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aadc6-143">String</span></span>|<span data-ttu-id="aadc6-144">Einen Kommentar zu den Abbruch an alle Teilnehmer gesendet.</span><span class="sxs-lookup"><span data-stu-id="aadc6-144">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="aadc6-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="aadc6-145">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="aadc6-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="aadc6-146">Response</span></span>

<span data-ttu-id="aadc6-p108">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aadc6-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aadc6-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aadc6-149">Example</span></span>
<span data-ttu-id="aadc6-150">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="aadc6-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aadc6-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aadc6-151">Request</span></span>
<span data-ttu-id="aadc6-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aadc6-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```

##### <a name="response"></a><span data-ttu-id="aadc6-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="aadc6-153">Response</span></span>
<span data-ttu-id="aadc6-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aadc6-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

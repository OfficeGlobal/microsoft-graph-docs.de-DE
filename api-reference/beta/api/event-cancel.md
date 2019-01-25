---
title: 'Ereignis: Abbrechen'
description: 'Dieser Aktion kann den Organisator einer Besprechung senden eine Absage und das Ereignis abzubrechen. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e39066c3360113965b0009473e520557853ba284
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530153"
---
# <a name="event-cancel"></a><span data-ttu-id="a50b6-103">Ereignis: Abbrechen</span><span class="sxs-lookup"><span data-stu-id="a50b6-103">event: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a50b6-104">Dieser Aktion kann den Organisator einer Besprechung senden eine Absage und das Ereignis abzubrechen.</span><span class="sxs-lookup"><span data-stu-id="a50b6-104">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="a50b6-105">Die Aktion wird das Ereignis in den Ordner Gelöschte Objekte verschoben.</span><span class="sxs-lookup"><span data-stu-id="a50b6-105">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="a50b6-106">Der Organisator kann auch ein Vorkommen einer Besprechungsserie abzubrechen, durch die Bereitstellung der Vorkommen-Ereignis-ID</span><span class="sxs-lookup"><span data-stu-id="a50b6-106">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="a50b6-107">Diese Aktion aufrufen Teilnehmerin Ruft einen Fehler (HTTP 400 Ungültige Anforderung), wobei die folgende Fehlermeldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="a50b6-107">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="a50b6-108">"Die Anforderung konnte nicht abgeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="a50b6-108">"Your request can't be completed.</span></span> <span data-ttu-id="a50b6-109">Sie müssen ein Organisator eine Besprechung abgebrochen werden."</span><span class="sxs-lookup"><span data-stu-id="a50b6-109">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="a50b6-110">Diese Aktion unterscheidet sich von [Löschen](event-delete.md) , **Abbrechen** nur den Organisator steht und den Organisator eine benutzerdefinierte Meldung an die Teilnehmer über den Abbruch senden können.</span><span class="sxs-lookup"><span data-stu-id="a50b6-110">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="a50b6-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a50b6-111">Permissions</span></span>
<span data-ttu-id="a50b6-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a50b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a50b6-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a50b6-114">Permission type</span></span>      | <span data-ttu-id="a50b6-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a50b6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a50b6-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a50b6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a50b6-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a50b6-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a50b6-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a50b6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a50b6-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a50b6-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a50b6-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a50b6-120">Application</span></span> | <span data-ttu-id="a50b6-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a50b6-121">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a50b6-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a50b6-122">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="a50b6-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a50b6-123">Request headers</span></span>
| <span data-ttu-id="a50b6-124">Name</span><span class="sxs-lookup"><span data-stu-id="a50b6-124">Name</span></span>       | <span data-ttu-id="a50b6-125">Typ</span><span class="sxs-lookup"><span data-stu-id="a50b6-125">Type</span></span> | <span data-ttu-id="a50b6-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a50b6-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a50b6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a50b6-127">Authorization</span></span>  | <span data-ttu-id="a50b6-128">string</span><span class="sxs-lookup"><span data-stu-id="a50b6-128">string</span></span>  | <span data-ttu-id="a50b6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a50b6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a50b6-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a50b6-131">Content-Type</span></span> | <span data-ttu-id="a50b6-132">string</span><span class="sxs-lookup"><span data-stu-id="a50b6-132">string</span></span>  | <span data-ttu-id="a50b6-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a50b6-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a50b6-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a50b6-135">Request body</span></span>
<span data-ttu-id="a50b6-136">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a50b6-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a50b6-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="a50b6-137">Parameter</span></span>    | <span data-ttu-id="a50b6-138">Typ</span><span class="sxs-lookup"><span data-stu-id="a50b6-138">Type</span></span>   |<span data-ttu-id="a50b6-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a50b6-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a50b6-140">comment</span><span class="sxs-lookup"><span data-stu-id="a50b6-140">comment</span></span>|<span data-ttu-id="a50b6-141">String</span><span class="sxs-lookup"><span data-stu-id="a50b6-141">String</span></span>|<span data-ttu-id="a50b6-142">Einen Kommentar zu den Abbruch an alle Teilnehmer gesendet.</span><span class="sxs-lookup"><span data-stu-id="a50b6-142">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="a50b6-143">Optional.</span><span class="sxs-lookup"><span data-stu-id="a50b6-143">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="a50b6-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="a50b6-144">Response</span></span>

<span data-ttu-id="a50b6-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a50b6-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a50b6-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a50b6-147">Example</span></span>
<span data-ttu-id="a50b6-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a50b6-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a50b6-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a50b6-149">Request</span></span>
<span data-ttu-id="a50b6-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a50b6-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a50b6-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="a50b6-151">Response</span></span>
<span data-ttu-id="a50b6-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a50b6-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

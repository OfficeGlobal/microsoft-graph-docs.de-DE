---
title: 'Ereignis: weiterleiten'
description: 'Mit dieser Aktion kann der Organisator oder Teilnehmer einer Besprechung-Ereignisses zum Weiterleiten der '
ms.openlocfilehash: 09a98f82e72eef7b223dfccb1f4433c3206f0f7f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058019"
---
# <a name="event-forward"></a><span data-ttu-id="9f6d7-103">Ereignis: weiterleiten</span><span class="sxs-lookup"><span data-stu-id="9f6d7-103">event: forward</span></span>

> <span data-ttu-id="9f6d7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f6d7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f6d7-106">Diese Aktion ermöglicht dem Organisator oder Teilnehmer einer Besprechung- [Ereignis](../resources/event.md) auf die Besprechungsanfrage an einen neuen Empfänger weiterleitet.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-106">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="9f6d7-107">Wenn das Ereignis Besprechung aus einem Teilnehmer Office 365-Postfach an einen anderen Empfänger weitergeleitet wird, diese Aktion sendet eine Nachricht zur Benachrichtigung des Organisators die Weiterleitung auch der Organisator Kopie des Ereignisses Besprechung den Empfänger hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-107">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="9f6d7-108">Diese Bequemlichkeit ist nicht verfügbar, von einem Outlook.com Konto weiterleiten zu können.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-108">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="9f6d7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f6d7-109">Permissions</span></span>
<span data-ttu-id="9f6d7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f6d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f6d7-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f6d7-112">Permission type</span></span>      | <span data-ttu-id="9f6d7-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f6d7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f6d7-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f6d7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9f6d7-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9f6d7-115">Calendars.Read</span></span>    |
|<span data-ttu-id="9f6d7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f6d7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f6d7-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9f6d7-117">Calendars.Read</span></span>    |
|<span data-ttu-id="9f6d7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f6d7-118">Application</span></span> | <span data-ttu-id="9f6d7-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9f6d7-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f6d7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f6d7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/forward
POST /users/{id | userPrincipalName}/events/{id}/forward
POST /groups/{id}/events/{id}/forward

POST /me/calendar/events/{id}/forward
POST /users/{id | userPrincipalName}/calendar/events/{id}/forward
POST /groups/{id}/calendar/events/{id}/forward

POST /me/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/forward

POST /me/calendargroup/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/forward

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="9f6d7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f6d7-121">Request headers</span></span>
| <span data-ttu-id="9f6d7-122">Name</span><span class="sxs-lookup"><span data-stu-id="9f6d7-122">Name</span></span>       | <span data-ttu-id="9f6d7-123">Typ</span><span class="sxs-lookup"><span data-stu-id="9f6d7-123">Type</span></span> | <span data-ttu-id="9f6d7-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f6d7-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f6d7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f6d7-125">Authorization</span></span>  | <span data-ttu-id="9f6d7-126">string</span><span class="sxs-lookup"><span data-stu-id="9f6d7-126">string</span></span>  | <span data-ttu-id="9f6d7-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f6d7-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f6d7-129">Content-Type</span></span> | <span data-ttu-id="9f6d7-130">string</span><span class="sxs-lookup"><span data-stu-id="9f6d7-130">string</span></span>  | <span data-ttu-id="9f6d7-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f6d7-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f6d7-133">Request body</span></span>
<span data-ttu-id="9f6d7-134">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9f6d7-135">Parameter</span><span class="sxs-lookup"><span data-stu-id="9f6d7-135">Parameter</span></span>    | <span data-ttu-id="9f6d7-136">Typ</span><span class="sxs-lookup"><span data-stu-id="9f6d7-136">Type</span></span>   |<span data-ttu-id="9f6d7-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f6d7-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f6d7-138">Kommentar</span><span class="sxs-lookup"><span data-stu-id="9f6d7-138">Comment</span></span>|<span data-ttu-id="9f6d7-139">String</span><span class="sxs-lookup"><span data-stu-id="9f6d7-139">String</span></span>|<span data-ttu-id="9f6d7-p106">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="9f6d7-142">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="9f6d7-142">ToRecipients</span></span>|<span data-ttu-id="9f6d7-143">[recipient](../resources/recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9f6d7-143">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="9f6d7-144">Die Liste der Empfänger des Ereignisses zum Weiterleiten.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-144">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="9f6d7-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f6d7-145">Response</span></span>

<span data-ttu-id="9f6d7-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f6d7-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f6d7-148">Example</span></span>
<span data-ttu-id="9f6d7-149">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9f6d7-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f6d7-150">Request</span></span>
<span data-ttu-id="9f6d7-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/forward
Content-type: application/json
Content-length: 56

{
  "ToRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ],
  "Comment": "Dana, hope you can make this meeting." 
}

```

##### <a name="response"></a><span data-ttu-id="9f6d7-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f6d7-152">Response</span></span>
<span data-ttu-id="9f6d7-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9f6d7-153">Here is an example of the response.</span></span>
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
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

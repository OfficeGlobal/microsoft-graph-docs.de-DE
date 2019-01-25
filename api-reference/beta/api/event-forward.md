---
title: 'Ereignis: weiterleiten'
description: 'Mit dieser Aktion kann der Organisator oder Teilnehmer einer Besprechung-Ereignisses zum Weiterleiten der '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6f1b3e1f089d927aeb21ca80ff77edda63121c60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510386"
---
# <a name="event-forward"></a><span data-ttu-id="18530-103">Ereignis: weiterleiten</span><span class="sxs-lookup"><span data-stu-id="18530-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18530-104">Diese Aktion ermöglicht dem Organisator oder Teilnehmer einer Besprechung- [Ereignis](../resources/event.md) auf die Besprechungsanfrage an einen neuen Empfänger weiterleitet.</span><span class="sxs-lookup"><span data-stu-id="18530-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="18530-105">Wenn das Ereignis Besprechung aus einem Teilnehmer Office 365-Postfach an einen anderen Empfänger weitergeleitet wird, diese Aktion sendet eine Nachricht zur Benachrichtigung des Organisators die Weiterleitung auch der Organisator Kopie des Ereignisses Besprechung den Empfänger hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="18530-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="18530-106">Diese Bequemlichkeit ist nicht verfügbar, von einem Outlook.com Konto weiterleiten zu können.</span><span class="sxs-lookup"><span data-stu-id="18530-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="18530-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18530-107">Permissions</span></span>
<span data-ttu-id="18530-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18530-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18530-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18530-110">Permission type</span></span>      | <span data-ttu-id="18530-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18530-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18530-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18530-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18530-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="18530-113">Calendars.Read</span></span>    |
|<span data-ttu-id="18530-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18530-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18530-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="18530-115">Calendars.Read</span></span>    |
|<span data-ttu-id="18530-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18530-116">Application</span></span> | <span data-ttu-id="18530-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="18530-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="18530-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18530-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="18530-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18530-119">Request headers</span></span>
| <span data-ttu-id="18530-120">Name</span><span class="sxs-lookup"><span data-stu-id="18530-120">Name</span></span>       | <span data-ttu-id="18530-121">Typ</span><span class="sxs-lookup"><span data-stu-id="18530-121">Type</span></span> | <span data-ttu-id="18530-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18530-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18530-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18530-123">Authorization</span></span>  | <span data-ttu-id="18530-124">string</span><span class="sxs-lookup"><span data-stu-id="18530-124">string</span></span>  | <span data-ttu-id="18530-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18530-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18530-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18530-127">Content-Type</span></span> | <span data-ttu-id="18530-128">string</span><span class="sxs-lookup"><span data-stu-id="18530-128">string</span></span>  | <span data-ttu-id="18530-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18530-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18530-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18530-131">Request body</span></span>
<span data-ttu-id="18530-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="18530-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18530-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="18530-133">Parameter</span></span>    | <span data-ttu-id="18530-134">Typ</span><span class="sxs-lookup"><span data-stu-id="18530-134">Type</span></span>   |<span data-ttu-id="18530-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18530-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18530-136">Kommentar</span><span class="sxs-lookup"><span data-stu-id="18530-136">Comment</span></span>|<span data-ttu-id="18530-137">String</span><span class="sxs-lookup"><span data-stu-id="18530-137">String</span></span>|<span data-ttu-id="18530-p105">Ein Kommentar, der eingefügt werden kann. Kann eine leere Zeichenfolge sein.</span><span class="sxs-lookup"><span data-stu-id="18530-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="18530-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="18530-140">ToRecipients</span></span>|<span data-ttu-id="18530-141">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="18530-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="18530-142">Die Liste der Empfänger des Ereignisses zum Weiterleiten.</span><span class="sxs-lookup"><span data-stu-id="18530-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="18530-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="18530-143">Response</span></span>

<span data-ttu-id="18530-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18530-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18530-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18530-146">Example</span></span>
<span data-ttu-id="18530-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="18530-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18530-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18530-148">Request</span></span>
<span data-ttu-id="18530-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18530-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="18530-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="18530-150">Response</span></span>
<span data-ttu-id="18530-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18530-151">Here is an example of the response.</span></span>
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
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

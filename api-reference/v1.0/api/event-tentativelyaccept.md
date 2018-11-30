---
title: 'event: tentativelyAccept'
description: Mit Vorbehalt annehmen Sie das angegebene Ereignis in einem Benutzerkalender ein.
ms.openlocfilehash: ff3147f134a1ccd7efe4a2879bbd714c0d1433a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017352"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="902e3-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="902e3-103">event: tentativelyAccept</span></span>

<span data-ttu-id="902e3-104">Das angegebene [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md)des Benutzers mit Vorbehalt annehmen.</span><span class="sxs-lookup"><span data-stu-id="902e3-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="902e3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="902e3-105">Permissions</span></span>
<span data-ttu-id="902e3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="902e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="902e3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="902e3-108">Permission type</span></span>      | <span data-ttu-id="902e3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="902e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="902e3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="902e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="902e3-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="902e3-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="902e3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="902e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="902e3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="902e3-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="902e3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="902e3-114">Application</span></span> | <span data-ttu-id="902e3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="902e3-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="902e3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="902e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="902e3-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="902e3-117">Request headers</span></span>
| <span data-ttu-id="902e3-118">Name</span><span class="sxs-lookup"><span data-stu-id="902e3-118">Name</span></span>       | <span data-ttu-id="902e3-119">Typ</span><span class="sxs-lookup"><span data-stu-id="902e3-119">Type</span></span> | <span data-ttu-id="902e3-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="902e3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="902e3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="902e3-121">Authorization</span></span>  | <span data-ttu-id="902e3-122">string</span><span class="sxs-lookup"><span data-stu-id="902e3-122">string</span></span>  | <span data-ttu-id="902e3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="902e3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="902e3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="902e3-125">Content-Type</span></span> | <span data-ttu-id="902e3-126">string</span><span class="sxs-lookup"><span data-stu-id="902e3-126">string</span></span>  | <span data-ttu-id="902e3-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="902e3-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="902e3-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="902e3-129">Request body</span></span>
<span data-ttu-id="902e3-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="902e3-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="902e3-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="902e3-131">Parameter</span></span>    | <span data-ttu-id="902e3-132">Typ</span><span class="sxs-lookup"><span data-stu-id="902e3-132">Type</span></span>   |<span data-ttu-id="902e3-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="902e3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="902e3-134">comment</span><span class="sxs-lookup"><span data-stu-id="902e3-134">comment</span></span>|<span data-ttu-id="902e3-135">String</span><span class="sxs-lookup"><span data-stu-id="902e3-135">String</span></span>|<span data-ttu-id="902e3-p104">In der Antwort enthaltener Text. Optional.</span><span class="sxs-lookup"><span data-stu-id="902e3-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="902e3-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="902e3-138">sendResponse</span></span>|<span data-ttu-id="902e3-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="902e3-139">Boolean</span></span>|<span data-ttu-id="902e3-p105">`true`,wenn eine Antwort an den Organisator gesendet werden soll; andernfalls `false`. Optional. Der Standardwert lautet `true`.</span><span class="sxs-lookup"><span data-stu-id="902e3-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="902e3-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="902e3-143">Response</span></span>

<span data-ttu-id="902e3-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="902e3-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="902e3-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="902e3-146">Example</span></span>
<span data-ttu-id="902e3-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="902e3-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="902e3-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="902e3-148">Request</span></span>
<span data-ttu-id="902e3-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="902e3-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="902e3-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="902e3-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="902e3-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="902e3-151">Response</span></span>
<span data-ttu-id="902e3-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="902e3-152">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
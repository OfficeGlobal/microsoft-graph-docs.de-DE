---
title: 'event: accept'
description: Akzeptieren Sie das angegebene Ereignis in einem Benutzerkalender an.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: afff4a9eebb72fa9c624decb55d2677d4c5d41fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894467"
---
# <a name="event-accept"></a><span data-ttu-id="d13ab-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="d13ab-103">event: accept</span></span>

> <span data-ttu-id="d13ab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d13ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d13ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d13ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d13ab-106">Akzeptieren Sie das angegebene [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md)des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d13ab-106">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d13ab-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d13ab-107">Permissions</span></span>
<span data-ttu-id="d13ab-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d13ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d13ab-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d13ab-110">Permission type</span></span>      | <span data-ttu-id="d13ab-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d13ab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d13ab-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d13ab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d13ab-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d13ab-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d13ab-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d13ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d13ab-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d13ab-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d13ab-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d13ab-116">Application</span></span> | <span data-ttu-id="d13ab-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d13ab-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d13ab-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d13ab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="d13ab-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d13ab-119">Request headers</span></span>
| <span data-ttu-id="d13ab-120">Name</span><span class="sxs-lookup"><span data-stu-id="d13ab-120">Name</span></span>       | <span data-ttu-id="d13ab-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d13ab-121">Type</span></span> | <span data-ttu-id="d13ab-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d13ab-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d13ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d13ab-123">Authorization</span></span>  | <span data-ttu-id="d13ab-124">string</span><span class="sxs-lookup"><span data-stu-id="d13ab-124">string</span></span>  | <span data-ttu-id="d13ab-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d13ab-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d13ab-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d13ab-127">Content-Type</span></span> | <span data-ttu-id="d13ab-128">string</span><span class="sxs-lookup"><span data-stu-id="d13ab-128">string</span></span>  | <span data-ttu-id="d13ab-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d13ab-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d13ab-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d13ab-131">Request body</span></span>
<span data-ttu-id="d13ab-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d13ab-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d13ab-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="d13ab-133">Parameter</span></span>    | <span data-ttu-id="d13ab-134">Typ</span><span class="sxs-lookup"><span data-stu-id="d13ab-134">Type</span></span>   |<span data-ttu-id="d13ab-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d13ab-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d13ab-136">comment</span><span class="sxs-lookup"><span data-stu-id="d13ab-136">comment</span></span>|<span data-ttu-id="d13ab-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d13ab-137">String</span></span>|<span data-ttu-id="d13ab-p105">In der Antwort enthaltener Text. Optional.</span><span class="sxs-lookup"><span data-stu-id="d13ab-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="d13ab-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="d13ab-140">sendResponse</span></span>|<span data-ttu-id="d13ab-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d13ab-141">Boolean</span></span>|<span data-ttu-id="d13ab-p106">`true`,wenn eine Antwort an den Organisator gesendet werden soll; andernfalls `false`. Optional. Der Standardwert lautet `true`.</span><span class="sxs-lookup"><span data-stu-id="d13ab-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="d13ab-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="d13ab-145">Response</span></span>

<span data-ttu-id="d13ab-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d13ab-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d13ab-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d13ab-148">Example</span></span>
<span data-ttu-id="d13ab-149">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="d13ab-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d13ab-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d13ab-150">Request</span></span>
<span data-ttu-id="d13ab-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d13ab-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="d13ab-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="d13ab-152">Response</span></span>
<span data-ttu-id="d13ab-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d13ab-153">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'event: tentativelyAccept'
description: Mit Vorbehalt annehmen Sie das angegebene Ereignis in einem Benutzerkalender ein.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0ab714f4f80702dd99be0dde80c9caf307c5c14c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957676"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="4ea4e-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="4ea4e-103">event: tentativelyAccept</span></span>

<span data-ttu-id="4ea4e-104">Das angegebene [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md)des Benutzers mit Vorbehalt annehmen.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ea4e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4ea4e-105">Permissions</span></span>
<span data-ttu-id="4ea4e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea4e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ea4e-108">Permission type</span></span>      | <span data-ttu-id="4ea4e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ea4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ea4e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ea4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ea4e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ea4e-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4ea4e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ea4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ea4e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ea4e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4ea4e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ea4e-114">Application</span></span> | <span data-ttu-id="4ea4e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ea4e-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ea4e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ea4e-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="4ea4e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ea4e-117">Request headers</span></span>
| <span data-ttu-id="4ea4e-118">Name</span><span class="sxs-lookup"><span data-stu-id="4ea4e-118">Name</span></span>       | <span data-ttu-id="4ea4e-119">Typ</span><span class="sxs-lookup"><span data-stu-id="4ea4e-119">Type</span></span> | <span data-ttu-id="4ea4e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ea4e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ea4e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ea4e-121">Authorization</span></span>  | <span data-ttu-id="4ea4e-122">string</span><span class="sxs-lookup"><span data-stu-id="4ea4e-122">string</span></span>  | <span data-ttu-id="4ea4e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ea4e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ea4e-125">Content-Type</span></span> | <span data-ttu-id="4ea4e-126">string</span><span class="sxs-lookup"><span data-stu-id="4ea4e-126">string</span></span>  | <span data-ttu-id="4ea4e-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ea4e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ea4e-129">Request body</span></span>
<span data-ttu-id="4ea4e-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4ea4e-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="4ea4e-131">Parameter</span></span>    | <span data-ttu-id="4ea4e-132">Typ</span><span class="sxs-lookup"><span data-stu-id="4ea4e-132">Type</span></span>   |<span data-ttu-id="4ea4e-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ea4e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ea4e-134">comment</span><span class="sxs-lookup"><span data-stu-id="4ea4e-134">comment</span></span>|<span data-ttu-id="4ea4e-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ea4e-135">String</span></span>|<span data-ttu-id="4ea4e-p104">In der Antwort enthaltener Text. Optional.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="4ea4e-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="4ea4e-138">sendResponse</span></span>|<span data-ttu-id="4ea4e-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea4e-139">Boolean</span></span>|<span data-ttu-id="4ea4e-p105">`true`,wenn eine Antwort an den Organisator gesendet werden soll; andernfalls `false`. Optional. Der Standardwert lautet `true`.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="4ea4e-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ea4e-143">Response</span></span>

<span data-ttu-id="4ea4e-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea4e-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ea4e-146">Example</span></span>
<span data-ttu-id="4ea4e-147">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ea4e-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ea4e-148">Request</span></span>
<span data-ttu-id="4ea4e-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4ea4e-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ea4e-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="4ea4e-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ea4e-151">Response</span></span>
<span data-ttu-id="4ea4e-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-152">Here is an example of the response.</span></span>
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

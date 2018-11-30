---
title: Ereignis löschen
description: Mit dieser API können Sie Ereignisse löschen.
ms.openlocfilehash: 6f9ee81f60fc3a45018cb137288bad7f22fb98a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019537"
---
# <a name="delete-event"></a><span data-ttu-id="cb91e-103">Ereignis löschen</span><span class="sxs-lookup"><span data-stu-id="cb91e-103">Delete event</span></span>

<span data-ttu-id="cb91e-104">Mit dieser API können Sie Ereignisse löschen.</span><span class="sxs-lookup"><span data-stu-id="cb91e-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb91e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cb91e-105">Permissions</span></span>
<span data-ttu-id="cb91e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb91e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb91e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb91e-108">Permission type</span></span>      | <span data-ttu-id="cb91e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb91e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb91e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb91e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb91e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb91e-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cb91e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb91e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb91e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb91e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cb91e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb91e-114">Application</span></span> | <span data-ttu-id="cb91e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb91e-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb91e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb91e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cb91e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb91e-117">Request headers</span></span>
| <span data-ttu-id="cb91e-118">Name</span><span class="sxs-lookup"><span data-stu-id="cb91e-118">Name</span></span>       | <span data-ttu-id="cb91e-119">Typ</span><span class="sxs-lookup"><span data-stu-id="cb91e-119">Type</span></span> | <span data-ttu-id="cb91e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb91e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cb91e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb91e-121">Authorization</span></span>  | <span data-ttu-id="cb91e-122">string</span><span class="sxs-lookup"><span data-stu-id="cb91e-122">string</span></span>  | <span data-ttu-id="cb91e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb91e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb91e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb91e-125">Request body</span></span>
<span data-ttu-id="cb91e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cb91e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb91e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb91e-127">Response</span></span>

<span data-ttu-id="cb91e-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb91e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb91e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb91e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb91e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb91e-131">Request</span></span>
<span data-ttu-id="cb91e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb91e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="cb91e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb91e-133">Response</span></span>
<span data-ttu-id="cb91e-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cb91e-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

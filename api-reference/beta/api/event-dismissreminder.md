---
title: 'event: dismissReminder'
description: Schließen Sie eine Erinnerung, die in einem Benutzerkalender für ein Ereignis ausgelöst wurde.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 885a285e3c35f59b0fde76be5c84ae152a2ad13a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523050"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="06c4f-103">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="06c4f-103">event: dismissReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06c4f-104">Schließen Sie eine Erinnerung, die für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md)des Benutzers ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="06c4f-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06c4f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06c4f-105">Permissions</span></span>
<span data-ttu-id="06c4f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06c4f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06c4f-108">Permission type</span></span>      | <span data-ttu-id="06c4f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06c4f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06c4f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06c4f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06c4f-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06c4f-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="06c4f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06c4f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06c4f-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06c4f-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="06c4f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06c4f-114">Application</span></span> | <span data-ttu-id="06c4f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06c4f-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="06c4f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06c4f-116">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="06c4f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06c4f-117">Request headers</span></span>

| <span data-ttu-id="06c4f-118">Name</span><span class="sxs-lookup"><span data-stu-id="06c4f-118">Name</span></span>       | <span data-ttu-id="06c4f-119">Typ</span><span class="sxs-lookup"><span data-stu-id="06c4f-119">Type</span></span> | <span data-ttu-id="06c4f-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06c4f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="06c4f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06c4f-121">Authorization</span></span>  | <span data-ttu-id="06c4f-122">string</span><span class="sxs-lookup"><span data-stu-id="06c4f-122">string</span></span>  | <span data-ttu-id="06c4f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06c4f-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="06c4f-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="06c4f-125">Response</span></span>

<span data-ttu-id="06c4f-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06c4f-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06c4f-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06c4f-128">Example</span></span>

<span data-ttu-id="06c4f-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="06c4f-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="06c4f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06c4f-130">Request</span></span>
<span data-ttu-id="06c4f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06c4f-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="06c4f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="06c4f-132">Response</span></span>
<span data-ttu-id="06c4f-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="06c4f-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-dismissreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

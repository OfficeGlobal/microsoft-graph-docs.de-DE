---
title: Kalender löschen
description: Mit dieser API können Sie Kalender löschen (nicht jedoch den Standardkalender).
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af1fe9a0b13aeb20a269b39bac8966bcc31508b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937418"
---
# <a name="delete-calendar"></a><span data-ttu-id="8bf2b-103">Kalender löschen</span><span class="sxs-lookup"><span data-stu-id="8bf2b-103">Delete calendar</span></span>

<span data-ttu-id="8bf2b-104">Mit dieser API können Sie Kalender löschen (nicht jedoch den Standardkalender).</span><span class="sxs-lookup"><span data-stu-id="8bf2b-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="8bf2b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8bf2b-105">Permissions</span></span>
<span data-ttu-id="8bf2b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bf2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bf2b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8bf2b-108">Permission type</span></span>      | <span data-ttu-id="8bf2b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8bf2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bf2b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8bf2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bf2b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bf2b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8bf2b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8bf2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bf2b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bf2b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8bf2b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8bf2b-114">Application</span></span> | <span data-ttu-id="8bf2b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bf2b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bf2b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bf2b-116">HTTP request</span></span>
<span data-ttu-id="8bf2b-117"><!-- { "blockType": "ignored" } -->Ein Benutzer [Kalender](../resources/calendar.md) als Standardkalender in der Standardeinstellung [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="8bf2b-117"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="8bf2b-118">Ein anderer [Kalender](../resources/calendar.md) als der Standardkalender in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="8bf2b-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8bf2b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8bf2b-119">Request headers</span></span>
| <span data-ttu-id="8bf2b-120">Name</span><span class="sxs-lookup"><span data-stu-id="8bf2b-120">Name</span></span>           |  <span data-ttu-id="8bf2b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8bf2b-121">Type</span></span>    | <span data-ttu-id="8bf2b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bf2b-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="8bf2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bf2b-123">Authorization</span></span>  |  <span data-ttu-id="8bf2b-124">string</span><span class="sxs-lookup"><span data-stu-id="8bf2b-124">string</span></span>  | <span data-ttu-id="8bf2b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8bf2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bf2b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8bf2b-127">Request body</span></span>
<span data-ttu-id="8bf2b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8bf2b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bf2b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bf2b-129">Response</span></span>

<span data-ttu-id="8bf2b-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8bf2b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bf2b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8bf2b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bf2b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bf2b-133">Request</span></span>
<span data-ttu-id="8bf2b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8bf2b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="8bf2b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bf2b-135">Response</span></span>
<span data-ttu-id="8bf2b-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8bf2b-136">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

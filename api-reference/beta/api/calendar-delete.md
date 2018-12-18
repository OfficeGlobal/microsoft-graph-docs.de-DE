---
title: Kalender löschen
description: Mit dieser API können Sie Kalender löschen (nicht jedoch den Standardkalender).
author: angelgolfer-ms
ms.openlocfilehash: d8e2a7aaaff9f4489d5ef1cbcae97bcdbceb8f17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348790"
---
# <a name="delete-calendar"></a><span data-ttu-id="78373-103">Kalender löschen</span><span class="sxs-lookup"><span data-stu-id="78373-103">Delete calendar</span></span>

> <span data-ttu-id="78373-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="78373-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78373-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78373-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78373-106">Mit dieser API können Sie Kalender löschen (nicht jedoch den Standardkalender).</span><span class="sxs-lookup"><span data-stu-id="78373-106">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="78373-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="78373-107">Permissions</span></span>
<span data-ttu-id="78373-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78373-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78373-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="78373-110">Permission type</span></span>      | <span data-ttu-id="78373-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="78373-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78373-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="78373-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78373-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78373-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="78373-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="78373-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78373-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78373-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="78373-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="78373-116">Application</span></span> | <span data-ttu-id="78373-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78373-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="78373-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="78373-118">HTTP request</span></span>
<span data-ttu-id="78373-119"><!-- { "blockType": "ignored" } -->Ein Benutzer [Kalender](../resources/calendar.md) als Standardkalender in der Standardeinstellung [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="78373-119"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="78373-120">Ein anderer [Kalender](../resources/calendar.md) als der Standardkalender in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="78373-120">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="78373-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="78373-121">Request headers</span></span>
| <span data-ttu-id="78373-122">Name</span><span class="sxs-lookup"><span data-stu-id="78373-122">Name</span></span>           |  <span data-ttu-id="78373-123">Typ</span><span class="sxs-lookup"><span data-stu-id="78373-123">Type</span></span>    | <span data-ttu-id="78373-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78373-124">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="78373-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="78373-125">Authorization</span></span>  |  <span data-ttu-id="78373-126">string</span><span class="sxs-lookup"><span data-stu-id="78373-126">string</span></span>  | <span data-ttu-id="78373-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="78373-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78373-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="78373-129">Request body</span></span>
<span data-ttu-id="78373-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="78373-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78373-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="78373-131">Response</span></span>

<span data-ttu-id="78373-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="78373-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78373-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="78373-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78373-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="78373-135">Request</span></span>
<span data-ttu-id="78373-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="78373-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="78373-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="78373-137">Response</span></span>
<span data-ttu-id="78373-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="78373-138">Here is an example of the response.</span></span> 
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

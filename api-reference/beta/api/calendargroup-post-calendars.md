---
title: Kalender erstellen
description: Mit dieser API können Sie in einer Kalendergruppe einen neuen Kalender für einen Benutzer erstellen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5cb13fc6259d21a752160b2a932f9a7c5b2330bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819733"
---
# <a name="create-calendar"></a><span data-ttu-id="00c2d-103">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="00c2d-103">Create Calendar</span></span>

> <span data-ttu-id="00c2d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="00c2d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00c2d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00c2d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00c2d-106">Mit dieser API können Sie in einer Kalendergruppe einen neuen Kalender für einen [Benutzer](../resources/user.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="00c2d-106">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="00c2d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="00c2d-107">Permissions</span></span>

<span data-ttu-id="00c2d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00c2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00c2d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00c2d-110">Permission type</span></span>                        | <span data-ttu-id="00c2d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00c2d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="00c2d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00c2d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="00c2d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00c2d-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="00c2d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00c2d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00c2d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00c2d-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="00c2d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00c2d-116">Application</span></span>                            | <span data-ttu-id="00c2d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00c2d-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="00c2d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00c2d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="00c2d-119">Die standardmäßige [CalendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="00c2d-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="00c2d-120">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="00c2d-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="00c2d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00c2d-121">Request headers</span></span>

| <span data-ttu-id="00c2d-122">Header</span><span class="sxs-lookup"><span data-stu-id="00c2d-122">Header</span></span>        | <span data-ttu-id="00c2d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="00c2d-123">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="00c2d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="00c2d-124">Authorization</span></span> | <span data-ttu-id="00c2d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="00c2d-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="00c2d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00c2d-127">Content-Type</span></span>  | <span data-ttu-id="00c2d-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="00c2d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00c2d-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00c2d-130">Request body</span></span>

<span data-ttu-id="00c2d-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="00c2d-131">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00c2d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="00c2d-132">Response</span></span>

<span data-ttu-id="00c2d-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00c2d-133">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00c2d-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00c2d-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="00c2d-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00c2d-135">Request</span></span>

<span data-ttu-id="00c2d-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00c2d-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="00c2d-137">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="00c2d-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="00c2d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="00c2d-138">Response</span></span>

<span data-ttu-id="00c2d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00c2d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

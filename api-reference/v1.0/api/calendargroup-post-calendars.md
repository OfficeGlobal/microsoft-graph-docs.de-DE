---
title: Kalender erstellen
description: Mit dieser API können Sie in einer Kalendergruppe einen neuen Kalender für einen Benutzer erstellen.
ms.openlocfilehash: fad4b3ebf0488d6619cdd0550dd7c9456640e69f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018705"
---
# <a name="create-calendar"></a><span data-ttu-id="4d8b2-103">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="4d8b2-103">Create Calendar</span></span>

<span data-ttu-id="4d8b2-104">Mit dieser API können Sie in einer Kalendergruppe einen neuen Kalender für einen [Benutzer](../resources/user.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-104">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d8b2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d8b2-105">Permissions</span></span>

<span data-ttu-id="4d8b2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d8b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d8b2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d8b2-108">Permission type</span></span>                        | <span data-ttu-id="4d8b2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d8b2-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4d8b2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d8b2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d8b2-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d8b2-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="4d8b2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d8b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d8b2-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d8b2-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="4d8b2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d8b2-114">Application</span></span>                            | <span data-ttu-id="4d8b2-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d8b2-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4d8b2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d8b2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="4d8b2-117">Die standardmäßige [CalendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="4d8b2-118">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="4d8b2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d8b2-119">Request headers</span></span>

| <span data-ttu-id="4d8b2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4d8b2-120">Header</span></span>        | <span data-ttu-id="4d8b2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4d8b2-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="4d8b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d8b2-122">Authorization</span></span> | <span data-ttu-id="4d8b2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4d8b2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d8b2-125">Content-Type</span></span>  | <span data-ttu-id="4d8b2-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="4d8b2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d8b2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d8b2-128">Request body</span></span>

<span data-ttu-id="4d8b2-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-129">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d8b2-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d8b2-130">Response</span></span>

<span data-ttu-id="4d8b2-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-131">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d8b2-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d8b2-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d8b2-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d8b2-133">Request</span></span>

<span data-ttu-id="4d8b2-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="4d8b2-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-135">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="4d8b2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d8b2-136">Response</span></span>

<span data-ttu-id="4d8b2-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d8b2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
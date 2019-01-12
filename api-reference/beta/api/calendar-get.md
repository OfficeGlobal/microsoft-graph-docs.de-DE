---
title: Kalender abrufen
description: 'Dient zum Abrufen der Eigenschaften und der Beziehungen eines calendar-Objekts. Der Kalender möglich für einen Benutzer, '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d54d408966e359a99c16c91113ea5ba7eebb3d1d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990629"
---
# <a name="get-calendar"></a><span data-ttu-id="4b75e-104">Kalender abrufen</span><span class="sxs-lookup"><span data-stu-id="4b75e-104">Get calendar</span></span>

> <span data-ttu-id="4b75e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4b75e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b75e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b75e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b75e-107">Dient zum Abrufen der Eigenschaften und der Beziehungen eines [calendar](../resources/calendar.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b75e-107">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="4b75e-108">Dies kann ein Kalender für einen [Benutzer](../resources/user.md) oder der Standardkalender einer Office 365-[Gruppe](../resources/group.md) sein.</span><span class="sxs-lookup"><span data-stu-id="4b75e-108">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="4b75e-109">Es gibt zwei Szenarien, in dem eine app Kalender des Benutzers abgerufen werden kann:</span><span class="sxs-lookup"><span data-stu-id="4b75e-109">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="4b75e-110">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="4b75e-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="4b75e-111">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen Kalender freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="4b75e-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="4b75e-112">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="4b75e-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="4b75e-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4b75e-113">Permissions</span></span>
<span data-ttu-id="4b75e-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b75e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b75e-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b75e-116">Permission type</span></span>      | <span data-ttu-id="4b75e-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b75e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b75e-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b75e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="4b75e-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4b75e-119">Calendars.Read</span></span>    |
|<span data-ttu-id="4b75e-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b75e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b75e-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4b75e-121">Calendars.Read</span></span>    |
|<span data-ttu-id="4b75e-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b75e-122">Application</span></span> | <span data-ttu-id="4b75e-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4b75e-123">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b75e-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b75e-124">HTTP request</span></span>
<span data-ttu-id="4b75e-125"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="4b75e-125"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="4b75e-126">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="4b75e-126">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="4b75e-127">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="4b75e-127">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b75e-128">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4b75e-128">Optional query parameters</span></span>
<span data-ttu-id="4b75e-129">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4b75e-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4b75e-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b75e-130">Request headers</span></span>
| <span data-ttu-id="4b75e-131">Name</span><span class="sxs-lookup"><span data-stu-id="4b75e-131">Name</span></span>       | <span data-ttu-id="4b75e-132">Typ</span><span class="sxs-lookup"><span data-stu-id="4b75e-132">Type</span></span> | <span data-ttu-id="4b75e-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b75e-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4b75e-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b75e-134">Authorization</span></span>  | <span data-ttu-id="4b75e-135">string</span><span class="sxs-lookup"><span data-stu-id="4b75e-135">string</span></span>  | <span data-ttu-id="4b75e-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b75e-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b75e-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b75e-138">Request body</span></span>
<span data-ttu-id="4b75e-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4b75e-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b75e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b75e-140">Response</span></span>

<span data-ttu-id="4b75e-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b75e-141">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b75e-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b75e-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b75e-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b75e-143">Request</span></span>
<span data-ttu-id="4b75e-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b75e-144">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```

##### <a name="response"></a><span data-ttu-id="4b75e-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b75e-145">Response</span></span>
<span data-ttu-id="4b75e-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b75e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "isDefaultCalendar": false,
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

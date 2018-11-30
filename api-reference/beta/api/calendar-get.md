---
title: Kalender abrufen
description: 'Dient zum Abrufen der Eigenschaften und der Beziehungen eines calendar-Objekts. Der Kalender möglich für einen Benutzer, '
ms.openlocfilehash: b4dd218e25d154fa1641a7a62d3b79790a15f7da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058108"
---
# <a name="get-calendar"></a><span data-ttu-id="23c67-104">Kalender abrufen</span><span class="sxs-lookup"><span data-stu-id="23c67-104">Get calendar</span></span>

> <span data-ttu-id="23c67-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23c67-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23c67-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23c67-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23c67-107">Dient zum Abrufen der Eigenschaften und der Beziehungen eines [calendar](../resources/calendar.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="23c67-107">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="23c67-108">Dies kann ein Kalender für einen [Benutzer](../resources/user.md) oder der Standardkalender einer Office 365-[Gruppe](../resources/group.md) sein.</span><span class="sxs-lookup"><span data-stu-id="23c67-108">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="23c67-109">Es gibt zwei Szenarien, in dem eine app Kalender des Benutzers abgerufen werden kann:</span><span class="sxs-lookup"><span data-stu-id="23c67-109">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="23c67-110">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="23c67-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="23c67-111">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen Kalender freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="23c67-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="23c67-112">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="23c67-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="23c67-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="23c67-113">Permissions</span></span>
<span data-ttu-id="23c67-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23c67-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23c67-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23c67-116">Permission type</span></span>      | <span data-ttu-id="23c67-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23c67-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23c67-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23c67-118">Delegated (work or school account)</span></span> | <span data-ttu-id="23c67-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="23c67-119">Calendars.Read</span></span>    |
|<span data-ttu-id="23c67-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23c67-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23c67-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="23c67-121">Calendars.Read</span></span>    |
|<span data-ttu-id="23c67-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23c67-122">Application</span></span> | <span data-ttu-id="23c67-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="23c67-123">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="23c67-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23c67-124">HTTP request</span></span>
<span data-ttu-id="23c67-125"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="23c67-125"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="23c67-126">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="23c67-126">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="23c67-127">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="23c67-127">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23c67-128">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="23c67-128">Optional query parameters</span></span>
<span data-ttu-id="23c67-129">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="23c67-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23c67-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23c67-130">Request headers</span></span>
| <span data-ttu-id="23c67-131">Name</span><span class="sxs-lookup"><span data-stu-id="23c67-131">Name</span></span>       | <span data-ttu-id="23c67-132">Typ</span><span class="sxs-lookup"><span data-stu-id="23c67-132">Type</span></span> | <span data-ttu-id="23c67-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23c67-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23c67-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="23c67-134">Authorization</span></span>  | <span data-ttu-id="23c67-135">string</span><span class="sxs-lookup"><span data-stu-id="23c67-135">string</span></span>  | <span data-ttu-id="23c67-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23c67-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23c67-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23c67-138">Request body</span></span>
<span data-ttu-id="23c67-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="23c67-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23c67-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="23c67-140">Response</span></span>

<span data-ttu-id="23c67-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23c67-141">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23c67-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23c67-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23c67-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23c67-143">Request</span></span>
<span data-ttu-id="23c67-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23c67-144">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```

##### <a name="response"></a><span data-ttu-id="23c67-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="23c67-145">Response</span></span>
<span data-ttu-id="23c67-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23c67-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

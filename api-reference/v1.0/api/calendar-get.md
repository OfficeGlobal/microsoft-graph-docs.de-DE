---
title: Kalender abrufen
description: 'Dient zum Abrufen der Eigenschaften und der Beziehungen eines calendar-Objekts. Der Kalender möglich für einen Benutzer, '
ms.openlocfilehash: f4ddefe694ea3afb03d9c6b1791f7774347deff3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018062"
---
# <a name="get-calendar"></a><span data-ttu-id="6d6e1-104">Kalender abrufen</span><span class="sxs-lookup"><span data-stu-id="6d6e1-104">Get calendar</span></span>

<span data-ttu-id="6d6e1-105">Dient zum Abrufen der Eigenschaften und der Beziehungen eines [calendar](../resources/calendar.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="6d6e1-106">Dies kann ein Kalender für einen [Benutzer](../resources/user.md) oder der Standardkalender einer Office 365-[Gruppe](../resources/group.md) sein.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="6d6e1-107">Es gibt zwei Szenarien, in dem eine app Kalender des Benutzers abgerufen werden kann:</span><span class="sxs-lookup"><span data-stu-id="6d6e1-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="6d6e1-108">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="6d6e1-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6d6e1-109">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen Kalender freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6d6e1-110">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="6d6e1-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d6e1-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6d6e1-111">Permissions</span></span>
<span data-ttu-id="6d6e1-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d6e1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d6e1-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d6e1-114">Permission type</span></span>      | <span data-ttu-id="6d6e1-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d6e1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d6e1-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d6e1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6d6e1-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6d6e1-117">Calendars.Read</span></span>    |
|<span data-ttu-id="6d6e1-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d6e1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d6e1-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6d6e1-119">Calendars.Read</span></span>    |
|<span data-ttu-id="6d6e1-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d6e1-120">Application</span></span> | <span data-ttu-id="6d6e1-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6d6e1-121">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d6e1-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d6e1-122">HTTP request</span></span>
<span data-ttu-id="6d6e1-123"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="6d6e1-123"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="6d6e1-124">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="6d6e1-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="6d6e1-125">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="6d6e1-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d6e1-126">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6d6e1-126">Optional query parameters</span></span>
<span data-ttu-id="6d6e1-127">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6d6e1-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d6e1-128">Request headers</span></span>
| <span data-ttu-id="6d6e1-129">Name</span><span class="sxs-lookup"><span data-stu-id="6d6e1-129">Name</span></span>       | <span data-ttu-id="6d6e1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6d6e1-130">Type</span></span> | <span data-ttu-id="6d6e1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d6e1-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d6e1-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d6e1-132">Authorization</span></span>  | <span data-ttu-id="6d6e1-133">string</span><span class="sxs-lookup"><span data-stu-id="6d6e1-133">string</span></span>  | <span data-ttu-id="6d6e1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d6e1-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d6e1-136">Request body</span></span>
<span data-ttu-id="6d6e1-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d6e1-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d6e1-138">Response</span></span>

<span data-ttu-id="6d6e1-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-139">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d6e1-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d6e1-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d6e1-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d6e1-141">Request</span></span>
<span data-ttu-id="6d6e1-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="6d6e1-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d6e1-143">Response</span></span>
<span data-ttu-id="6d6e1-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d6e1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
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

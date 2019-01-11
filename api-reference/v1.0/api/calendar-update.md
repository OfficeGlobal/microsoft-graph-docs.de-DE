---
title: Kalender aktualisieren
description: 'Aktualisieren Sie die Eigenschaften eines calendar-Objekts. Der Kalender möglich für einen Benutzer, '
localization_priority: Normal
ms.openlocfilehash: f56ce185718c2a639f32606b9db79f0154a824e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857113"
---
# <a name="update-calendar"></a><span data-ttu-id="73deb-104">Kalender aktualisieren</span><span class="sxs-lookup"><span data-stu-id="73deb-104">Update calendar</span></span>

<span data-ttu-id="73deb-105">Aktualisieren Sie die Eigenschaften eines [calendar](../resources/calendar.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73deb-105">Update the properties of of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="73deb-106">Dies kann ein Kalender für einen [Benutzer](../resources/user.md) oder der Standardkalender einer Office 365-[Gruppe](../resources/group.md) sein.</span><span class="sxs-lookup"><span data-stu-id="73deb-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="73deb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="73deb-107">Permissions</span></span>
<span data-ttu-id="73deb-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73deb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73deb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73deb-110">Permission type</span></span>      | <span data-ttu-id="73deb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73deb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73deb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73deb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="73deb-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73deb-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="73deb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73deb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73deb-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73deb-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="73deb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73deb-116">Application</span></span> | <span data-ttu-id="73deb-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73deb-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="73deb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73deb-118">HTTP request</span></span>
<span data-ttu-id="73deb-119"><!-- { "blockType": "ignored" } -->Eines Benutzers oder einer Gruppe als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="73deb-119"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
PATCH /me/calendar
PATCH /users/{id | userPrincipalName}/calendar
PATCH /groups/{id}/calendar
```
<span data-ttu-id="73deb-120">Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="73deb-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}

PATCH /me/calendarGroup/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="73deb-121">Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="73deb-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
PATCH /me/calendarGroups/{id}/calendars/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="73deb-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73deb-122">Request headers</span></span>
| <span data-ttu-id="73deb-123">Header</span><span class="sxs-lookup"><span data-stu-id="73deb-123">Header</span></span>       | <span data-ttu-id="73deb-124">Wert</span><span class="sxs-lookup"><span data-stu-id="73deb-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73deb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="73deb-125">Authorization</span></span>  | <span data-ttu-id="73deb-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="73deb-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73deb-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73deb-128">Content-Type</span></span>  | <span data-ttu-id="73deb-p105">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="73deb-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73deb-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73deb-131">Request body</span></span>
<span data-ttu-id="73deb-p106">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="73deb-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="73deb-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73deb-135">Property</span></span>     | <span data-ttu-id="73deb-136">Typ</span><span class="sxs-lookup"><span data-stu-id="73deb-136">Type</span></span>   |<span data-ttu-id="73deb-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73deb-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73deb-138">color</span><span class="sxs-lookup"><span data-stu-id="73deb-138">color</span></span>|<span data-ttu-id="73deb-139">String</span><span class="sxs-lookup"><span data-stu-id="73deb-139">String</span></span>|<span data-ttu-id="73deb-p107">Gibt das Farbdesign an, um den Kalender von anderen Kalendern in einer Benutzeroberfläche zu unterscheiden. Die Eigenschaftswerte sind: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="73deb-p107">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="73deb-142">name</span><span class="sxs-lookup"><span data-stu-id="73deb-142">name</span></span>|<span data-ttu-id="73deb-143">String</span><span class="sxs-lookup"><span data-stu-id="73deb-143">String</span></span>|<span data-ttu-id="73deb-144">Der Kalendername.</span><span class="sxs-lookup"><span data-stu-id="73deb-144">The calendar name.</span></span>|

## <a name="response"></a><span data-ttu-id="73deb-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="73deb-145">Response</span></span>

<span data-ttu-id="73deb-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73deb-146">If successful, this method returns a `200 OK` response code and updated [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73deb-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73deb-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73deb-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73deb-148">Request</span></span>
<span data-ttu-id="73deb-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73deb-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendar
Content-type: application/json

{
  "name": "Social events"
}
```
##### <a name="response"></a><span data-ttu-id="73deb-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="73deb-150">Response</span></span>
<span data-ttu-id="73deb-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73deb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Social events",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
  "description": "Update calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

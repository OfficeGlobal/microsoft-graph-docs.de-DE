---
title: Kalender erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen Kalenders für einen Benutzer.
ms.openlocfilehash: 7cb1dbf60cacfb86ee79d9cf9d344dae878fd1f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059796"
---
# <a name="create-calendar"></a><span data-ttu-id="848a1-103">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="848a1-103">Create Calendar</span></span>

> <span data-ttu-id="848a1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="848a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="848a1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="848a1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="848a1-106">Verwenden Sie diese API zum Erstellen eines neuen Kalenders für einen [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="848a1-106">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="848a1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="848a1-107">Permissions</span></span>
<span data-ttu-id="848a1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="848a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="848a1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="848a1-110">Permission type</span></span>      | <span data-ttu-id="848a1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="848a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="848a1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="848a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="848a1-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="848a1-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="848a1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="848a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="848a1-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="848a1-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="848a1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="848a1-116">Application</span></span> | <span data-ttu-id="848a1-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="848a1-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="848a1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="848a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="848a1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="848a1-119">Request headers</span></span>
| <span data-ttu-id="848a1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="848a1-120">Header</span></span>       | <span data-ttu-id="848a1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="848a1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="848a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="848a1-122">Authorization</span></span>  | <span data-ttu-id="848a1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="848a1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="848a1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="848a1-125">Content-Type</span></span>  | <span data-ttu-id="848a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="848a1-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="848a1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="848a1-127">Request body</span></span>
<span data-ttu-id="848a1-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="848a1-128">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="848a1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="848a1-129">Response</span></span>

<span data-ttu-id="848a1-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="848a1-130">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="848a1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="848a1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="848a1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="848a1-132">Request</span></span>
<span data-ttu-id="848a1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="848a1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}

```
<span data-ttu-id="848a1-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="848a1-134">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="848a1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="848a1-135">Response</span></span>
<span data-ttu-id="848a1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="848a1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
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
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
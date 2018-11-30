---
title: Kalender erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen Kalenders für einen Benutzer.
ms.openlocfilehash: 8ffa88331478d7bbbe1e94c87d58505041d63d41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019517"
---
# <a name="create-calendar"></a><span data-ttu-id="cd561-103">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="cd561-103">Create Calendar</span></span>

<span data-ttu-id="cd561-104">Verwenden Sie diese API zum Erstellen eines neuen Kalenders für einen [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="cd561-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="cd561-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd561-105">Permissions</span></span>
<span data-ttu-id="cd561-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd561-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd561-108">Permission type</span></span>      | <span data-ttu-id="cd561-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd561-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd561-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd561-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd561-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd561-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cd561-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd561-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd561-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd561-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="cd561-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd561-114">Application</span></span> | <span data-ttu-id="cd561-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd561-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd561-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd561-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="cd561-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd561-117">Request headers</span></span>
| <span data-ttu-id="cd561-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd561-118">Header</span></span>       | <span data-ttu-id="cd561-119">Wert</span><span class="sxs-lookup"><span data-stu-id="cd561-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd561-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd561-120">Authorization</span></span>  | <span data-ttu-id="cd561-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd561-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd561-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd561-123">Content-Type</span></span>  | <span data-ttu-id="cd561-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cd561-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd561-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd561-125">Request body</span></span>
<span data-ttu-id="cd561-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cd561-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cd561-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd561-127">Response</span></span>

<span data-ttu-id="cd561-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd561-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd561-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd561-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd561-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd561-130">Request</span></span>
<span data-ttu-id="cd561-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd561-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="cd561-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cd561-132">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cd561-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd561-133">Response</span></span>
<span data-ttu-id="cd561-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd561-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
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
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
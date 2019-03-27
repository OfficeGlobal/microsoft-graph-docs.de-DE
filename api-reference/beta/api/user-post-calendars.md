---
title: Kalender erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen Kalenders für einen Benutzer.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afbb37d9394f2c08c94c6c8f41c56431e6938831
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869330"
---
# <a name="create-calendar"></a><span data-ttu-id="0f941-103">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="0f941-103">Create Calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f941-104">Verwenden Sie diese API zum Erstellen eines neuen Kalenders für einen [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="0f941-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0f941-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f941-105">Permissions</span></span>
<span data-ttu-id="0f941-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f941-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f941-108">Permission type</span></span>      | <span data-ttu-id="0f941-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f941-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f941-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f941-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f941-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f941-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0f941-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f941-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f941-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f941-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0f941-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f941-114">Application</span></span> | <span data-ttu-id="0f941-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f941-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f941-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f941-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="0f941-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f941-117">Request headers</span></span>
| <span data-ttu-id="0f941-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0f941-118">Header</span></span>       | <span data-ttu-id="0f941-119">Wert</span><span class="sxs-lookup"><span data-stu-id="0f941-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f941-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f941-120">Authorization</span></span>  | <span data-ttu-id="0f941-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f941-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f941-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f941-123">Content-Type</span></span>  | <span data-ttu-id="0f941-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f941-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f941-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f941-125">Request body</span></span>
<span data-ttu-id="0f941-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0f941-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0f941-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f941-127">Response</span></span>

<span data-ttu-id="0f941-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [calendar](../resources/calendar.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f941-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f941-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f941-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f941-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f941-130">Request</span></span>
<span data-ttu-id="0f941-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f941-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="0f941-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendar](../resources/calendar.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0f941-132">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0f941-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f941-133">Response</span></span>
<span data-ttu-id="0f941-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f941-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-calendars.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

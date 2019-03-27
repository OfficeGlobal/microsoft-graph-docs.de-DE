---
title: CalendarGroup erstellen
description: Mit dieser API können Sie eine neue Ressource des Typs „CalendarGroup“ erstellen.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 922fa813009090e504a71049ca0f8c717fc48354
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869477"
---
# <a name="create-calendargroup"></a><span data-ttu-id="b493b-103">CalendarGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="b493b-103">Create CalendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b493b-104">Mit dieser API können Sie eine neue Ressource des Typs „CalendarGroup“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="b493b-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="b493b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b493b-105">Permissions</span></span>
<span data-ttu-id="b493b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b493b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b493b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b493b-108">Permission type</span></span>      | <span data-ttu-id="b493b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b493b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b493b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b493b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b493b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b493b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b493b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b493b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b493b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b493b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b493b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b493b-114">Application</span></span> | <span data-ttu-id="b493b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b493b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b493b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b493b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="b493b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b493b-117">Request headers</span></span>
| <span data-ttu-id="b493b-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b493b-118">Header</span></span>       | <span data-ttu-id="b493b-119">Wert</span><span class="sxs-lookup"><span data-stu-id="b493b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b493b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b493b-120">Authorization</span></span>  | <span data-ttu-id="b493b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b493b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b493b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b493b-123">Content-Type</span></span>  | <span data-ttu-id="b493b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b493b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b493b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b493b-125">Request body</span></span>
<span data-ttu-id="b493b-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [CalendarGroup](../resources/calendargroup.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b493b-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b493b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b493b-127">Response</span></span>

<span data-ttu-id="b493b-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [CalendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b493b-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b493b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b493b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b493b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b493b-130">Request</span></span>
<span data-ttu-id="b493b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b493b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="b493b-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendarGroup](../resources/calendargroup.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b493b-132">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b493b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b493b-133">Response</span></span>
<span data-ttu-id="b493b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b493b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-calendargroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: CalendarGroup erstellen
description: Mit dieser API können Sie eine neue Ressource des Typs „CalendarGroup“ erstellen.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 0a969c2f9916bf94d05f4082f6c429460652c860
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834785"
---
# <a name="create-calendargroup"></a><span data-ttu-id="f5cd7-103">CalendarGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="f5cd7-103">Create CalendarGroup</span></span>

<span data-ttu-id="f5cd7-104">Mit dieser API können Sie eine neue Ressource des Typs „CalendarGroup“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="f5cd7-104">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5cd7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f5cd7-105">Permissions</span></span>
<span data-ttu-id="f5cd7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5cd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5cd7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5cd7-108">Permission type</span></span>      | <span data-ttu-id="f5cd7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5cd7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5cd7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5cd7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f5cd7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5cd7-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f5cd7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5cd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5cd7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5cd7-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f5cd7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5cd7-114">Application</span></span> | <span data-ttu-id="f5cd7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5cd7-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5cd7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5cd7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="f5cd7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5cd7-117">Request headers</span></span>
| <span data-ttu-id="f5cd7-118">Header</span><span class="sxs-lookup"><span data-stu-id="f5cd7-118">Header</span></span>       | <span data-ttu-id="f5cd7-119">Wert</span><span class="sxs-lookup"><span data-stu-id="f5cd7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5cd7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5cd7-120">Authorization</span></span>  | <span data-ttu-id="f5cd7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5cd7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5cd7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5cd7-123">Content-Type</span></span>  | <span data-ttu-id="f5cd7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f5cd7-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5cd7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5cd7-125">Request body</span></span>
<span data-ttu-id="f5cd7-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [CalendarGroup](../resources/calendargroup.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f5cd7-126">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f5cd7-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5cd7-127">Response</span></span>

<span data-ttu-id="f5cd7-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [CalendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5cd7-128">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5cd7-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5cd7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5cd7-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5cd7-130">Request</span></span>
<span data-ttu-id="f5cd7-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5cd7-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="f5cd7-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendarGroup](../resources/calendargroup.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f5cd7-132">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f5cd7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5cd7-133">Response</span></span>
<span data-ttu-id="f5cd7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5cd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

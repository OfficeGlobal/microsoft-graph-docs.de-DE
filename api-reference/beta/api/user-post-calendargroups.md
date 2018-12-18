---
title: CalendarGroup erstellen
description: Mit dieser API können Sie eine neue Ressource des Typs „CalendarGroup“ erstellen.
author: dkershaw10
ms.openlocfilehash: a68be3470489b20667112b67d15f4472a3817d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319047"
---
# <a name="create-calendargroup"></a><span data-ttu-id="70458-103">CalendarGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="70458-103">Create CalendarGroup</span></span>

> <span data-ttu-id="70458-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="70458-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70458-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70458-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70458-106">Mit dieser API können Sie eine neue Ressource des Typs „CalendarGroup“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="70458-106">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="70458-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="70458-107">Permissions</span></span>
<span data-ttu-id="70458-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70458-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70458-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70458-110">Permission type</span></span>      | <span data-ttu-id="70458-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70458-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70458-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70458-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70458-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70458-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="70458-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70458-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70458-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70458-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="70458-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70458-116">Application</span></span> | <span data-ttu-id="70458-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70458-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="70458-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70458-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="70458-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70458-119">Request headers</span></span>
| <span data-ttu-id="70458-120">Header</span><span class="sxs-lookup"><span data-stu-id="70458-120">Header</span></span>       | <span data-ttu-id="70458-121">Wert</span><span class="sxs-lookup"><span data-stu-id="70458-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70458-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70458-122">Authorization</span></span>  | <span data-ttu-id="70458-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="70458-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70458-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70458-125">Content-Type</span></span>  | <span data-ttu-id="70458-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70458-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70458-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70458-127">Request body</span></span>
<span data-ttu-id="70458-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [CalendarGroup](../resources/calendargroup.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="70458-128">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="70458-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="70458-129">Response</span></span>

<span data-ttu-id="70458-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [CalendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70458-130">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70458-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70458-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70458-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70458-132">Request</span></span>
<span data-ttu-id="70458-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70458-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="70458-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [calendarGroup](../resources/calendargroup.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="70458-134">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="70458-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="70458-135">Response</span></span>
<span data-ttu-id="70458-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70458-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

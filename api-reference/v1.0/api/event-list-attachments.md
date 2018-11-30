---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste der einem Ereignis angefügten Objekte des Typs attachment abrufen.
ms.openlocfilehash: 4ba864aad8e36429354bd7aa71bca061bba9f7d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019132"
---
# <a name="list-attachments"></a><span data-ttu-id="38ad1-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="38ad1-103">List attachments</span></span>

<span data-ttu-id="38ad1-104">Mit dieser API können Sie eine Liste der einem Ereignis angefügten Objekte des Typs [attachment](../resources/attachment.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="38ad1-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>
## <a name="permissions"></a><span data-ttu-id="38ad1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38ad1-105">Permissions</span></span>
<span data-ttu-id="38ad1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38ad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38ad1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38ad1-108">Permission type</span></span>      | <span data-ttu-id="38ad1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38ad1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38ad1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38ad1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38ad1-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="38ad1-111">Calendars.Read</span></span>    |
|<span data-ttu-id="38ad1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38ad1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38ad1-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="38ad1-113">Calendars.Read</span></span>    |
|<span data-ttu-id="38ad1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38ad1-114">Application</span></span> | <span data-ttu-id="38ad1-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="38ad1-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="38ad1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38ad1-116">HTTP request</span></span>
<span data-ttu-id="38ad1-117">Anlagen für ein [Ereignis](../resources/event.md) in der Benutzer als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="38ad1-117">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments
GET /users/{id | userPrincipalName}/events/{id}/attachments

GET /me/calendar/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
GET /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="38ad1-118">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="38ad1-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="38ad1-119">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="38ad1-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="38ad1-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="38ad1-120">Optional query parameters</span></span>
<span data-ttu-id="38ad1-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="38ad1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="38ad1-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38ad1-122">Request headers</span></span>
| <span data-ttu-id="38ad1-123">Name</span><span class="sxs-lookup"><span data-stu-id="38ad1-123">Name</span></span>       | <span data-ttu-id="38ad1-124">Typ</span><span class="sxs-lookup"><span data-stu-id="38ad1-124">Type</span></span> | <span data-ttu-id="38ad1-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38ad1-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="38ad1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="38ad1-126">Authorization</span></span>  | <span data-ttu-id="38ad1-127">string</span><span class="sxs-lookup"><span data-stu-id="38ad1-127">string</span></span>  | <span data-ttu-id="38ad1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38ad1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38ad1-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38ad1-130">Request body</span></span>
<span data-ttu-id="38ad1-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="38ad1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38ad1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="38ad1-132">Response</span></span>

<span data-ttu-id="38ad1-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38ad1-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38ad1-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38ad1-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38ad1-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38ad1-135">Request</span></span>
<span data-ttu-id="38ad1-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38ad1-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="38ad1-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="38ad1-137">Response</span></span>
<span data-ttu-id="38ad1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38ad1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
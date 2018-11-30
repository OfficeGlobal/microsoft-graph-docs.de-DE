---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste der einem Ereignis angefügten Objekte des Typs attachment abrufen.
ms.openlocfilehash: cc632ab14bf2c64628cdf5177da5601f4b04f4d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059645"
---
# <a name="list-attachments"></a><span data-ttu-id="33eaa-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="33eaa-103">List attachments</span></span>

> <span data-ttu-id="33eaa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33eaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33eaa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33eaa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33eaa-106">Mit dieser API können Sie eine Liste der einem Ereignis angefügten Objekte des Typs [attachment](../resources/attachment.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="33eaa-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="33eaa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="33eaa-107">Permissions</span></span>
<span data-ttu-id="33eaa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33eaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33eaa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33eaa-110">Permission type</span></span>      | <span data-ttu-id="33eaa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33eaa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33eaa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33eaa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33eaa-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="33eaa-113">Calendars.Read</span></span>    |
|<span data-ttu-id="33eaa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33eaa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33eaa-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="33eaa-115">Calendars.Read</span></span>    |
|<span data-ttu-id="33eaa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33eaa-116">Application</span></span> | <span data-ttu-id="33eaa-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="33eaa-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="33eaa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33eaa-118">HTTP request</span></span>
<span data-ttu-id="33eaa-119">Anlagen für ein [Ereignis](../resources/event.md) in der Benutzer als [Kalender](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="33eaa-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="33eaa-120">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="33eaa-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

GET /me/calendargroup/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="33eaa-121">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="33eaa-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33eaa-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="33eaa-122">Optional query parameters</span></span>
<span data-ttu-id="33eaa-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="33eaa-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="33eaa-124">Insbesondere können Sie die $ Abfragezeichenfolgen-Parameter, um alle für das Ereignis Anlagen Inline mit dem Rest der Ereigniseigenschaften erweitern.</span><span class="sxs-lookup"><span data-stu-id="33eaa-124">In particular, you can use the $expand query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="33eaa-125">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="33eaa-125">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```


## <a name="request-headers"></a><span data-ttu-id="33eaa-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33eaa-126">Request headers</span></span>
| <span data-ttu-id="33eaa-127">Name</span><span class="sxs-lookup"><span data-stu-id="33eaa-127">Name</span></span>       | <span data-ttu-id="33eaa-128">Typ</span><span class="sxs-lookup"><span data-stu-id="33eaa-128">Type</span></span> | <span data-ttu-id="33eaa-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33eaa-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="33eaa-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="33eaa-130">Authorization</span></span>  | <span data-ttu-id="33eaa-131">string</span><span class="sxs-lookup"><span data-stu-id="33eaa-131">string</span></span>  | <span data-ttu-id="33eaa-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="33eaa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33eaa-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33eaa-134">Request body</span></span>
<span data-ttu-id="33eaa-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="33eaa-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33eaa-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="33eaa-136">Response</span></span>

<span data-ttu-id="33eaa-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33eaa-137">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33eaa-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33eaa-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33eaa-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33eaa-139">Request</span></span>
<span data-ttu-id="33eaa-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33eaa-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="33eaa-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="33eaa-141">Response</span></span>
<span data-ttu-id="33eaa-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33eaa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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
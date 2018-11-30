---
title: Ereignis erstellen
description: Mit dieser API können Sie einen neuen Termin erstellen.
ms.openlocfilehash: 19f37edcf1862e8fdd89e08111bd55bd4b416d46
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057958"
---
# <a name="create-event"></a><span data-ttu-id="116b1-103">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="116b1-103">Create event</span></span>

> <span data-ttu-id="116b1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="116b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="116b1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="116b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="116b1-106">Mit dieser API können Sie einen neuen [Termin](../resources/event.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="116b1-106">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="116b1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="116b1-107">Permissions</span></span>
<span data-ttu-id="116b1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="116b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="116b1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="116b1-110">Permission type</span></span>      | <span data-ttu-id="116b1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="116b1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="116b1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="116b1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="116b1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="116b1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="116b1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="116b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="116b1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="116b1-115">Not supported.</span></span>    |
|<span data-ttu-id="116b1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="116b1-116">Application</span></span> | <span data-ttu-id="116b1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="116b1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="116b1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="116b1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="116b1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="116b1-119">Request headers</span></span>
| <span data-ttu-id="116b1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="116b1-120">Header</span></span>       | <span data-ttu-id="116b1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="116b1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="116b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="116b1-122">Authorization</span></span>  | <span data-ttu-id="116b1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="116b1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="116b1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="116b1-125">Request body</span></span>
<span data-ttu-id="116b1-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="116b1-126">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="116b1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="116b1-127">Response</span></span>
<span data-ttu-id="116b1-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="116b1-128">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="116b1-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="116b1-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="116b1-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="116b1-130">Request</span></span>
<span data-ttu-id="116b1-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="116b1-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="116b1-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="116b1-132">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="116b1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="116b1-133">Response</span></span>
<span data-ttu-id="116b1-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="116b1-134">The following is an example of the response.</span></span>
><span data-ttu-id="116b1-135">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="116b1-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="116b1-136">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="116b1-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

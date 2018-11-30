---
title: Ereignis erstellen
description: Mit dieser API können Sie einen neuen Termin erstellen.
ms.openlocfilehash: 79d5b4289c3326a02c279ea8e48fc5fef19a7797
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019925"
---
# <a name="create-event"></a><span data-ttu-id="bcd37-103">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="bcd37-103">Create event</span></span>
<span data-ttu-id="bcd37-104">Mit dieser API können Sie einen neuen [Termin](../resources/event.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bcd37-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bcd37-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bcd37-105">Permissions</span></span>
<span data-ttu-id="bcd37-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcd37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcd37-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bcd37-108">Permission type</span></span>      | <span data-ttu-id="bcd37-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bcd37-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcd37-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bcd37-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bcd37-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd37-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcd37-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bcd37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcd37-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcd37-113">Not supported.</span></span>    |
|<span data-ttu-id="bcd37-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bcd37-114">Application</span></span> | <span data-ttu-id="bcd37-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcd37-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcd37-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcd37-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="bcd37-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bcd37-117">Request headers</span></span>
| <span data-ttu-id="bcd37-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bcd37-118">Header</span></span>       | <span data-ttu-id="bcd37-119">Wert</span><span class="sxs-lookup"><span data-stu-id="bcd37-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcd37-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcd37-120">Authorization</span></span>  | <span data-ttu-id="bcd37-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bcd37-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcd37-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bcd37-123">Request body</span></span>
<span data-ttu-id="bcd37-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bcd37-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bcd37-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcd37-125">Response</span></span>
<span data-ttu-id="bcd37-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bcd37-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcd37-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bcd37-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bcd37-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcd37-128">Request</span></span>
<span data-ttu-id="bcd37-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bcd37-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="bcd37-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bcd37-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="bcd37-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcd37-131">Response</span></span>
<span data-ttu-id="bcd37-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bcd37-132">The following is an example of the response.</span></span>
><span data-ttu-id="bcd37-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="bcd37-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
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
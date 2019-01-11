---
title: Ereignis erstellen
description: Mit dieser API können Sie einen neuen Termin erstellen.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 4b7e0803b6eb59a2446da658815c19d08256587b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883909"
---
# <a name="create-event"></a><span data-ttu-id="337fe-103">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="337fe-103">Create event</span></span>

> <span data-ttu-id="337fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="337fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="337fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="337fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="337fe-106">Mit dieser API können Sie einen neuen [Termin](../resources/event.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="337fe-106">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="337fe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="337fe-107">Permissions</span></span>
<span data-ttu-id="337fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="337fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="337fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="337fe-110">Permission type</span></span>      | <span data-ttu-id="337fe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="337fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="337fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="337fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="337fe-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="337fe-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="337fe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="337fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="337fe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="337fe-115">Not supported.</span></span>    |
|<span data-ttu-id="337fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="337fe-116">Application</span></span> | <span data-ttu-id="337fe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="337fe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="337fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="337fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="337fe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="337fe-119">Request headers</span></span>
| <span data-ttu-id="337fe-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="337fe-120">Header</span></span>       | <span data-ttu-id="337fe-121">Wert</span><span class="sxs-lookup"><span data-stu-id="337fe-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="337fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="337fe-122">Authorization</span></span>  | <span data-ttu-id="337fe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="337fe-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="337fe-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="337fe-125">Request body</span></span>
<span data-ttu-id="337fe-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="337fe-126">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="337fe-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="337fe-127">Response</span></span>
<span data-ttu-id="337fe-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="337fe-128">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="337fe-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="337fe-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="337fe-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="337fe-130">Request</span></span>
<span data-ttu-id="337fe-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="337fe-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="337fe-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="337fe-132">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="337fe-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="337fe-133">Response</span></span>
<span data-ttu-id="337fe-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="337fe-134">The following is an example of the response.</span></span>
><span data-ttu-id="337fe-135">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="337fe-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="337fe-136">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="337fe-136">All the properties will be returned from an actual call.</span></span>
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
